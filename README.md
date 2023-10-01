# RL Distortion Audio

Ein Projekt, das Q-Learning verwendet, um Audioverzerrungsparameter zu optimieren.

## Überblick

Dieses Projekt verwendet ein Q-Learning-Agenten, um die besten Parameter für einen Audioverzerrer zu finden. Das Ziel ist es, ein Eingangssignal so zu verzerren, dass es einem Ziel-Audiosignal so ähnlich wie möglich ist.

## Struktur

Das Projekt besteht aus mehreren Hauptkomponenten:

- **DistortionParameters**: Eine Klasse, die die Verzerrungsparameter (Gain, Tone, Level) speichert und verwaltet.
  
- **DistortionEnvironment**: Eine Klasse, die ein Eingangssignal generiert, es mit den gegebenen Verzerrungsparametern verarbeitet und das verarbeitete Signal zurückgibt.
  
- **QLearningAgent**: Ein Q-Learning-Agent, der lernt, die besten Verzerrungsparameter zu wählen, um das Eingangssignal dem Ziel-Audiosignal anzunähern.

## Verwendung

1. Initialisieren Sie die `DistortionParameters` mit zufälligen Werten.
2. Erstellen Sie eine Instanz von `DistortionEnvironment` mit den initialisierten Parametern.
3. Initialisieren Sie den `QLearningAgent`.
4. Trainieren Sie den Agenten, indem Sie ihn Aktionen auswählen lassen, die Belohnung berechnen und den Q-Wert aktualisieren.
5. Überprüfen und analysieren Sie die Ergebnisse.

## Abhängigkeiten

- numpy
- scipy
- matplotlib

## Lizenz

[MIT](LICENSE)
