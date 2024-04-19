
# CMake

Edit:  
(CMakeLists.txt)   

CMDs:  
```
cmake -G{GENERATOR_NAME} -B{BUILD_DIR_PATH} -H{SOURCE_DIR_PATH}

cmake --build {BUILD_DIR_PATH} --target ALL_BUILD --config {BUILD_TYPE}
```



Ex.  
cmake -S . -B ..\libbbuild   
 
cd  ..\libbbuild     

cmake --build . --target ALL_BUILD --config Release  
