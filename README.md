# 示例说明
1.已开放、测试通过：Triangle、Model Viewer、Area Lights、Audio、Box2D、2D Fluid Simulation、3D Fluid Simulation、Ray Tracing、Octree、ImGui、Animated GIF、Motion blur；
2.编译未通过的示例：Bullet Physics、DART Physics；
3.还有其他示例未测试，但估计问题不大；

# 生成vcpkg可执行文件

- windows下执行命令：
```bat
./vcpkg/bootstrap-vcpkg.bat
```

- linux/mac下执行命令：
```bash
./vcpkg/bootstrap-vcpkg.sh
```

# 安装依赖库

所有的依赖库全都是vcpkg支持的跨平台开源库，可以直接使用vcpkg安装。
- windows：执行文件`./vcpkg_install.bat`
- linux/mac：执行文件`./vcpkg_install.sh`


# CMake 构建

## Debug

```bat
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Debug
cmake --build . --config Debug  --target ALL_BUILD -j 16
```

## Release

```bat
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
cmake --build . --config Release --target ALL_BUILD -j 16
```