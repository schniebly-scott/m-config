# m-config 
## Manjaro Linux Config Files  


**Common Commands** 

Commands that help for setting up linux

Trim SSD saver:
``` 
$ sudo systemctl status fstrim.timer
$ sudo systemctl enable fstrim.timer
```

**ZSH** 

Add the following code to the .zshrc file at the bottom before p10k config: 

``` 
if [[ -e ~/m-config/zsh.ext ]]; then
  source ~/m-config/zsh.ext 
fi 
```


**kitty** 

Run the following to create a hardlink: 

``` 
rm .config/kitty/kitty.conf
ln m-config/kitty.conf .config/kitty/kitty.conf
```
