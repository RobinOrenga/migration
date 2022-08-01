# migration
Migration AD
Pour automatiser la migration d’un serveur j’ai créé un script de migration de l’AD.
Ce script va se composer de 10 actions qui pourront être modifiées selon les besoins de
chacun.
Je vais effectuer différentes opérations :
- Réaliser l’installation de l’ADDS.
- Promouvoir en tant que contrôleur de domaine pour rejoindre l’ancien domaine.
- Vérifier les différents rôles pour qu’ils soient bien installés.
- Mettre en place la migration des rôles FSMO.
- Vérifier les FSMO.
Sur l’ancien serveur dès que la migration a été faite il faudra :
- Supprimer le rôle ADDS.
- Rétrograder l’ancien serveur.
- Augmenter le niveau fonctionnel de la forêt et du domaine au besoin.
- Vérifier que les différentes actions ont bien été réalisées à l’aide de la fonction de
LOG.
- Redémarrer l’équipement.
Pour lancer ce script il sera possible de le lancer en PowerShell, PowerShell ISE en
administrateur pour avoir le script en haut et les actions effectuées en bas.
Image 26 : Console PowerShell ISE
Il sera possible aussi de l’exécuter en « .exe » avec un logiciel qui convertit les « .ps1 » en
« .exe ». Pour ma part je mettrai le script dans le chemin C:\script\migrationad
