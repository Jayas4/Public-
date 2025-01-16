

mettre un fichier xml dans le windows pour repondre a toutes les quesions et executer des scripts auto

<a href="https://schneegans.de/windows/unattend-generator/">Cliquez ici pour voir le site de génération </a>
=
<a href="https://github.com/Jayas4/Public-/blob/main/autounattend.xml">Fichier Xml</a>

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




