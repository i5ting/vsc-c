# vscode c programming

http://code.visualstudio.com/docs/languages/cpp


## 安装

```
ext install c/c++
```

## 配置调试环境

使用`F5`快捷键，选`c/c++`即可生成luanch.json，默认即可

## 配置task

https://go.microsoft.com/fwlink/?LinkId=733558

.vscode/tasks.json

```
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "0.1.0",
    "command": "clang",
    "isShellCommand": true,
    "args": [
        "test.c", // 入口文件
        "-g",     // 是否生成调试信息
        "-O0",    // 提示编译速度
        "-m32"    // 64bit下
    ],
    "showOutput": "always"
}
```

## 编译

```
command+shift+b
```

## Debug

```
command+shift+d
```