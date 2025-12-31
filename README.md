# 🛡️ Outlook PST & OST Browser | Editor

![License](https://img.shields.io/badge/Lizenz-Proprietär-red.svg)
![Platform](https://img.shields.io/badge/Plattform-Windows-lightgrey.svg)
![Framework](https://img.shields.io/badge/.NET-8.0-blueviolet.svg)

**Outlook PST & OST Browser | Editor** ist eine professionelle Hochleistungs-Lösung zur forensischen Analyse, Verwaltung und Bearbeitung von Microsoft Outlook Datendateien. Die Software erlaubt es, E-Mails, Anhänge und komplexe Ordnerstrukturen zu extrahieren, zu editieren und in einer AES-256 verschlüsselten Datenbank sicher zu archivieren.

<img width="1618" height="885" alt="2025-12-31 14_57_29-Outlook PST   OST Browser_Editor _ Outlook 16 0 0 19530 _ BOREAS _ 31 12 2025" src="https://github.com/user-attachments/assets/9d14106b-0b24-4f78-8f74-c2a9f95b08c9" />
---

## 🚀 Kernfunktionen

* **🔍 Deep Extraction & Browsing**
    Vollständige Rekonstruktion und blitzschnelle Navigation durch Outlook-Ordnerhierarchien in Echtzeit.
* **📂 Universal Import Support**
    Nahtlose Anbindung an aktive Outlook-Profile (**Auto Import**) sowie Standalone-Support für **PST**-Archive und **OST**-Offline-Caches.
* **✍️ Integrierter Editor**
    Gezieltes Löschen und Verwalten von Inhalten direkt im Tresor, um Archivbestände sauber zu halten.
* **🔐 AES-256 Verschlüsselung**
    Militärstandard-Verschlüsselung für alle HTML-Körper und Dateianhänge. Der Schlüssel wird via PBKDF2 aus Ihrem Master-Passwort abgeleitet.
* **💎 Smart Compression (Deep Clean)**
    Einzigartiger Algorithmus zur physikalischen Minimierung der Datenbankgröße durch Entfernung verwaister Datenfragmente.

---

## 🛠️ Technische Umsetzung

### Architektur & Stack
* **Framework:** .NET 8.0 (Windows Desktop)
* **Datenbank:** SQLite mit **WAL-Mode** (Write-Ahead Logging) für maximale Datenintegrität.
* **Security:** Implementierung von `System.Security.Cryptography.Aes` (256-Bit) für alle sensiblen Datenfelder.

### 🧠 Speichermanagement (Vacuum Logic)
Im Gegensatz zu einfachen Viewern implementiert dieser Editor eine dreistufige Kompressionstechnologie:
1.  **Orphaned Data Detection:** Identifikation von Anhängen und HTML-Fragmenten ohne gültige Mail-Referenz.
2.  **WAL Checkpoint:** Synchronisation der Schreibvorgänge zur Vermeidung von Datenverlust.
3.  **Physical Vacuum:** Physikalische Reorganisation der Datenbankbits zur effektiven Reduzierung der Dateigröße.

---

## 📦 Installation & Benutzung

Die Software wird als schlüsselfertiger **Installer** bereitgestellt.

1.  Laden Sie die neueste `Outlook_Browser_Editor_Setup.exe` aus den Releases herunter.
2.  Folgen Sie dem Setup-Assistenten.
3.  **Passwort-Sicherheit:** Vergeben Sie beim ersten Start ein Master-Passwort. 
    > ⚠️ **Achtung:** Das Passwort wird nirgendwo gespeichert. Ohne dieses Passwort ist der Zugriff auf die verschlüsselte Datenbank unmöglich.

---

## ⚠️ Hinweis zu OST-Dateien
Microsoft bindet OST-Dateien fest an die ursprüngliche Hardware. Das Öffnen von OST-Dateien fremder Systeme kann den Fehler **0x80004005** verursachen. In diesem Fall nutzen Sie bitte die Funktion **Auto Import** auf dem Originalgerät.

---

## ⚖️ Lizenz

Diese Software ist ein proprietäres Produkt von **Malte Speck**. Es handelt sich NICHT um Open-Source-Software.
Die Nutzung unterliegt der in diesem Repository enthaltenen [eigenen Lizenzvereinbarung (EULA)](LICENSE.txt).

**Wichtigste Einschränkungen:**
- für die Nutzung, für kommerzielle Zwecke ist eine separate Genehmigung erfordert.
- Keine Weiterverbreitung ohne ausdrückliche Genehmigung.
- Kein Reverse Engineering (Rückentwicklung) oder Modifikation des Codes.
- Alle Rechte vorbehalten.

---

## 📧 Kontakt
Entwickelt von **Malte Speck**. Bei technischen Fragen oder für Lizenzanfragen kontaktieren Sie mich bitte über dieses GitHub-Profil.
