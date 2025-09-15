# Faugus Launcher
A simple and lightweight app for running Windows games using [UMU-Launcher](https://github.com/Open-Wine-Components/umu-launcher)

### Support the project
<a href='https://ko-fi.com/K3K210EMDU' target='_blank'><img src=https://github.com/Faugus/faugus-launcher/blob/main/assets/ko-fi.png width="155" height="35"/></a>&nbsp;&nbsp;
<a href='https://www.paypal.com/donate/?business=57PP9DVD3VWAN&no_recurring=0&currency_code=USD' target='_blank'><img src=https://github.com/Faugus/faugus-launcher/blob/main/assets/paypal.png width="155" height="35"/></a>

## Installation
```
flatpak install flathub io.github.Faugus.faugus-launcher
```

## Running
```
flatpak run io.github.Faugus.faugus-launcher
```

## Steam Flatpak integration
Allow Faugus Launcher to detect Steam users:
```
sudo flatpak override io.github.Faugus.faugus-launcher --filesystem=~/.var/app/com.valvesoftware.Steam/.steam/steam/userdata/
```
Allow Steam to run Faugus Launcher's shortcuts:
```
sudo flatpak override com.valvesoftware.Steam --talk-name=org.freedesktop.Flatpak
```
Allow Steam to see the game's icon:
```
sudo flatpak override com.valvesoftware.Steam --filesystem=~/.var/app/io.github.Faugus.faugus-launcher/config/faugus-launcher/
```
### Known issues:
- The 'stop' button won't close games/apps
- Gamescope doesn't work
- It may not use the system theme in some DEs
