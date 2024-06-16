# winget-private

https://chatgpt.com/share/26950371-3bd9-468d-b0e2-39323f2d30eb
https://github.com/microsoft/winget-pkgs/blob/master/doc/tools/YamlCreate.md

```PS (As Admin)
cd Tools
winget settings --enable LocalManifestFiles
.\YamlCreate.ps1
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
winget source add --name mdelgert --arg https://github.com/mdelgert/winget-private/main/manifests/
```
