# vscode-settings
VS Code settings for bootstrapping projects. This is mainly for my convenience. If it helps you out...great :)

## dotnet
 - build and test tasks
 - Ignore dotnet files from the explorer
 - ReSharper Shortcuts. keybindings.json can be copied to `Preference: Open Keyboard Shortcuts File`

### Extensions
```sh
code --install-extension ms-vscode.csharp
code --install-extension jmrog.vscode-nuget-package-manager
```

## Node.js

### Extensions
```sh
# ESLint: Create ESLint configuration
code --install-extension dbaeumer.vscode-eslint
```

### Packages
```sh
npm i -D jest
```

## AWS SAM
### Installation
```sh
# install docker
pip install aws-sam-cli
pip install awscli

sam init -r nodejs8.10 -n my-app
cd my-app/hello_world
npm install
```

### Debugging
```sh
# API debugging setup
# termimal A
cd my-app
sam local start-api -d 5858

# terminal B
curl 127.0.0.1:3000/hello
```

```sh
# non-API debugging setup
echo {} | sam local invoke -d 5858
```

Edit-debug cycle
 - attach debugger. see launch.json
 - debug
 - debugger will detach itself after each request is complete
 - repeat


## All
```
code --install-extension eamodio.gitlens
```
