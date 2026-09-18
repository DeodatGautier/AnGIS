# AnGIS

**Ecological and genetic monitoring of mosquitoes with geographic information tools.**

Manage collection sites, environmental observations, individual mosquitoes and genotypes; explore them on an interactive map and run genotype statistics.

This repository provides application downloads and documentation. Application source code is not published.

[**Download the latest Windows release**](https://github.com/DeodatGautier/AnGIS/releases/latest) · [Report a problem](https://github.com/DeodatGautier/AnGIS/issues)

## Download and install

1. Open the latest release and expand **Assets**.
2. Download `AnGIS-Setup-0.5.0-x64.exe`.
3. Run the installer and launch **AnGIS** from the Start menu.

Windows 10/11, x64. Python is not required. Installation is per user, without administrator rights. The installer and application support English and Russian. A desktop shortcut is optional.

GitHub’s automatically generated “Source code” archives contain this repository’s documentation, not the application installer.

## Features

- Interactive map with multiple base layers and collection-site markers.
- World Ecosystems overlay and legend.
- Bundled climate layers for temperature and precipitation.
- Collection-site records, individual mosquito data, genotypes and attached images.
- Environmental and genetic filtering.
- Genotype frequencies and chi-square statistical analysis.
- CSV/Excel import and Excel, CSV and JSON export.
- Asynchronous retrieval of environmental information.

Online base maps and external environmental services require an internet connection. Bundled climate tiles are served locally by the application. Availability of external services may vary.

## Quick start

1. Launch AnGIS and choose your preferred language in Settings.
2. Add a collection site or import your tabular data.
3. Open a site to enter environmental observations and individual/genotype records.
4. Choose map layers and marker coloring, and filter the records of interest.
5. Open statistical analysis and export your results when ready.

A new installation starts with an empty database. For Excel import, use a `Sites` sheet and an optional `Individuals` sheet. Site records require `expedition_name`, `latitude`, `longitude`, `date` and `region`. Back up your data before bulk updates.

## Data and updates

User data is stored in `%LOCALAPPDATA%\AnoGIS`; this legacy folder name is retained for compatibility. Installation files are stored separately in `%LOCALAPPDATA%\Programs\AnGIS`.

User databases and settings are preserved on uninstall. Close AnGIS before installing an update. Back up the user-data directory and any separately stored attached images before moving to another computer.

## Verify a download

Download the matching `.exe.sha256` asset and compare it with:

```powershell
Get-FileHash -Algorithm SHA256 .\AnGIS-Setup-0.5.0-x64.exe
```

A matching checksum confirms file integrity; it is not a digital signature.

## Authors

Alexander Kurilov · Anton Moskaev

Developed for the Federal State University of Education.

## Reporting problems

Open an issue with the AnGIS version, Windows version, reproduction steps and expected/actual behavior. Include a small anonymized example or screenshot when useful; remove private data and sensitive collection-site coordinates.
