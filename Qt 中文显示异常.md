不保证百分百解决。
在软件文件夹下找到存放 Qt6Core.dll 等文件的文件夹，如果有 qt.conf，用文本编辑器打开，直接在内容里加上

```
[Platforms]
WindowsArguments=fontengine=freetype
```

如果 qt.conf 本身已经有一个 [Platforms] ，只要在其下加上 WindowsArguments=fontengine=freetype 。
如果没有 qt.conf ，新建一个 qt.conf ，写上代码块的内容，注意保存为 UTF-8 。
没看懂可以问 AI 。
