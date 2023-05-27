# GLOB_RECURSE：允许 * 匹配嵌套的目录
# CONFIGURE_DEPENDS：让每次 cmake --build 时自动检测目录是否更新
# 将src文件夹及其子文件夹下的所有.cpp文件与include文件夹及其子文件夹下的所有.h文件加到src变量中
# 之所以添加头文件，是为了让Visual Studio可以识别到头文件并纳入 VS 的项目资源浏览器
file(GLOB_RECURSE srcs CONFIGURE_DEPENDS src/*.cpp include/*.h)
# 添加要生成的可执行程序
add_executable(tinyrenderer ${srcs})
# 指定头文件目录
target_include_directories(tinyrenderer PUBLIC include)


