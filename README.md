# SpringBoot-log4j2-RCE

需要删除springboot自带的log4j，将jar手动添加到库中。


Linux平台检测：

```bash
for i in `find / -name log4j*.jar 2>/dev/null`;do echo $i |grep -E "log4j-(.*)?(api|core)-2\.([0-9][-\x2e]|[01][0-4])" ;done
```
