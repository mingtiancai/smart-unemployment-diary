# 1.编译安装第三方库

源码编译glfw3源码，glad是下载的python库，然后根据命令行提示自己根据实际开发环境生成的。

同时还编译了boost，因为不知要做learnOpengl中的demo，更要形成一个软件，至少给自己开发大型3d图形仿真软件摸索设计架构开发经验。

相关的软件项目地址：
https://github.com/mingtiancai/Real-Time-Rendering-Cpp17

不过learOpenGL仅仅是examples中的一部分。咱所图者大！

# 2.helloWindow

glfwInit---初始化GLFW
glfwWindowHint---配置glfw一些参数

GLAD用来管理opengl函数的指针
```cpp
if (!gladLoadGLLoader((GLADloadproc)glfwGetProcAddress))
{
    std::cout << "Failed to initialize GLAD" << std::endl;
    return -1;
}    
```

