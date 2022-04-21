# m-config 
## Manjaro Linux Config Files  

**ZSH** 

Add the following code to the .zshrc file at the bottom before p10k config: 

``` 
if [[ -e ~/m-config/zsh.ext ]]; then
  source ~/m-config/zsh.ext 
fi 
```
