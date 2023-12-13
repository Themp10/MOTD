
### Running
Cloner le dossier :
```shell
git clone https://github.com/themp10/MOTD.git
```

Acceder au dossier
```shell
cd MOTD/
```

Installer les packages necessaires

```shell
sudo apt-get install figlet curl bc fortune lm-sensors
```


Desactiver le MOTD Ubuntu par défaut:

```shell
sudo chmod -R -x /etc/update-motd.d/
sudo chmod -x /usr/share/landscape/landscape-sysinfo.wrapper
```

Donner les droits d'execution à `motd.sh`
```shell
sudo chmod +x motd.sh
sudo chmod +x framework.sh
sudo chmod -R +x modules/
```
OR 
```shell
cd
sudo chmod -R +x MOTD/
```

### Executer au login


Pour executer le MOTD au login 
ajouter cette ligne dans `.profile`

```shell
~/MOTD/motd.sh
```
