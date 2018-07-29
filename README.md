# Auto Fish Config Cloud Storage

## Fish Shell
https://github.com/fish-shell/fish-shell

## Oh my Fish
https://github.com/oh-my-fish/oh-my-fish

## Installation

Once Fish shell and Oh My Fish is installed.
If your configuration is in your '~/.config' folder add this bash script
to store your fish configuration on your own GitHub repo.

```
cd
git clone https://github.com/laynef/Auto-Fish-Shell-Configs.git temp
cd ~/.config
git init
git remote add origin <YOUR-GITHUB-LINK>
cp ./../temp/save.sh ~/.config/save.sh
bash save.sh
git push --set-upstream origin master
rm -rf temp
```

Make your first git commit and push it up to your github repo

```
alias saveconfig 'bash ~/.config/save.sh'
funcsave saveconfig
saveconfig
```

Now run the command 'saveconfig' after any alias creation to keep stored on GitHub
```
saveconfig
```


Each time your run 'saveconfig' your configure for fish will be saved
in your own github repo. To get that data back

```
cd
git clone <YOUR-GITHUB-LINK> .config
```