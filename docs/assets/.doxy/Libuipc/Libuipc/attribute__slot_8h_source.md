

# File attribute\_slot.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_slot.h**](attribute__slot_8h.md)

[Go to the documentation of this file](attribute__slot_8h.md)


```C++
#pragma once
#include <uipc/common/smart_pointer.h>
#include <uipc/geometry/attribute.h>
#include <map>
#include <uipc/common/exception.h>
#include <uipc/backend/buffer_view.h>
#include <uipc/common/buffer_info.h>
#include <chrono>
namespace uipc::geometry
{
using TimePoint = std::chrono::time_point<std::chrono::high_resolution_clock>;
class AttributeCollection;
class UIPC_CORE_API IAttributeSlot
{
  public:
    template <typename T>
    friend class AttributeFriend;

    IAttributeSlot()          = default;
    virtual ~IAttributeSlot() = default;
    // delete copy_from
    IAttributeSlot(const IAttributeSlot&)            = delete;
    IAttributeSlot& operator=(const IAttributeSlot&) = delete;
    // enable move
    IAttributeSlot(IAttributeSlot&&) noexcept            = default;
    IAttributeSlot& operator=(IAttributeSlot&&) noexcept = default;

    [[nodiscard]] std::string_view name() const noexcept;

    [[nodiscard]] std::string_view type_name() const noexcept;

    [[nodiscard]] bool allow_destroy() const noexcept;

    [[nodiscard]] bool is_shared() const noexcept;

    [[nodiscard]] SizeT size() const noexcept;

    [[nodiscard]] Json to_json() const;

    [[nodiscard]] bool is_evolving() const noexcept;
    void               is_evolving(bool v) noexcept;

    [[nodiscard]] TimePoint last_modified() const noexcept;

  protected:
    friend class AttributeCollection;

    virtual std::string_view get_name() const noexcept          = 0;
    virtual bool             get_allow_destroy() const noexcept = 0;

    virtual bool get_is_evolving() const noexcept = 0;
    virtual void set_is_evolving(bool v) noexcept = 0;

    void         make_owned();
    virtual void do_make_owned() = 0;

    SizeT         use_count() const;
    virtual SizeT get_use_count() const = 0;

    S<IAttributeSlot> clone(std::string_view name, bool allow_destroy) const;
    virtual S<IAttributeSlot> do_clone(std::string_view name, bool allow_destroy) const = 0;

    S<IAttributeSlot> clone_empty(std::string_view name, bool allow_destroy) const;
    virtual S<IAttributeSlot> do_clone_empty(std::string_view name,
                                             bool allow_destroy) const = 0;

    void         share_from(const IAttributeSlot& other) noexcept;
    virtual void do_share_from(const IAttributeSlot& other) noexcept = 0;

    virtual IAttribute&       attribute() noexcept;
    virtual IAttribute&       get_attribute() noexcept = 0;
    virtual const IAttribute& attribute() const noexcept;
    virtual const IAttribute& get_attribute() const noexcept     = 0;
    virtual TimePoint         get_last_modified() const noexcept = 0;
};

template <typename T>
class AttributeSlot final : public IAttributeSlot
{
  public:
    using value_type = T;

    AttributeSlot(std::string_view m_name, S<Attribute<T>> attribute, bool allow_destroy);

    template <typename U>
    friend span<U> view(AttributeSlot<U>& slot);

    [[nodiscard]] span<const T> view() const noexcept;

  private:
    friend class AttributeCollection;

    virtual std::string_view get_name() const noexcept override;
    virtual bool             get_allow_destroy() const noexcept override;
    virtual bool             get_is_evolving() const noexcept;
    virtual void             set_is_evolving(bool v) noexcept;

    virtual IAttribute&       get_attribute() noexcept override;
    virtual const IAttribute& get_attribute() const noexcept override;
    virtual SizeT             get_use_count() const noexcept override;


    void do_make_owned() override;
    virtual S<IAttributeSlot> do_clone(std::string_view name, bool allow_destroy) const override;
    virtual S<IAttributeSlot> do_clone_empty(std::string_view name,
                                             bool allow_destroy) const override;
    virtual void do_share_from(const IAttributeSlot& other) noexcept override;
    virtual TimePoint get_last_modified() const noexcept override;

    TimePoint       m_last_modified;
    std::string     m_name;
    S<Attribute<T>> m_attribute;
    bool            m_allow_destroy;
    bool            m_is_evolving = false;
};
}  // namespace uipc::geometry
#include "details/attribute_slot.inl"
```


