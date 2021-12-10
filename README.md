# LaZagne

Usage
----
* Launch all modules
```
laZagne.exe all
```

* Launch only a specific module
```
laZagne.exe browsers
```

* Launch only a specific software script
```
laZagne.exe browsers -firefox
```

* Write all passwords found into a file (-oN for Normal txt, -oJ for Json, -oA for All).
Note: If you have problems to parse JSON results written as a multi-line strings, check [this](https://github.com/AlessandroZ/LaZagne/issues/226). 
```
laZagne.exe all -oN
laZagne.exe all -oA -output C:\Users\test\Desktop
```

* Get help
```
laZagne.exe -h
laZagne.exe browsers -h
```


* Change verbosity mode (2 different levels)
```
laZagne.exe all -vv
```

* Quiet mode (nothing will be printed on the standard output)
```
laZagne.exe all -quiet -oA
```

* To decrypt domain credentials, it could be done specifying the user windows password. Otherwise it will try all passwords already found as windows passwords. 
```
laZagne.exe all -password ZapataVive
