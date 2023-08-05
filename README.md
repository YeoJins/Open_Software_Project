# Open_Software_Project

macbook m1에서 vscode로 opencv c++ 빌드

1. CMakeLists.txt 파일 수정
   
```cpp
cmake_minimum_required(VERSION 3.27.1)
project(Cproject)  // 프로젝트 이름
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(Cproject cat.cpp) // 프로젝트 이름 + cpp 파일 이름
target_link_libraries(Cproject ${OpenCV_LIBS}) // 프로젝트 이름
```
2. make하기

```cpp
// vscode 내의 터미널에서 진행
make
./Cproject
```
