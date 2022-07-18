# Git

- ['GitHub 글 목록'](https://www.lainyzine.com/ko/subject/github/)을 참고하여 작성함.

## 초기 세팅

```
git config --global user.name "Your Name"
git config --global user.email you@example.com
```

## Create a new repository

```
git clone [URL]
cd [Dir]
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main
```

## Push an existing folder

```
cd existing_folder
git init --initial-branch=main
git remote add origin [URL]
git add .
git commit -m "Initial commit"
git push -u origin main
```

## Push an existing Git repository

```
cd existing_repo
git remote rename origin old-origin
git remote add origin [URL]
git push -u origin --all
git push -u origin --tags
```

## 원격저장소 초기화

```
rm -rf ./.git
git init
```

## push 후 gitignore 적용

```
git rm -r --cached .
git add .
git status
git commit -m "apply .gitignore"
git push
```
