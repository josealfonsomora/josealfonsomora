# Jose Alfonso Mora
### Android Tech Lead at [Zego](https://www.zego.com/)

### Git Alias

#### Log

```
git config --global alias.lg "log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
```

#### Squash

```
git config --global alias.squash '!f(){ git reset --soft HEAD~${1} && git commit --edit -m"$(git log --format=%B --reverse HEAD..HEAD@{1})";};f'
```

### ADB commands

#### Launch Android link
```
adb shell am start -d url
```

#### View running activities
```
adb shell "dumpsys activity activities | grep mResumedActivity"
```

### Tools

[iTerm2 + zsh + oh-my-zsh](https://medium.com/ayuth/iterm2-zsh-oh-my-zsh-the-most-power-full-of-terminal-on-macos-bdb2823fb04c)

[Charles Proxy](https://www.charlesproxy.com/)

[Proxy Toggle](https://github.com/theappbusiness/android-proxy-toggle)

[USB Android device mirror](https://github.com/Genymobile/scrcpy)

[Adb wifi](https://developer.android.com/studio/command-line/adb#wireless)

```
adb tcpip 5555
adb shell "ip addr show wlan0 | grep -e wlan0$ | cut -d\" \" -f 6 | cut -d/ -f 1"  // to obtain the phone's IP address
adb connect <Android_device_id>:5555
adb connect <ip_address>:5555
```

[Jetbrains Toolbox](https://www.jetbrains.com/toolbox-app/)
