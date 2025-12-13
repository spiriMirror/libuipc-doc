

# File uid\_info.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**uid\_info.h**](uid__info_8h.md)

[Go to the documentation of this file](uid__info_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/string.h>
#include <uipc/common/json.h>
#include <uipc/common/list.h>
#include <functional>


namespace uipc::builtin
{
struct UIPC_CORE_API UIDInfo
{
    static constexpr U64 OfficialBuiltinUIDStart = 0;
    static constexpr U64 UserDefinedUIDStart     = 1ull << 32;

    U64    uid = 0;
    string name;
    string type;
    string author;
    string email;
    string website;
    string description;
    Json   extras;

    bool is_official_builtin_uid(U64 uid) const noexcept;

    bool is_user_defined_uid(U64 uid) const noexcept;

    Json to_json() const noexcept;
};

class UIPC_CORE_API UIDInfoCreator
{
  public:
    UIDInfoCreator(std::function<list<UIDInfo>()> creator, std::string_view file, int line) noexcept;

    list<UIDInfo> operator()() const;

    std::string_view file() const noexcept;
    int              line() const noexcept;

  private:
    std::function<list<UIDInfo>()> m_creator;
    std::string                    m_file;
    int                            m_line = 0;
};
}  // namespace uipc::builtin
```


