# winget-private

https://chatgpt.com/share/26950371-3bd9-468d-b0e2-39323f2d30eb
https://github.com/microsoft/winget-pkgs/blob/master/doc/tools/YamlCreate.md
https://blogs.infosupport.com/hosting-your-own-winget-private-repository/
https://blogs.infosupport.com/adding-a-package-to-your-private-winget-restsource-feed-using-its-api/
https://github.com/microsoft/winget-create
https://github.com/omaha-consulting/winget.pro

```PS (As Admin)
cd Tools
winget install wingetcreate
winget settings --enable LocalManifestFiles
wingetcreate new
```

```PS (Validate)
winget validate --manifest C:\Source\winget-private\manifests\d\Dell\MyDell\3.2.308.1
```

```PS (Install)
winget install --manifest C:\Source\winget-private\manifests\d\Dell\MyDell\3.2.308.1
```

```PS (Uninstall)
winget uninstall MyDell
```

```PS (Add GitRepo)
winget source add --name mdelgert --arg https://raw.githubusercontent.com/mdelgert/winget-private/main/manifests/
winget source list
```
