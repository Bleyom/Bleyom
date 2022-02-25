<h1 align="center">Hi 👋, I'm Bleyom</h1>
<h3 align="center">Linux Enthusiast and Open Source developer</h3>

- 🌱 I’m currently learning **bash**
![](https://i.imgur.com/qHBpZi5.png)
![](https://i.imgur.com/ajjpQOZ.png)
```bash
#!/bin/bash
# Define Colors
blue='\033[0;34m'
orange='\033[0;32m'
pinky='\033[0;35m'
end='\033[0;00m'
# Define variables
init=$(cat /proc/1/comm)
os=$(grep -m1 "NAME=" </etc/os-release | cut -d '"' -f 2)
display=$(echo "$XDG_SESSION_TYPE")
skills=("bash," "linux," "git")
bar=$(ps -e | grep -m 1 -o \
    -e " i3bar$" \
    -e " dzen2$" \
    -e " tint2$" \
    -e " xmobar$" \
    -e " swaybar$" \
    -e " polybar$" \
    -e " lemonbar$" \
    -e " taffybar$"  \
    -e " waybar$" \
| tr -d " ")
term=$(ps -e | grep -m 1 -o \
    -e " alacritty$" \
    -e " gnome-terminal$" \
    -e " kitty$" \
    -e " xterm$" \
    -e " u*rxvt[dc]*$" \
    -e " [a-z0-9-]*terminal$" \
    -e " cool-retro-term$" \
    -e " konsole$" \
    -e " termite$" \
    -e " tilix$" \
    -e " sakura$" \
    -e " terminator$" \
    -e " termonad$" \
    -e " x*st$" \
    -e " tilda$" \
    -e " wezterm-gui$"\
| tr -d " ")
wm=$(wmctrl -m | sed '2,4d' | cut -c7-)


echo "My skill's are: ${skills[*]}"

if [[ $init == "runit" ]]; then
    echo -ne "using ${orange}runit${end} like init \n"
    elif [[ $init == "systemd" ]]; then
    echo -ne "usint ${orange}systemd${end} like init \n"
    elif [[ $init == "openrc" ]]; then
    echo -ne "using ${orange}openrc${end} like init \n"
fi

echo -ne "OS used is $os\n"
echo -ne "Display protocol used is ${display}\n"
echo -ne "Status bar used is ${bar}\n"
echo -ne "Term used is ${pinky}${term}${end}\n"
echo -ne "Window manager used is ${blue}${wm}${end}\n"


```

### Ciao 👋
![](https://i.imgur.com/qnVh20t.jpg)
  
  
