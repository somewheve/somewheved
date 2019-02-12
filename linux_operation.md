# linux opreation

- 在当前目录下查找指定名称的字符串
''' find /path/ -name "filename" '''

- 当前目录搜索文件内容含有某字符的文件
''' find /path f | xargs grep "file content"  '''

- 查找指定类型文件含有某字符串
''' find /path f -name "*.sh" | xargs grep -i "file content" '''




