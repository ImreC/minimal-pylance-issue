# minimal-pylance-issue

The bug:
Pylance language server does not recognize editable installs. I tried a similar setup with Jedi and it works. It also works with all other tooling. 

What I am trying to do:
Install a package called `files` locally in editable mode through poetry. 

What I am expecting to happen:
Pylance recognizes the locally installed package when I select the proper interpreter path and offers intellisense

What actually happens:
```
Import "files" could not be resolved 
PylancereportMissingImports
```

System information: 

OS: `Pop!_OS 22.04 LTS (Ubuntu 22.04 LTS)`

vs-code about:
```
Version: 1.78.1
Commit: 6a995c4f4cc2ced6e3237749973982e751cb0bf9
Date: 2023-05-04T09:46:23.602Z
Electron: 22.5.1
Chromium: 108.0.5359.215
Node.js: 16.17.1
V8: 10.8.168.25-electron.0
OS: Linux x64 6.2.6-76060206-generic
Sandboxed: Yes
```

Pylance: `v2023.5.20`
