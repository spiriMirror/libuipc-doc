

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
namespace uipc::geometry
{
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

    [[nodiscard]] Json to_json(SizeT i) const;

    [[nodiscard]] Json to_json() const;

    friend backend::BufferView backend_view(const IAttributeSlot&) noexcept;

  protected:
    friend class AttributeCollection;

    [[nodiscard]] virtual std::string_view get_name() const noexcept = 0;
    [[nodiscard]] virtual bool get_allow_destroy() const noexcept    = 0;

    void         make_owned();
    virtual void do_make_owned() = 0;

    [[nodiscard]] SizeT         use_count() const;
    [[nodiscard]] virtual SizeT get_use_count() const = 0;

    [[nodiscard]] virtual S<IAttributeSlot> clone(std::string_view name,
                                                  bool allow_destroy) const;
    [[nodiscard]] virtual S<IAttributeSlot> do_clone(std::string_view name,
                                                     bool allow_destroy) const = 0;
    [[nodiscard]] virtual S<IAttributeSlot> clone_empty(std::string_view name,
                                                        bool allow_destroy) const;
    [[nodiscard]] virtual S<IAttributeSlot> do_clone_empty(std::string_view name,
                                                           bool allow_destroy) const = 0;

    [[nodiscard]] virtual IAttribute&       attribute() noexcept;
    [[nodiscard]] virtual IAttribute&       get_attribute() noexcept = 0;
    [[nodiscard]] virtual const IAttribute& attribute() const noexcept;
    [[nodiscard]] virtual const IAttribute& get_attribute() const noexcept = 0;
    [[nodiscard]] virtual Json              do_to_json(SizeT i) const      = 0;
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

  protected:
    friend class AttributeCollection;
    // [[nodiscard]] virtual const BufferInfo& get_buffer_info() const noexcept override;

    [[nodiscard]] virtual std::string_view get_name() const noexcept override;
    [[nodiscard]] virtual bool get_allow_destroy() const noexcept override;

    [[nodiscard]] virtual IAttribute& get_attribute() noexcept override;
    [[nodiscard]] virtual const IAttribute& get_attribute() const noexcept override;
    [[nodiscard]] virtual SizeT get_use_count() const noexcept override;


    void                                    do_make_owned() override;
    [[nodiscard]] virtual S<IAttributeSlot> do_clone(std::string_view name,
                                                     bool allow_destroy) const override;
    [[nodiscard]] virtual S<IAttributeSlot> do_clone_empty(std::string_view name,
                                                           bool allow_destroy) const override;

    [[nodiscard]] virtual Json do_to_json(SizeT i) const override;

  private:
    pmr::string     m_name;
    S<Attribute<T>> m_attribute;
    bool            m_allow_destroy;
};
}  // namespace uipc::geometry
#include "details/attribute_slot.inl"
```


