# Project Title
This is a bash shell script that can give a multiplexing experience similar to that of the Windows tool "SuperPutty"

### Installing
This is a shell script so you can git clone to pull it down, or simply download just the DuperPutty.sh script.  This is a Linux only script.  It could work on MacOS or on Windows with WSL but I have not tried, or have the desire to.

### Prerequisites
- This requires TMUX and Byobu be installed.
- The reason for byobu is its simplified key bindings and general nicer ease of use (in my opinion).

Example:
```
./DupperPutty.sh <session_name> <username> 'HOST1 HOST2 HOST3'
```
![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif1.gif)

Switching Tabs can be done using F4:

![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif2.gif)


## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments
* This is based off the work done by linuxpixie
* http://linuxpixies.blogspot.jp/2011/06/tmux-copy-mode-and-how-to-control.html
