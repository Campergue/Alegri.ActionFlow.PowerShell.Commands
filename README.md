# Alegri.Powershell.ActionFlowTool

## Kurz Beschreibung

Ein Aktion Flow Tool für Powershell das es ermöglicht mit einer XML Datei verschiedene Aktionen auszuführen. Diese Tool stellt jedoch rein die generalisierte Funktion des Aktion Flow dar. Die eigentlichen Funktionen werden durch sogenannte Aktionspakete zur Verfügung gestellt. Diese Pakete müssen im Aktionspaket Manager eingetragen werden.

Dieses Tool kennt zwei Aktionstypen [manuell, automatisch].

Bei einer manuelle Aktion wird die Beschreibung als Hinweis auf der Konsole ausgegeben und es wird auf eine Bestätigung des Users erwartet. Entsprechend der Eingabe des User wird das Skript beendet bzw. weitergeführt.

Das Tool stehl eine Globale Funktion Create-QuestionTask zur Verfügung, die es dem Entwickler einer Aktion ermöglicht, ebenfalls eine manuelle Interaktion des Users einzubauen.

Ein Beispiel für eine Aktionspaket finden Sie in einem [seperaten Projekt](https://github.com/Campergue/Alegri.ActionPack.Template.Powershell.Commands).

## Einfachste Form der Verwendung
1. Laden Sie das Projekt auf Ihren Lokalen Rechner
2. Erstellen / Fügen Sie das Modul dem Lokalen Profile der PowerShell Umgebung zu
  1. In der Regel finden Sie unter C:\User\[IhrUserName]\Documents einen WindowsPowerShell Ordner. Wenn nicht erstellen Sie den Ordner
  2. Innerhalb des Ordner befinden sich zwei Dateien für die UserProfile Einstellungen für die PowerShell
  ![image](https://cloud.githubusercontent.com/assets/6292190/21509854/afcb1abe-cc8d-11e6-8e49-858602bf1a14.png)
    1. Die ProfilDatei für die PowerShell Klassic. Sollte die Datei bei Ihnen nicht vorhanden sein, können Sie diese Datei selbst erstellen
    2. Die ProfilDatei für die PowerShell ISE. Sollte die Datei bei Ihnen nicht vorhanden sein, können Sie diese Datei selbst erstellen.
  3. Importieren Sie die .psm1 Datei des Moduls in die jeweilige Profil Datei. Ersetzen Sie den Pfad mit dem Pfad auf Ihren Rechner zu dem Projekt.
![image](https://cloud.githubusercontent.com/assets/6292190/21509915/46157d98-cc8e-11e6-9226-9babc9232767.png)
  
## Einbinden eines Aktionspaket
![image](https://cloud.githubusercontent.com/assets/6292190/21509729/24ecc7cc-cc8c-11e6-9194-3b1c02bb8c0d.png)
  1. Sie prüfen als erstes ob die Aktion in dem Aktionspaket enthalten ist. Wenn ja rufen Sie die Start Funktion auf um die Aktion auszuführen.

Sie müssen das Paket wie das ActionFlowTool Modul einbinden.

---
##Short Description

An action flow tool for Powershell that allows you to perform various actions with an XML file. However, this tool is merely the generalized function of the action flow. The actual functions are provided by so-called action packages. These packages must be entered in the Action Pack Manager.

This tool has two types of actions [manual, automatic].

In the case of a manual action, the description is displayed as a note on the console and a confirmation of the user is expected. According to the user's input, the script is terminated or redirected.

The tool provides a global function Create-QuestionTask, which allows the developer of an action to also incorporate a manual interaction of the user.

An example of an action package can be found in a [seperate project](https://github.com/Campergue/Alegri.ActionPack.Template.Powershell.Commands).

## The simplest form of use
1. Download the project to your local computer
2. Create / Add the module to the Local Profile of the PowerShell environment
  1. Typically, you will find a WindowsPowerShell folder under C: \ User \ [yourUserName] \ Documents. If not, create the folder
  2. Inside the folder are two files for the UserProfile settings for the PowerShell
  ! [Image] (https://cloud.githubusercontent.com/assets/6292190/21509854/afcb1abe-cc8d-11e6-8e49-858602bf1a14.png)
    1. The profile file for the PowerShell Classic. If the file does not exist, you can create it yourself
    2. The profile file for the PowerShell ISE. If the file does not exist, you can create it yourself.
  3. Import the .psm1 file of the module into the respective profile file. Replace the path with the path to your computer to the project.
! [Image] (https://cloud.githubusercontent.com/assets/6292190/21509915/46157d98-cc8e-11e6-9226-9babc9232767.png)
  
## Integrating an action package
! [Image] (https://cloud.githubusercontent.com/assets/6292190/21509729/24ecc7cc-cc8c-11e6-9194-3b1c02bb8c0d.png)
  1. You first check whether the action is contained in the action package. If so, call the startup function to perform the action.

You must include the package as the ActionFlowTool module.
