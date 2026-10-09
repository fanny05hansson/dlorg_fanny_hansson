# dlorg - Downloads Organizer 📁

`dlorg` är ett smart Bash-skript skapat för att automatiskt städa upp och organisera din `Downloads`-mapp i Linux. Skriptet lyssnar i realtid efter nya filer och sorterar dem direkt i undermappar baserat på deras filändelser.

## Funktioner 🚀
Skriptet övervakar mappen och sorterar automatiskt filer till följande mappar:
* **pdfs/** – För PDF-dokument (`.pdf`)
* **images/** – För bilder (`.jpg`, `.png`, `.gif`, etc.)
* **text/** – För vanliga textfiler (`.txt`, `.md`)
* **docs/** – För textdokument (`.docx`, `.doc`)
* **videos/** – För videofiler (`.mp4`, `.mkv`) *(Extra mapp)*
* **archives/** – För komprimerade filer (`.zip`, `.tar`) *(Extra mapp)*
* **other/** – För alla andra filtyper

## Installation & Förberedelser 🛠️
För att skriptet ska fungerar på Oracle Linux behöver verktyget `inotify-tools` vara installerat via EPEL:

```bash
sudo dnf install oracle-epel-release-el10 -y
sudo dnf install inotify-tools -y
```

Se till att skriptet har körrättigheter:
```bash
chmod +x dlorg
```

## Användning 💻
Starta skriptet genom att köra följande kommando i din terminal:
```bash
./dlorg
```
Skriptet kommer nu att ligga i bakgrunden och övervaka din `~/Downloads`-mapp automatiskt!

