# A Simple Way to Use Imgui in Ubuntu


## Preparation
+ OpenGl
```bash
sudo apt-get install build-essential

sudo apt-get install libgl1-mesa-dev

sudo apt-get install libglu1-mesa-dev
```

+Glfw3
Downloads release from https://www.glfw.org/ and extract
```bash
cd glfw-3.3.6
mkdir build & cd build
cmake ..
make
sudo make install
```

## Usage
```bash
cd imgui_test
mkdir build & cd build
cmake ..
make
./imgui_test
```