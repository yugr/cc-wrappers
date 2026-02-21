Shell wrappers for GCC drivers to simplify compiler replacements
in various situations.

This is mainly to work around cases when `CC`, `CXX` or flags
environment variables are not respected by projects.

To use, define
```
export WRAPPER_CC=/path/to/c-compiler WRAPPER_CXX=/path/to/cxx-compiler
```
and optionally
```
export WRAPPER_CFLAGS=... WRAPPER_CXXFLAGS=... WRAPPER_PRE_CFLAGS=... WRAPPER_PRE_CXXFLAGS
```
