
<a href="https://schneegans.de/windows/unattend-generator/">Cliquez ici pour voir le site de génération </a>
=
<a href="https://github.com/Jayas4/Public-/blob/main/autounattend.xml">Cliquez ici pour voir le résultat </a>


Logs : 
```
-Langue d'installation Francais
-Disposition du clavier Francais
-Bypass WindowsRequire
-Mise a niveau du nom par script ps1
-Windows Decide compact ou non
-Windows determine la timzone
-Windows determine les partition
-Clée généric Entreprise
-Création compte elve password: 26400Crest group:Administrator
-Le mot de passe n'expire pas
-Fail windows 10 try
-Basic File Explorer
-SearchBox visible
-Icones par defaut
-Remove Widgets
-Cacher TaskView de la TaskBar
-Ne pas montrer les resultats de bing pendant les recherches
-
-Pins par défaut
-Desactiver l'UAC
-Desactiver Smart L'app Control
-Desactiver SmartScreen dans edge
-Activation Chemin Long
-Activation RDP (Remote Desktop services)
-Autorisation des scripts Powhershell
-Desactiver les sons système
-Désactiver les suggestion
-Cacher la Edge First Experiene
-Supprimer Windows.old
-Utilisation par defaut des effets visuel
-Skip Wifi Config
-Desactiver l'envoie des diagnostic
-La carte mère décide les lock keys
-Personnalisation par defaut

-Suppresion de :
3D Viewer  Bing Search  Camera  Clock  Copilot  Dev Home  Family  Feedback Hub  Get Help  Handwriting (all languages)   Internet Explorer  Mail and Calendar  Math Input Panel  Media Features  Mixed Reality  Movies & TV  News  Notepad (modern)  Office 365  OneDrive  OneNote  OneSync  OpenSSH Client  Outlook for Windows  Paint  Paint 3D  Photos  Power Automate  PowerShell 2.0  PowerShell ISE  Quick Assist  Recall  Remote Desktop Client  Skype  Snipping Tool  Solitaire Collection  Speech (all languages)   Steps Recorder  Sticky Notes  Teams  Tips  To Do  Voice Recorder  Wallet  Weather  Windows Fax and Scan  Windows Hello  Windows Media Player (classic)  Windows Media Player (modern)  Windows Terminal  WordPad  Xbox

-Après création 1 user group:Admin run en ps1 :
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

-Après la création 1 user group:Admin et exection du script ci dessus en ps1 :
# Liste des applications à installer via Chocolatey
$applications = @(
    "googlechrome",          # Google Chrome
    "firefox",               # Mozilla Firefox
    "vscode",                # Visual Studio Code
    "7zip",                  # 7-Zip
    "spotify",               # Spotify
    "adobe-acrobat-reader",  # Adobe Acrobat Reader
    "notepadplusplus",       # Notepad++
    "slack",                 # Slack
    "vlc",                   # VLC Media Player
    "git"                    # Git
)

# Fonction pour installer les applications
function Install-Applications {
    foreach ($app in $applications) {
        Write-Host "Installation de l'application: $app" -ForegroundColor Green
        try {
            # Installation de l'application via Chocolatey
            choco install $app -y --quiet
        } catch {
            Write-Host "Erreur lors de l'installation de $app: $_" -ForegroundColor Red
        }
    }
}

# Exécution de l'installation des applications
Install-Applications

Write-Host "Installation des applications terminée !" -ForegroundColor Cyan

-Pas de conf WDAC policy 

```
