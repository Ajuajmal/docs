# Setting invalid path

> Setting invalid path may leads to crash the terminal commands / bash /

eg :-

 `bash: ls: command not found`

 `bash: dircolors: command not found`

## Error on .bashrc

 exporting a PATH with missing basic PATH configs: -

 `export PATH=$HOME/.cargo/bin`

 but required `:$PATH` at the end ,

 `export PATH=$HOME/.cargo/bin:$PATH`




## Fix By Following ( Debian 10)

> Opened the .bashrc using text-editor and made the changes as above or alternatively you can comment out the recently added paths and  
excecute the following :-

>`Note`  I excecuted in  2 terminal session and opend 3 rd terminal session for checking the all the commands is working now. I closed the following 2 terminal session by CTRL+C after checking few commands is working.


 ` /usr/bin/find / -name ls 2> /dev/null`

 ` /usr/bin/grep -rn --color "export PATH" ~/. 2> /dev/null`

>`Solution Source` [https://devconnected.com/command-not-found-in-bash-fixed/](https://devconnected.com/command-not-found-in-bash-fixed/)
