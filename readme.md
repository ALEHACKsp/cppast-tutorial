# Tutorial

1. Install Windows SDK 

Configure test.bat

2.	Install LLVM 5.0.1 x64
	path:  D:/Program Files/LLVM
	
## Example 

```
cppast.exe --file t.cpp -v --msvc_extensions --msvc_compatibility -I"C:\Program Files (x86)\Windows Kits\10\Include\10.0.18362.0" -D UNICODE -D _UNICODE -D _DEBUG -D _CONSOLE
```	

### Output

```
AST for 't.cpp':
|-iostream (include directive): `#include <iostream>`
|-_ALLOW_COMPILER_AND_STL_VERSION_MISMATCH (macro definition): `#define _ALLOW_COMPILER_AND_STL_VERSION_MISMATCH`
+-printcoll (function template) [definition]: `template<typename T> void printcoll(T const& coll);`
```