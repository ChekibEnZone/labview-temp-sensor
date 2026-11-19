# Temp Sensor Test — LabVIEW

Petit VI LabVIEW de test d'acquisition de température : il simule un capteur, affiche la mesure en temps réel sur un graphe déroulant et s'arrête avec un bouton STOP.

## Fonctionnement

- **Boucle While** cadencée par une temporisation (*Wait (ms)*), qui fixe la période d'échantillonnage.
- **Capteur simulé** : la fonction *Random Number (0-1)* remplace la mesure réelle, ce qui permet de tester l'IHM et la boucle sans matériel.
- **Waveform Chart** : affichage de la courbe en temps réel (amplitude en fonction du temps).
- **Bouton STOP** : arrêt propre de la boucle.

## Utilisation

1. Ouvrir `Temp_Sensor_test.vi` dans LabVIEW (fichier enregistré avec LabVIEW 26.3).
2. Lancer le VI (flèche *Run*).
3. Observer la courbe, puis cliquer sur **STOP**.

## Pistes d'évolution

- Remplacer le nombre aléatoire par une vraie acquisition (DAQmx, thermocouple ou PT100).
- Mettre la mesure à l'échelle en °C et ajouter des seuils d'alarme.
- Enregistrer les mesures dans un fichier (CSV ou TDMS).

## Auteur

Chequib Kouka — technicien bancs d'essai et instrumentation.
