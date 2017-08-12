# DuperPutty
This is a bash shell script that can give a multiplexing experience similar to that of the Windows tool "SuperPutty".  This could be useful if you need to ssh to many hosts at once.  You do not need to maintain a hostlist file, you can easily paste in a list of hosts for more ad hoc type scenarios.

### Installing
This is a shell script so you can git clone to pull it down, or simply download just the DuperPutty.sh script.  This is a Linux only script.  It could work on MacOS or on Windows with WSL but I have not tried, or have the desire to.

### Prerequisites
- This requires TMUX and Byobu be installed.
- The reason for byobu is its simplified key bindings and general nicer ease of use (in my opinion).

### Example:

```
./DupperPutty.sh <session_name> <username> 'HOST1 HOST2 HOST3'
```
![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif1.gif)

Switching Tabs can be done using F4:

![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif2.gif)

Sending commands to all panes done using CTL+F9:

![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif3.gif)


## License
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/amaturehr/DuperPutty/blob/master/LICENSE) file for details

## Acknowledgments
* This is based off the work done by linuxpixie
* http://linuxpixies.blogspot.jp/2011/06/tmux-copy-mode-and-how-to-control.html
* Thanks for the existance of tmux and byobu as well amazing tools
