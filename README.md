# XAI Methods: GradCAM and Similarity Explanation

## Kurzbeschreibung
Dieses Projekt nutzt TensorFlow und das ResNet50-Modell, um Bilder zu analysieren und die wahrscheinlichste Klasse des Modells zu bestimmen. Auf Basis dieser Klassifikation werden Erklärungen mithilfe von GradCAM und Similarity Explanation generiert. Bilder können vorab im richtigen Format bereitgestellt oder über separate Funktionen und Dateien formatiert werden.

## Inhaltsverzeichnis
1. [Verwendung](#verwendung)
2. [Funktionen und Features](#funktionen-und-features)
3. [Konfiguration](#konfiguration)
4. [Lizenz](#lizenz)
5. [Autoren](#autoren)

## Verwendung
1. 
    Formatieren von Bildern: Falls die Bilder noch nicht im richtigen Format vorliegen, kann dies mit dem Notebook `image_transformation.ipynb` durchgeführt werden.
2. 
    Vorhersagen generieren: Verwenden Sie das Notebook `resnet_prediction.ipynb`, um die Vorhersage des Modells für die wahrscheinlichste Klasse zu erhalten.
3.
    Erklärungen erstellen: Übertragen Sie die vorhergesagte Klassen-ID manuell in die Notebooks für GradCAM `gradcam.ipynb` und Similarity Explanation `similarity_exp_tensorflow_tfds.ipynb`, um Erklärungsbilder zu generieren. 

## Funktionen und Features
- Verwendung des ResNet50-Modells zur Bildklassifikation.
- GradCAM zur Visualisierung der wichtigsten Bildbereiche, die das Modell zur Klassifikation verwendet hat.
- Similarity Explanation zur Berechnung und Visualisierung von Bildähnlichkeiten basierend auf dem ImageNet-Datensatz.

## Konfiguration
Python 3.9.11 dient als Kernel. Für die Nutzung der Similarity Explanation wird der ImageNet-Datensatz benötigt, der über 100 GB groß sein kann und manuell heruntergeladen werden muss. Stellen Sie sicher, dass genügend Speicherplatz verfügbar ist.

## Lizenz
Dieses Projekt ist nur für den internen Gebrauch im Rahmen meiner Bachelorarbeit bestimmt und basiert auf Quellcode aus anderen Projekten, die unter unterschiedlichen Lizenzen veröffentlicht wurden. Es wird nicht für eine breite Veröffentlichung oder kommerzielle Nutzung freigegeben.

## Autoren
Robert Lenz