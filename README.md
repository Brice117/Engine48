# Tank Sounding

Application Android qui calcule le volume net (m³) des réservoirs 80 (Dirty Bilge), 50 (Oily Bilge),
24 (Sludge PS) et 94 (Sludge SB) à partir de la hauteur de sonde (cm) et de l'assiette (trim, m).

Calcul : interpolation linéaire sur le trim (colonnes −0,5 / 0 / +0,5) pour les deux lignes de cm
encadrant la sonde, puis interpolation linéaire sur le cm. Hors table, la valeur est ramenée à la borne
(0–97 cm, ±0,5 m) avec un avertissement.

- `www/index.html` : toute l'application (tables dans `TANKS`) — s'ouvre aussi directement dans un navigateur.
- `.github/workflows/android.yml` : compile l'APK sur GitHub (onglet Actions → artefact « Jaugeage-apk »).
