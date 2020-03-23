# Git Files To Automate Creating Unity Projects

Add the function below to ~/.bash_profile

`
setupunity() {

    git init
    curl -o .gitignore https://raw.githubusercontent.com/github/gitignore/master/Unity.gitignore
    git add .
    git commit -m "Initial commit."

}
`

