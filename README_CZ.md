# Robot Cockpit – automatický build APK

## 1. Nahraj projekt na GitHub

Rozbal ZIP a nahraj celý jeho obsah do nového GitHub repozitáře.
Důležité je zachovat složku:

.github/workflows/build-apk.yml

## 2. Spuštění buildu

Na GitHubu otevři:

Actions → Build APK → Run workflow

Případně se workflow spustí automaticky po pushnutí změn do hlavní větve.

## 3. Stažení APK

Po dokončení buildu otevři konkrétní běh workflow.
Dole najdi sekci Artifacts.

Stáhni:

RobotCockpit-debug-apk

ZIP rozbal a v telefonu spusť:

app-debug.apk

## Co obsahuje první testovací verze

- 2D mapu a základní odometrii
- virtuální joystick
- START/STOP/VPŘED/VZAD
- panel IMU a gyro
- enkodéry
- GPS
- LiDAR panel
- baterii
- jednoduchý editor/přehled tras

Data jsou zatím simulovaná. Bluetooth/Wi-Fi komunikaci s ESP32 doplníme v další verzi.
