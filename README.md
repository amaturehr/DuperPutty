### DuperPutty>_ 
![proj_icon](https://www.shareicon.net/download/48x48/2016/07/15/618380_command_320x320.png)

This is a bash shell script that can give a multiplexing experience similar to that of the Windows tool "SuperPutty".  This could be useful if you need to ssh to many hosts at once.  You do not need to maintain a hostlist file, you can easily paste in a list of hosts for more ad hoc type scenarios. 

While tmux/byobu by themselves provide great multiplexing, this was helpful for me to be able to easily ssh to many hosts and send commands to all.  This is no replacement for tools like ansible (which allows you to pretty easily issue command across many hosts), or tools like clusterssh and other cluster tools, but it may just fit the in-between scenarios of ad hoc multiplexing.

### Installing
This is a shell script so no need to install, simply download just the DuperPutty.sh script.  However for a more "integrated" experience, you could grab it doing the following:

Using CURL:
```
sudo curl -L https://github.com/amaturehr/DuperPutty/raw/master/DuperPutty.sh -o /usr/local/bin/DuperPutty
sudo chmod a+rx /usr/local/bin/DuperPutty
```
Using WGET:

```
sudo wget https://github.com/amaturehr/DuperPutty/raw/master/DuperPutty.sh -O  /usr/local/bin/DuperPutty
sudo chmod a+rx /usr/local/bin/DuperPutty
```
Please don't blindly run the above, only do so if the idea of this script sounds useful and you would like it easily available in your path as a "standard" command.

This is a Linux only script.  It could work on MacOS or on Windows with WSL but I have not tried, or have the desire to.

### Prerequisites
- This requires TMUX and Byobu be installed.  Typically installing byobu pulls in tmux as a dependency 

```
sudo apt install byobu
```

- The reason for byobu is its simplified key bindings and general nicer ease of use (in my opinion).

### Example:

```
./DupperPutty.sh <session_name> <username> 'HOST1 HOST2 HOST3'
```
![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif1.gif)

Switching Tabs can be done using F3/F4 keys. F4 to go forward, F3 to go back:

![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif2.gif)

Sending commands to all panes done using CTL+F9:

![Syntax Example](https://github.com/amaturehr/DuperPutty/blob/master/.gifs/gif3.gif)


## License
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/amaturehr/DuperPutty/blob/master/LICENSE) file for details

## Acknowledgments
* This is based off the work done by linuxpixie: http://linuxpixies.blogspot.jp/2011/06/tmux-copy-mode-and-how-to-control.html
* Thanks for the existance of tmux and byobu as well amazing tools
