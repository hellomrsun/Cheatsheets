# services-status-check-cheatsheet

### 1. IIS website status check 

#### 1.1 Check all websites on IIS with status

```bash
> Invoke-Command -ComputerName $SERVER_NAME { Import-Module WebAdministration; Get-ChildItem -path IIS:\Sites | Format-Table }
```

ex:

| Name | ID | State | Physical Path |
| ---- | --- | --- | ------------- |
| site1 | 1 | Started | http *:: |
| site2 | 2 | Started | net.tcp :* |


#### 1.2 Check all sub-sites below a site on IIS

```bash
> Invoke-Command -ComputerName $SERVER_NAME { Import-Module WebAdministration; Get-ChildItem -path IIS:\Sites\$WEBSITE_NAME | Format-Table }
```

ex:

| Type | Name | Physical Path |
| ---- | --- | ------------- |
| application | subsite1 | D:\INETPUB\site1\subsite1 |
| application | subsite2 | D:\INETPUB\site1\subsite2 |


#### 1.3 Check all websites status with sub-sites on IIS

```bash
> Invoke-Command -ComputerName $SERVER_NAME { Import-Module WebAdministration; Get-ChildItem -path IIS:\AppPools | Format-Table }
```

ex:

| Type  | State   | Applications |
| ----  | ----    | ------------ |
| site1 | Started | subsite1     |
|       |         | subsite2     |
|       |         | subsite3     |
| site2 | Started | site2        |
| site3 | Started | site3        |




