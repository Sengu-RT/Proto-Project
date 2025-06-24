# Spotify Playlist LCD Anzeige

Steuere deine Spotify Playlist auf einem LCD-Display mit Node-RED mit Skip-Funktion und Reset-Funktion um an den Anfang zu kommen

## 🔧 Funktionsweise
1. **Playlist-Abruf** via Spotify API
   - Authentifizierung mit OAuth-Token
   - Abfrage der aktuellen Playlist
2. **Datenverarbeitung** in Node-RED
   - Speicherung aller Songs im Flow-Kontext
   - Extrahierung von Songname und Künstler
3. **LCD-Ausgabe**
   - Zeile 1: Songname
   - Zeile 2: Künstler
4. **Skip-Funktion**
   - Manuelles Durchschalten per Button-Trigger
5. **Reset-Funktion**
   - Manuelles Reset per Button-Trigger

## 🛠 Hardware
| Komponente          | Beschreibung                     |
|---------------------|----------------------------------|
| Raspberry Pi        | Node-RED Host                   |
| 16x2 LCD Display   | I2C oder parallele Anbindung     |
| Taster             | Für Skip-Funktion (GPIO)         |

## 📋 Installationsanleitung

### 1. Voraussetzungen
Node-RED installieren
sudo apt-get install nodered
Python Bibliotheken
pip install RPi.GPIO smbus2
