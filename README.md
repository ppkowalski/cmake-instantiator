# cmake-instantiator

Sample usage:

```
SET(supprted_types nt "unsigned int" "long long" short "unsigned long") 

INSTANTIATE_CPP(
  SRCS
  LEVELS 1
  VALUES ${supported_types}
  TARGETS Something.instance0.cxx
)

add_library(Something ${SRCS} Something.h)
target_include_directories(Something PRIVATE ${CMAKE_CURRENT_LIST_DIR})
```
