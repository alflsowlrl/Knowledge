# How to use matplotlib-cpp in ros
---
install
```
cd ~
git clone https://github.com/lava/matplotlib-cpp.git
```
CMakeLists.txt
```
add_compile_options(-std=c++11 -I/usr/include/python2.7 -lpython2.7)
...
target_link_libraries(${your node name}
  ...
  python2.7
  ...
)
