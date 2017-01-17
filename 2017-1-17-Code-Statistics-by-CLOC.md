# 使用 CLOC 统计代码

CLOC（Counts Lines of Code）是一款特别好使的代码统计工具。它能统计出源码中的空行数，评论行数和实际代码行数，还能自动忽略重复文件，并且支持各种编程语言，实在是精准量化代码的好帮手👍！

## 使用
以 Mac 为例，打开终端：
```
cloc <path-to-file-or-directory>
```

结果样例：
```
5605 text files.
5386 unique files.
2176 files ignored.

https://github.com/AlDanial/cloc v 1.65  T=25.49 s (134.7 files/s, 51980.3 lines/s)
-----------------------------------------------------------------------------------
Language                         files          blank        comment           code
-----------------------------------------------------------------------------------
Perl                              2892         136396         184362         536445
C                                  130          24676          33684         155648
C/C++ Header                       148           9766          16569         147858
Bourne Shell                       112           4044           6796          42668
Pascal                               8            458           1603           8592
XML                                 33            142              0           2410
YAML                                49             20             15           2078
C++                                 10            313            277           2033
make                                 4            426            488           1986
Prolog                              12            438              2           1146
JSON                                14              1              0           1037
yacc                                 1             85             76            998
Windows Message File                 1            102             11            489
DOS Batch                           14             92             41            389
Windows Resource File                3             10              0             85
D                                    1              5              7              8
Lisp                                 2              0              3              4
-----------------------------------------------------------------------------------
SUM:                              3434         176974         243934         903874
-----------------------------------------------------------------------------------
```

## 安装
使用 [Homebrew](http://brew.sh) 安装：
```
brew install cloc
```

卸载：
```
brew uninstall cloc
```

如果 Homebrew 发生 `/usr/local must be writable.` 错误，请尝试：
```
sudo chown -R $<your-username>:<your-group-name> /usr/local
```
`username` 是 Mac 的登录用户名，`group-name` 是用户的组名，例如: Admin。

## 参考
1. [GitHub - AlDanial/cloc: cloc counts blank lines, comment lines, and physical lines of source code in many programming languages.](https://github.com/AlDanial/cloc#Options)
2. [Homebrew — The missing package manager for macOS](http://brew.sh)
3. [macos - Make files in `/usr/local` writable for homebrew - Ask Different](http://apple.stackexchange.com/questions/192227/make-files-in-usr-local-writable-for-homebrew)
