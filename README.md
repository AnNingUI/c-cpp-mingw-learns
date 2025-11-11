这是我在我学校之外学到的 C/CPP 小知识

注：
  - 这里不涉及 C/CPP 语法的教学
  - 有任何错误 请提交 issue 或者 pr 指正

1. [MSYS2-MINGW环境配置](./1.MSYS2-MINGW环境配置.md)
2. [多文件编程与构建系统](./2.多文件编程与构建系统.md)
3. [使用第三方库](./3.使用第三方库.md)
4. [使用wxwidgets](./4.使用wxwidgets.md)

---

## Q & A
```
Q:
  适合 macos / linux 嘛
A:
  由于我的电脑是 windows
  所以这些经验只适合 windows

Q:
  为什么不用 Windows MSVC 的工具
  如 Visual Studio 2022, vcpkg
A:
  Visual Studio 2022 太依赖 GUI 了，大部分选项需要找半天，学到的知识也不好迁移
  vcpkg 大部分包甚至无法编译通过

Q:
  使用 IDE 推荐那些
A:
  vscode + clangd插件
  zed      [zed clangd 开箱即用  ]
  Clion    [Clion clangd 开箱即用]

Q:
  gcc 是什么，cmake,make,meson,ninja又是什么
A:
  见参考，gcc 是 最基础的编译器，make和ninja是组织编译器编译的工具，cmake和meson则是跨平台组织`组织编译器编译的工具`的工具
  另外除了 gcc 之外还有其他基础编译器，比如 llvm 的 clang, 还有 tcc 等，但在这里不是我们要涉及的内容
```



## 参考
1. what is gcc, cmake, make, meson, ninja ?

| 名称        | 作用                                     | 类比理解       |
| --------- | -------------------------------------- | ---------- |
| **GCC**   | 把源代码编译成可执行文件的**编译器**                   | 翻译员        |
| **Make**  | 读取 `Makefile`，按规则自动执行编译命令的**构建工具**     | 执行编译指令的工头  |
| **Ninja** | 比 Make 更快的**构建执行器**                    | 高效的工头      |
| **CMake** | 生成 `Makefile` 或 `Ninja` 脚本的**构建系统生成器** | 会写计划书的工程经理 |
| **Meson** | 比 CMake 更新、更简洁的**构建系统生成器**             | 更现代的工程经理   |
