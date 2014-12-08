# sync sublime text settings using git

## package folder

**windows:**
```C:\Users\[YourName]\AppData\Roaming\Sublime Text 3\Packages```

**mac:**
```/Library/Application\ Support/Sublime\ Text\ 3/Packages/```

**linux:**


## files that should be ignored

**add following into your .gitignore file**

```
Package Control.last-run
Package Control.ca-list
Package Control.ca-bundle
Package Control.system-ca-bundle
Package Control.cache/
Package Control.ca-certs/
```

## on first machine

```
cd [package folder]/User/
git init
git add <files to share>
git commit -m "Initial"
git remote add origin [your git repo]
git push origin master
```
## on other machines
```
cd [package folder]
mv User User.old
git clone [your git repo] User
```

## update settings from one of the machines
```
cd [package folder]/User
git add -A
git commit -m "Update settings"
git push
```

## sync on other 
```
cd [package folder]/User
git pull
```
