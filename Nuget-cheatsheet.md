# Nuget-commands-cheatsheet

## 1. Nuget http proxy

### Set http proxy

```bash
> nuget.exe config -set http_proxy=http://{proxy}:{port}
> nuget.exe config -set http_proxy.user={domain}\{user}
> nuget.exe config -set http_proxy.password={password}
```

### Get http proxy name

```bash
> nuget.exe config http_proxy
```

### Get http proxy user

```bash
> nuget.exe config http_proxy.user
```

### Get http proxy password

```bash
> nuget.exe config http_proxy.password
```

or just go to folder  
**%appdata%\NuGet\NuGet.Config**

same as 

**C:\Users\{user_profile}\AppData\Roaming\NuGet\NuGet.Config**

You can see the content like this:

```bash
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <packageSources>
    <add key="nuget.org" value="https://api.nuget.org/v3/index.json" protocolVersion="3" />
  </packageSources>
  <config>
    <add key="http_proxy" value="http://" />
    <add key="http_proxy.user" value="" />
    <add key="http_proxy.password" value="" />
  </config>
</configuration>
```


