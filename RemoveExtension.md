remove all the extention .txt of the files in a folder
```batch
ren *.txt *.
```
or
```batch
@ECHO OFF
FOR %%f IN (*.txt) DO RENAME "%%f" "%%~nf"`
```

do it recursivly
```batch
@ECHO OFF
FOR /R %%f IN (*.txt) DO RENAME "%%f" "%%~nf"`
```

---
ref: [SO](http://stackoverflow.com/questions/6401928/batch-file-remove-second-file-extension)
