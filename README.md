# lab2-polytech-2.0
## Сборка IFile
cd libs && mkdir -p build && cd build && cmake .. && make
## Сборка всего проекта 
cd ../..
mkdir build && cd build
cmake .. -S .. -B .
make
ctest --output-on-failure
