
A MORE ADVANCED SCRIPT IS AVAILABLE (IT INCLUDES BUNGEECORD) : https://github.com/LaBaaSe/Mcinstall
# French Version

# Script d'installation automatique de serveur minecraft
Ce script permet d'installer automatiquement un serveur minecraft sur un VPS linux. Le script installe automatiquement l'environnement Java 8 requis pour le bon fonctionnement du serveur. 

# Versions supportées 
Spigot  1.9.4, 1.8.8, 1.11.2, 1.12.2 et 1.10.2

# Téléchargement
Avant de télécharger le script vous avez besoin d'installer curl :
En root :
```bash
apt-get install curl
```

Si vous n'êtes pas root : 
```bash
sudo apt-get install curl
```

Maintenant vous pouvez procéder à l'installation 
En root : 
```bash
curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall

```

Si vous n'êtes pas en root : 
```bash
sudo curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
```

Si vous avez un problème lors du téléchargement référez vous à la section "Résolution de problèmes"

# Utilisation
Exécutez la commande suivante.
(Si vous êtes connecté avec root ) 
```bash
minecraftinstall
```

(Si vous n'êtes pas connecté avec root )

```bash
sudo minecraftinstall
```

# DEBUG/VERBOSE

Si vous souhaitez voir toutes les logs pendant l'excécution du programme exécutez la commande suivante :
(Si vous êtes connecté avec root ) 
```bash
minecraftinstall -verbose
```
(Si vous n'êtes pas connecté avec root )

```bash
sudo minecraftinstall -verbose
```
# Update

Le script dispose de son propre système de mise à jour. Tous les sois à minuit, il vérifie les mises à jour, en téléchargeant un fichier de moins de 20 ko qui sera dans le dossier /tmp (temporaire)
Lors du lancement du script, le script va automatiquement vérifier si des mises à jours sont disponibles via le fichier qui a été téléchargé auparavant automatiquement.
Il supprimera donc le fichier temporaire et appliquera la mise à jour.
Comment mettre à jour le script SEULEMENT si vous n'avez pas la dernière version avec l'auto-updater :
Tapez cette commande (root)
``` bash
rm /usr/bin/minecraftinstall && wget -P /usr/bin https://uploads.laabase.ovh/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall 
```

Tapez cette commande (no-root)
```bash
sudo rm /usr/bin/minecraftinstall && sudo wget -P /usr/bin https://uploads.laabase.ovh/minecraftinstall && sudo chmod 0777 /usr/bin/minecraftinstall
```


# Résolution de problèmes :

Si vous avez une erreur du type  
```bash
Erreur : le certificat de « uploads.laabase.ovh » n'est pas de confiance.
Erreur : le certificat de « uploads.laabase.ovh » n'est pas d'un émetteur connu.
``` 
Réalisez la commande suivante (root): 
or : 
```bash
apt-get install ca-certificates
``` 

```bash
curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall``` 

Si vous n'êtes pas root : 
```bash
sudo apt-get install ca-certificates
``` 

```bash
 sudo curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
 ``` 

# English Version (With english script)

# Auto-Install Minecraft server Script
This script automatically installs a minecraft server on a linux VPS. The script automatically installs the java 8 environment required for the proper functioning of the server.

# Supported Minecraft Versions : 

Spigot  1.9.4, 1.8.8, 1.11.2, 1.12.2 and 1.10.2

# Download

Before install the script you need to install curl 
As root :
```bash
apt-get install curl
```

If you are not root :
```bash
sudo apt-get install curl
```
Then you can install the script : 
If you are root : 
```bash
curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
```

If you are not root : 

```bash
sudo curl https://uploads.laabase.ovh/download.php?file=minecraftinstall --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
```

# Use the script : 

if you are root
```bash
minecraftinstall
```

If you are not root : 

```bash
sudo minecraftinstall
``` 

# DEBUG/VERBOSE

If you want to see all the logs while running the program run the following command:
(If you are logged in with root)

```bash
minecraftinstall -verbose
```
(If you are not logged in with root)

```bash
sudo minecraftinstall -verbose
```
# Update

The script has its own update system. All at midnight, check for updates by uploading a file of less than 20 KB that will be in the / tmp (temporary) folder
When launching the script, the script will automatically check if updates are available via the file that was previously downloaded automatically.
It will delete the temporary file and apply the update.

HOW TO UPDATE ONLY IF YOU DO NOT HAVE THE VERSION WITH THE AUTO-UPDATER
Type this command (root)
``` bash
rm /usr/bin/minecraftinstall && wget -P /usr/bin https://uploads.laabase.ovh/en/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall 
```

Type this command (no-root)
```bash
sudo rm /usr/bin/minecraftinstall && sudo wget -P /usr/bin https://uploads.laabase.ovh/en/minecraftinstall && sudo chmod 0777 /usr/bin/minecraftinstall
```
# Problem solving

If you have an error of the type
```bash
Error: the certificate of "uploads.laabase.ovh" is not trusted.
Error: The certificate of "uploads.laabase.ovh" is not from a known issuer.
```
Make the following commands (root):
```bash
 apt-get install ca-certificates
``` 
```bash
curl https://uploads.laabase.ovh/download.php?file=minecraftinstall_en --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
``` 
If you are not root : 
```bash
sudo apt-get install ca-certificates
``` 

```bash
sudo curl https://uploads.laabase.ovh/download.php?file=minecraftinstall_en --output /usr/bin/minecraftinstall && chmod 0777 /usr/bin/minecraftinstall
```
# Support

If you got any trouble you can contact me at : adam@laabase.ovh
