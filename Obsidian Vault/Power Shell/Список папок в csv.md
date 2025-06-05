```powershell
Get-ChildItem -Path D:\ -Directory | Select-Object FullName | Export-Csv -Path D:\folders.csv -NoTypeInformation -Encoding "Unicode"
2
```