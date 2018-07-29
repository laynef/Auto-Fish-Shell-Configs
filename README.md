# Auto Fish Config Cloud Storage

## Installation

Store your fish configuration on your own GitHub repo

```
cd
git clone https://github.com/laynef/Auto-Fish-Shell-Configs.git temp
cd ~/.config
git init
git remote add origin <YOUR-GITHUB-LINK>
cp ./../temp/save.sh ~/.config/save.sh
bash save.sh
git push origin 
```

Make your first git commit and push it up to your github repo

```
alias saveconfig 'bash ~/.config/save.sh'
funcsave saveconfig
saveconfig
```

Each time your run 'saveconfig' your configure for fish will be saved
in your own github repo. To get that data back

```
cd
git clone <YOUR-GITHUB-LINK> .config
```