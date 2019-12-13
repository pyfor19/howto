# How to GIT

## Usefull links

- Install [Git](https://www.git-scm.com/)
- [GitHub Cheat Sheet](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
  - [GitHub Guides](https://guides.github.com/)
- [Setup Guide (French)](https://git-scm.com/book/fr/v2D%C3%A9marrage-rapide-Param%C3%A9trage-%C3%A0-la-premi%C3%A8re-utilisation-de-Git)

  - [Git – Config Username & Password – Store Credentials](https://www.shellhacks.com/git-config-username-password-store-credentials/)
  - [Personnalisation de Git](https://git-scm.com/book/fr/v2/Personnalisation-de-Git-Configuration-de-Git)
  - [SSH Key](https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)
  - [How to setup SSH under Windows 10](https://dev.to/bdbch/setting-up-ssh-and-git-on-windows-10-2khk)

## Git setup

### Global setup

```
git config --global user.name "<user name>"
git config --global user.email "<email>"
git config --global color.ui true
git config --global core.autocrlf true
```

### .gitignore

- [.gitignore configurations files](https://github.com/github/gitignore)

### Create a new repository using https

```
git clone https://github.com/<my_git_profile>/<my_git_project>.git
cd <my_git_project>
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master
```

### Push an existing folder using ssh

```
cd <existing_folder>
git init
git remote add origin https://github.com/<my_git_profile>/<my_git_project>.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

### Push an existing Git repository using ssh

```
cd <existing_repo>
git remote rename origin old-origin
git remote add origin https://github.com/<my_git_profile>/<my_git_project>.git
git push -u origin --all
git push -u origin --tags
```
