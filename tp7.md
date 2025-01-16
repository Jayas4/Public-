

mettre un fichier xml dans le windows pour repondre a toutes les quesions et executer des scripts auto

<a href="https://schneegans.de/windows/unattend-generator/">Cliquez ici pour voir le site de génération </a>
=
<a href="https://github.com/Jayas4/Public-/blob/main/autounattend.xml">Fichier Xml</a>

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


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




