# sync sublime text settings using git

## package folder

**windows:**
```C:\Users\[YourName]\AppData\Roaming\Sublime Text 3\Packages```

**mac:**
```/Library/Application\ Support/Sublime\ Text\ 2/Packages/```

**linux:**


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
git clone git@github.com:jive/sublimesettings.git User
```

## update settings from one of the machines
```
cd [package folder]/User
git commit -m "Update settings"
git push
```

## sync on other 
```
cd [package folder]/User
git pull
```
