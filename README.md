# Git Files To Automate Creating Unity Projects

## For Mac OS X Users

Add the function below to ~/.bash_profile

```
setupunity() {

    git init
    curl -o .gitignore https://raw.githubusercontent.com/emre2345/unity-git-setup/master/unity.gitignore
    curl -o .gitattributes https://raw.githubusercontent.com/emre2345/unity-git-setup/master/unity.gitattributes
    cd Packages && curl -o manifest.json https://raw.githubusercontent.com/emre2345/unity-git-setup/master/unity.manifest && cd ..
    git add .
    git commit -m "Initial commit."

}

```

