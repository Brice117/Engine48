# Engine48

Outil d'aide pour l'officier mécanicien (application Android).

**Sounding** : volume net (m³) des réservoirs 80 (Dirty Bilge), 50 (Oily Bilge), 24 (Sludge PS) et 94 (Sludge SB)
à partir de la sonde (cm) et de l'assiette (trim, m). Interpolation linéaire sur le trim (colonnes −0,5 / 0 / +0,5)
pour les deux lignes de cm encadrant la sonde, puis sur le cm. Hors table, la valeur est ramenée à la borne
(0–97 cm, ±0,5 m) avec un avertissement. Total et partage du relevé.

**Items** : liste de matériel (Material ID, Description, Position), recherche, modification, export CSV.
Les données restent sur le téléphone (exporter régulièrement pour en garder une copie).

- `www/index.html` : toute l'application (tables de jaugeage dans `TANKS`).
- `.github/workflows/android.yml` : compile l'APK sur GitHub (onglet Actions → artefact « Engine48-apk »).
