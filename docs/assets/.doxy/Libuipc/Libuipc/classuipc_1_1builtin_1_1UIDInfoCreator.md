

# Class uipc::builtin::UIDInfoCreator



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**builtin**](namespaceuipc_1_1builtin.md) **>** [**UIDInfoCreator**](classuipc_1_1builtin_1_1UIDInfoCreator.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**UIDInfoCreator**](#function-uidinfocreator) (std::function&lt; list&lt; [**UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) &gt;()&gt; creator, std::string\_view file, int line) noexcept<br> |
|  std::string\_view | [**file**](#function-file) () noexcept const<br> |
|  int | [**line**](#function-line) () noexcept const<br> |
|  list&lt; [**UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) &gt; | [**operator()**](#function-operator) () const<br> |




























## Public Functions Documentation




### function UIDInfoCreator 

```C++
uipc::builtin::UIDInfoCreator::UIDInfoCreator (
    std::function< list< UIDInfo >()> creator,
    std::string_view file,
    int line
) noexcept
```




<hr>



### function file 

```C++
std::string_view uipc::builtin::UIDInfoCreator::file () noexcept const
```




<hr>



### function line 

```C++
int uipc::builtin::UIDInfoCreator::line () noexcept const
```




<hr>



### function operator() 

```C++
list< UIDInfo > uipc::builtin::UIDInfoCreator::operator() () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/uid_info.h`

