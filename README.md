# Jose Alfonso Mora

### Remote Senior Android Engineer

### Tools that I use:

#### Git Alias

```
lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
```

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
