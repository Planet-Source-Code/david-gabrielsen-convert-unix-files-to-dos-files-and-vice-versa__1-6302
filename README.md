<div align="center">

## Convert UNIX files to DOS files and vice versa


</div>

### Description

This code converts UNIX files to DOS files and DOS files to UNIX files
 
### More Info
 
the text to be converted

This code has 2 Functions. One function that takes a DOS string as argument and returns a UNIX string, and one function that takes a UNIX string as argument and returns a DOS string.

UNIX or DOS text

absolutely none


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[David Gabrielsen](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/david-gabrielsen.md)
**Level**          |Intermediate
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__1-5.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/david-gabrielsen-convert-unix-files-to-dos-files-and-vice-versa__1-6302/archive/master.zip)





### Source Code

```
Private Function convertDOStoUNIX(DOSstring As String) As String
 convertDOStoUNIX = Replace(DOSstring, vbCrLf, vbLf, 1, Len(DOSstring), vbTextCompare)
End Function
Private Function convertUNIXtoDOS(UNIXstring As String) As String
 convertUNIXtoDOS = Replace(UNIXstring, vbLf, vbCrLf, 1, Len(UNIXstring), vbTextCompare)
End Function
```

