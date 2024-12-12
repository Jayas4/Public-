# SOLUTION UNNIVERSEL

mettre un fichier xml dans le windows pour repondre a toutes les quesions et executer des scripts auto

<a href="https://schneegans.de/windows/unattend-generator/">Cliquez ici pour voir le site de génération </a>
=
<a href="https://github.com/Jayas4/Microsoft/blob/main/Documentation/autounattend.xml">Cliquez ici pour voir le résultat </a>

Pour un déploiement réseau il faut ouvrir l'iso puis glisser le fichier autounattend.xml avec winrar par exemple , et le mettre dans la racine de l'iso , puis de lancer votre installation 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## II. Débarassé de ce qui n'est pas utile a la main
### A. Supprimer les application et les choses inutiles
```
Tiny11 Builder n'est pas un crack de Windows,
il vous faudra donc disposer d'une licence d'utilisation du système d'exploitation pour compléter l'installation.
 Si vous avez acheté un PC complet dans le commerce, cette licence est certainement incluse avec et lié à la carte-mère
de l'ordinateur.
Dans le cas contraire, de nombreux sites de commerce en ligne propose régulièrement des clés d'activation pour Windows 11
à prix intéressant, vérifiez simplement à quelle version de Windows correspond la clé achetée (Famille, Pro, IoT, etc.).
```

Pour installer Edge
```
 winget install edge
```
Pour installer Firefox
```
winget install -e --id Mozilla.Firefox
```
Pour installer Chrome
```
winget install -e --id Google.Chrome
```

Une fois que vous avez bien ces informations en tête, voici la marche à suivre pour créer une version allégée de Windows avec Tiny11 Builder.

►Télécharger l'image ISO de Windows 11 en Français <a href="https://www.microsoft.com/en-us/software-download/windows11">Cliquez ici </a> La page propose trois méthodes différentes pour récupérer Windows 11. Descendez dans la page jusqu'à trouver l'option "Download Windows 11 Disk Image (ISO) for x64 devices", puis cliquez sur la liste déroulante Select Download et sélectionnez l'option Windows 11 (multi-edition ISO for x64 devices, puis cliquez sur le bouton bleu Download Now. Une nouvelle section intitulée "Select the product language" apparaît, cliquez sur la liste déroulante Choose one et sélectionnez French puis cliquez enfin sur le bouton bleu Confirm. Une nouvelle page apparaît, cliquez alors sur le bouton bleu 64-bit Download et choisissez un répertoire de destination pour lancer le téléchargement de l'image ISO de Windows 11.

<p align="center"> <img src="https://img-19.commentcamarche.net/vGzRlaDkfL6M_fWtHq0omXIv7cE=/1080x/smart/bb30936e61db43e18bd8ad6573ef6db0/ccmcms-commentcamarche/39491852.png" width="500" height="auto" /> </p>

►Télécharger Tiny11 Builder à partir de la page GitHub du projet : Installation : <a href="https://github.com/ntdevlabs/tiny11builder?tab=readme-ov-file">Cliquez ici </a> pour télécharger directement  Script Tiny11 
Sur la page GitHub du projet, cliquez sur le bouton vert <> Code puis sur Download ZIP. Ouvrez ensuite le répertoire dans lequel vous avez enregistrez le fichier et décompresse l'archive ZIP à l'endroit voulu, mais ne lancez pas tout de suite le script Tiny11 Builder.

<p align="center"> <img src="https://img-19.commentcamarche.net/tG7KcxPMrmXyEOvlChO7emV8grI=/1080x/smart/beba76b5e7bd4300849ecfaf4e6d2652/ccmcms-commentcamarche/39491853.png" width="500" height="auto" /> </p>

► Autorisez l'exécution de scripts PowerShell provenant de sources externes : ouvrez le menu Démarrer, tapez "powershell" dans la barre de recherche puis, sur le résultat WIndows PowerShell cliquez sur Exécuter en tant qu'administrateur.

<p align="center"> <img src="https://img-19.commentcamarche.net/lesWp2uoLZBkv_7_7qEjM6aBhKc=/1080x/smart/dd4883642f354ee39c8cac0fa3b8bee3/ccmcms-commentcamarche/39491854.png" width="500" height="auto" /> </p>

► Dans la fenêtre de PowerShell, tapez la commande suivante : Set-ExecutionPolicy unrestricted et validez en appuyant sur Entrée, puis tapez la lettre O et validez à nouveau en appuyant sur Entrée.

<p align="center"> <img src="https://img-19.commentcamarche.net/qUWLrosfYaujXA7NfzePQSvxRDE=/600x/smart/35d1a8c089be4dc39904ca363d4ea47b/ccmcms-commentcamarche/39491855.png" width="500" height="auto" /> </p>

► Montez le volume de l'image ISO de Windows 11 : dans l'Explorateur de fichiers, ouvrez le répertoire dans lequel vous avez enregistré l'image ISO de Windows 11, double-cliquez dessus et validez le message de confirmation qui apparaît. Cela aura pour effet de "monter" cette image disque comme un périphérique sur votre ordinateur et vous le verrez apparaître comme un lecteur de DVD dans l'arborescence de l'Explorateur de Fichiers. Notez bien la lettre qui se trouve entre parenthèses dans le nom du lecteur (sur la capture d'écran ci-dessous, c'est la lettre D).

<p align="center"> <img src="https://img-19.commentcamarche.net/Kt272I6_S0aVRh0y0Xx1B36jNec=/600x/smart/0343657614c840869f79f87189758eff/ccmcms-commentcamarche/39491856.png" width="500" height="auto" /> </p>

► Lancez Tiny11 Builder : dans l'Explorateur de fichiers, ouvrez le répertoire dans lequel vous avez décompressé l'archive ZIP de Tiny11 Builder, faîtes un clic-droit sur le fichier tiny11maker.ps1 puis cliquez sur Exécuter avec PowerShell. Deux messages d'avertissement successifs vont s'afficher dans PowerShell, validez les en tapant chaque fois la lettre O puis en appuyant sur Entrée.

<p align="center"> <img src="https://img-19.commentcamarche.net/jrk8SkUREqE_eZmQlsRtsDnS2kk=/600x/smart/759d76d0d099497e91bfe50d525e7406/ccmcms-commentcamarche/39491857.png" width="500" height="auto" /> </p>

► Sélectionnez l'image de Windows 11 : une fois le script Tiny11 Builder lancé dans PowerShell, indiquez la lettre du lecteur contenant l'image officielle de Windows 11 que vous avez noté précédemment (dans notre exemple, il s'agit de la lettre D) et validez en appuyant sur Entrée.

<p align="center"> <img src="https://img-19.commentcamarche.net/gAUJGl92vhZyzSIUHCDD_vpLenI=/600x/smart/bce96ddea9de40818a0d6d515402568e/ccmcms-commentcamarche/39491858.png" width="500" height="auto" /> </p>

► Sélectionnez la version de Windows 11 à alléger : une liste des différentes versions de Windows 11 disponible va apparaître dans la fenêtre de PowerShell. Chacune est identifiée par un index sur la première ligne. Pour sélectionnez la version de Windows 11 que vous souhaitez alléger, tapez le numéro de son index et validez en appuyant sur Entrée. Par exemple, la version Windows 11 Famille (la plus courante sur les ordinateurs grand public) porte le numéro 1.

<p align="center"> <img src="https://img-19.commentcamarche.net/ud-TcV0PhpD_D14bR6VRQug6Qg4=/600x/smart/d7e389e698c64d30a3670d1f63a62288/ccmcms-commentcamarche/39491859.png" width="500" height="auto" /> </p>

► Attendre la fin du processus : le script Tiny11 Builder va ensuite procéder à la création d'une image allégée de la version de Windows 11 que vous avez sélectionné. Le processus peut prendre quelques minutes, durant lesquelles vous verrez défiler tout un tas de lignes de différentes couleurs dans la fenêtre de PowerShell. Patienter jusqu'à la fin du processus, qui sera signalé par le message "Done. Creation completed! Press any key to exit the script..." et appuyer ensuite sur n'importe quelle touche pour fermer la fenêtre PowerShell.

<p align="center"> <img src="https://img-19.commentcamarche.net/1xd186nei_MCGGlo3mBV2A2qngA=/600x/smart/0a11079a4f364e49afc625f2d50eb17b/ccmcms-commentcamarche/39491860.png" width="500" height="auto" /> </p>

► Créer une clé USB Bootable de l'image allégée de Windows 11 : retournez dans le répertoire à partir duquel vous avez lancer le script Tiny11 Builder, vous y trouverez un nouveau fichier nommé "tiny11.iso". Il s'agit du fichier d'installation de la version allégée de Windows 11 que vous venez de créer. Pour l'utiliser et l'installer sur un ordinateur de votre choix, vous devez le copier sur une clé USB Bootable, en utilisant par l'exemple l'outil gratuit Rufus, dont nous vous présentons le fonctionnement dans cette fiche de téléchargement.

<p align="center"> <img src="https://img-19.commentcamarche.net/4WNawv0BNjrYtvuPZ-TNYIHSvvo=/600x/smart/7f59cceab9ed452c8f31c7c6c4a26629/ccmcms-commentcamarche/39491861.png" width="500" height="auto" /> </p>

Vous pouvez lancer le script Tiny11 Builder autant de fois que nécessaire, par exemple pour créer différentes images allégées de différentes versions de Windows 11 selon vos besoins. Pensez simplement à renommer le fichier "tiny11.iso" et à la déplacer à un autre emplacement après sa création, carTiny11 Builder remplacera ce fichier à chaque nouveau lancement du script. Une fois la clé USB Bootable créée, vous pourrez la conserver à porter de main pour installer cette version de Windows 11 personnalisée à chaque fois que vous en autre besoin. Notez que, s'agissant d'une modification non officielle de l'OS, il se peut que les futures mises à jour de Windows ne s'installent pas correctement sur cette version modifiée. Consultez régulièrement la page GitHub de Tiny11 Builder pour vous tenir informé des problèmes connus et des évolutions du projet.

## III. Installation des logiciels de travail 


Installer WinGet: 
```
Add-AppxPackage -RegisterByFamilyName -MainPackage Microsoft.DesktopAppInstaller_8wekyb3d8bbwe
```

Applications
```

winget install -e --id WiresharkFoundation.Wireshark
winget install -e --id Python.Python.3.11
winget install -e --id WinSCP.WinSCP
winget install -e --id RARLab.WinRAR
winget install -e --id Adobe.Acrobat.Reader.64-bit
winget install -e --id ArduinoSA.IDE.stable
winget install -e --id RaspberryPiFoundation.RaspberryPiImager
winget install -e --id dotPDNLLC.paintdotnet
winget install -e --id PuTTY.PuTTY
winget install -e --id MyPaint.MyPaint
winget install -e --id Lenovo.SystemUpdate
winget install -e --id Google.Chrome
winget install -e --id Mozilla.Firefox
winget install -e --id Microsoft.OfficeDeploymentTool
winget install -e --id VMware.WorkstationPro
```


Pense bête :
$macToNameMap = @{
    "00-14-22-01-23-45" = "PC-01"
    "00-14-22-56-78-90" = "PC-02"

    "00-14-22-AB-CD-EF" = "PC-03"
    "00-1A-2B-3C-4D-5E" = "PC-04"
	"00-14-22-01-23-45" = "PC-05"
    "00-14-22-56-78-90" = "PC-06"
    "00-14-22-AB-CD-EF" = "PC-07"
    "00-1A-2B-3C-4D-5E" = "PC-08"
	"00-14-22-01-23-45" = "PC-09"
    "00-14-22-56-78-90" = "PC-10"
    "00-14-22-56-78-90" = "PC-11"
    "00-14-22-56-78-90" = "PC-12"
    "00-14-22-56-78-90" = "PC-13"
    "00-14-22-56-78-90" = "PC-14"
	"00-14-22-56-78-90" = "PC-15"
    "00-14-22-56-78-90" = "PC-16"
}

$macAddress = (Get-NetAdapter | Select-Object -First 1 -ExpandProperty MacAddress).ToUpper()

if ($macToNameMap.ContainsKey($macAddress)) {
    $newName = $macToNameMap[$macAddress]
} else {
    $newName = "PC-ERREUR"
}

$newName

winget install -e --id WiresharkFoundation.Wireshark
winget install -e --id Python.Python.3.11
winget install -e --id WinSCP.WinSCP
winget install -e --id RARLab.WinRAR
winget install -e --id Adobe.Acrobat.Reader.64-bit
winget install -e --id ArduinoSA.IDE.stable
winget install -e --id RaspberryPiFoundation.RaspberryPiImager
winget install -e --id dotPDNLLC.paintdotnet
winget install -e --id PuTTY.PuTTY
winget install -e --id MyPaint.MyPaint
winget install -e --id Lenovo.SystemUpdate
winget install -e --id Google.Chrome
winget install -e --id Mozilla.Firefox
winget install -e --id Microsoft.OfficeDeploymentTool
winget install -e --id VMware.WorkstationPro




