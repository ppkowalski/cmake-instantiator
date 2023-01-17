# cmake-instantiator

Sample usage:

```
SET(supprted_types nt "unsigned int" "long long" short "unsigned long") 

INSTANTIATE_CPP(
  SRC
  LEVELS 1
  VALUES ${supported_types}
  TARGETS Something.instance0.cxx
)
```
