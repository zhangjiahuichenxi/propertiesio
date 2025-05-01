这是一个用于读写properties文件的python库
示例：
```
#!/usr/bin/python
# -*- coding: utf-8 -*-

import propertiesIO

file_path = '/Users/billy/Desktop/bak/test.properties' #要操作的properties文件的路径
props = propertiesIO.parse(file_path)   #读取文件
props.put('key_a', 'value_a')       #修改/添加key=value
print(props.get('key_a'))            #根据key读取value
print("props.has_key('key_a')=" + str(props.has_key('key_a')))   #判断是否包含该key1```
