# m-config 
## Manjaro Linux Config Files  


**Common Commands** 

Commands that help for setting up linux

Trim SSD saver:
``` 
$ sudo systemctl status fstrim.timer
$ sudo systemctl enable fstrim.timer
```

Change to zsh:
``` 
$ chsh
> /bin/zsh
```

Github cache credentials:
``` 
$ git config --global credential.helper cache
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


**vim** 

Run the following to create a hardlink: 

``` 
ln m-config/vimrc .vimrc
```


**awesome** 

First, run the following to create the directory needed in the next step:
``` 
$ mkdir -p ~/.config/awesome/
```

Create hardlinks for the configs:
``` 
$ ln m-config/awesome/rc.lua .config/awesome/rc.lua
```
