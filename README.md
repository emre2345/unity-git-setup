# Git Files To Automate Creating Unity Projects

Add the function below to ~/.bash_profile

```
setupunity() {

    git init
    curl -o .gitignore https://raw.githubusercontent.com/emre2345/unity-git-setup/master/unity.gitignore
    curl -o .gitattributes https://raw.githubusercontent.com/emre2345/unity-git-setup/master/unity.gitattributes
    git add .
    git commit -m "Initial commit."

}
```

