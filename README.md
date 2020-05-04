# timer script
Lightweight timer with always-on-top window and sound at the end of countdown

### Preferences

* [tkinter](https://docs.python.org/3/library/tkinter.html?highlight=tkinter#module-tkinter) has to be installed: `apt-get install python-tk`

### Usage

* download timer file or copy it's content to your computer 
* move timer file into one of your PATH destinations, for example `~/.local/bin`. You can check PATH by `echo $PATH` in terminal
* make timer file executable: `chmod +x timer`
* create or copy file named `sound.mp3` into the same location

### Run the timer script

Type in bash terminal `timer` to run program.  
You can use the next markers: 
* `xh` where `x` is integer hours
* `ym` where `y` is integer minutes (can be more than 60, for example 90m to set the timer for an hour and a half)
* `zs` where `z` is integer seconds (also can be more than a minute)
    >Indeed you can call the timer with any combination of theese flags:  
     `timer 1h 1h` will set the timer for 2 hours  
     `timer 15m 90s` will set the timer for 16.5 minutes  
     `timer 300s` will set the timer for 5 minutes  
     It also can be in any order: `timer 15s 20m 1h` will work
* markers without letters with any of masks `h m s`, `m s`, `m`.
    >It means that if you type three numbers, the first of it will be recognized as hours, the second - as minutes, the third will become seconds  
    If there is only two numbers, the script understands it as minutes and seconds.   
    One number will set only minutes  
* no markers (manual setting)
    >Type `timer` and press Enter to run the program, then double click on number you want to set up, input number and press enter to run countdown

To run the countdown press Enter. After it will have finished, the `sound.mp3` plays, window destroys and program exits.                                                                    

