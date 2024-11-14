

# File attribute\_copy.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_copy.h**](attribute__copy_8h.md)

[Go to the documentation of this file](attribute__copy_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/span.h>

namespace uipc::geometry
{
class UIPC_CORE_API AttributeCopy
{
    template <typename T>
    friend class Attribute;

  public:
    enum CopyType
    {
        None = 0,
        SameDim,
        Range,
        Pull,
        Push,
        Pair
    };

    CopyType type() const noexcept;

    AttributeCopy() noexcept;

    static AttributeCopy range(SizeT dst_offset, SizeT src_offset, SizeT count) noexcept;
    static AttributeCopy pull(span<const SizeT> mapping) noexcept;
    static AttributeCopy push(span<const SizeT> mapping) noexcept;

    static AttributeCopy pair(span<const std::pair<SizeT, SizeT>> pairs) noexcept;

  private:
    CopyType m_type = CopyType::None;

    // Range
    SizeT m_dst_offset = ~0ull;
    SizeT m_src_offset = ~0ull;
    SizeT m_count      = ~0ull;

    // pull, push
    span<const SizeT> m_mapping;

    // pair mapping
    span<const std::pair<SizeT, SizeT>> m_pairs;

    template <typename T>
    void copy(span<T> dst, span<const T> src) const noexcept;
};
}  // namespace uipc::geometry

#include "details/attribute_copy.inl"
```


