# Outlook PST & OST Browser | Editor (OutlookVault 2026)

![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11-0078D4?style=flat-square)
![Framework](https://img.shields.io/badge/.NET-8.0-512BD4?style=flat-square)
![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)
![Security](https://img.shields.io/badge/Security-AES256-green?style=flat-square)
![Build](https://img.shields.io/badge/Build-149-orange?style=flat-square)

**Outlook PST & OST Browser | Editor** ist eine hochmoderne WPF-Anwendung zur revisionssicheren Archivierung, Betrachtung und Extraktion von Microsoft Outlook-Daten. Das System arbeitet vollständig lokal und speichert Inhalte in einer hochverschlüsselten SQLite-Datenbank, unabhängig von einer laufenden Outlook-Installation.

<img width="1658" height="937" alt="2026-01-02 23_18_08-Outlook PST   OST Browser _ Editor _ BOREAS _ 02 01 2026 _ Profil_ malte speck@o" src="https://github.com/user-attachments/assets/3c28d122-bbc3-4c13-bce0-93b3c2ed9bd9" />
<img width="1660" height="935" alt="2026-01-02 23_18_22-Outlook PST   OST Browser _  Editor _  BOREAS _ DB_ BOREAS_vault db" src="https://github.com/user-attachments/assets/da7c262d-bf11-45f3-991f-2bef7ed6f3fe" />
<img width="1658" height="937" alt="2026-01-02 23_19_24-Outlook PST   OST Browser _  Editor _  BOREAS _ DB_ BOREAS_vault db" src="https://github.com/user-attachments/assets/9b956ac5-653c-4e5a-bedd-4367335dc074" />
<img width="500" height="700" alt="2026-01-02 23_21_26-" src="https://github.com/user-attachments/assets/679023c0-0541-4793-acaa-32718b0fc99c" />
<img width="800" height="500" alt="2026-01-02 23_21_43-" src="https://github.com/user-attachments/assets/c6ad2727-5223-4011-99f8-b22a3678d62b" />
---

## 🚀 Hauptfunktionen (Features)

### 🎨 Modernes UI & UX Design
* **Windows 11 Style:** Rahmenlose Fenster, moderne Dialogführung und Schatteneffekte für eine elegante Optik.
* **Intelligente Farbkodierung:**
    * **Betreff:** Dunkelgrün
    * **Absender:** Dunkelrot
    * **Datum:** Outlook-Blau
* **Neon-Icons:** Wichtige Systemfunktionen (DB-Check, Optimierung, Backup) sind durch Neon-Grün und Neon-Magenta hervorgehoben.
* **Live-Systemuhr:** Farbige Statusleisten-Uhr (Stunden: Schwarz | Minuten: Rot | Sekunden: Gold).
* **Integrierter Viewer:** HTML-Rendering für E-Mails und Vorschau für Anhänge (PDF, Office, etc.).

### 🔒 Sicherheit & Architektur
* **AES-256 Verschlüsselung:** Alle Daten landen in einer passwortgeschützten `_vault.db`. Der Zugriff ist ohne Key unmöglich.
* **Audit-Log:** Ein detailliertes Sicherheitsprotokoll (`logs.db`) speichert alle Aktionen (Import, Export, Löschungen, Login-Versuche).
* **Domain-Lock (Anti-Commercial):** Die Software erkennt automatisch, ob der Computer Teil einer Firmen-Domäne ist und verweigert in diesem Fall den Start.

### 📥 Import & Synchronisation
* **Full Auto Import:** Sichert vollautomatisch das gesamte aktive Outlook-Profil.
* **Diff Import (Smart Update):** Selektiver Import, der Datumsstempel vergleicht und nur neue oder geänderte E-Mails importiert (Inkrementelles Backup).
* **PST Support:** Direktes Einlesen externer `.pst` Dateien.

### 📤 Export & Management
* **ZIP-Export:** Exportiert ganze Ordnerstrukturen inkl. Anhängen als ZIP-Archiv.
* **EML-Export:** Speichert einzelne Nachrichten im universellen Format.
* **Wartung:** `VACUUM`-Befehl zur Datenbank-Komprimierung und Integritätsprüfung.

---

## 🛠️ Technische Voraussetzungen

* **OS:** Windows 10 oder Windows 11 (64-Bit)
* **Runtime:** .NET Desktop Runtime 8.0
* **Datenbank:** SQLite (Microsoft.Data.Sqlite)
* **Abhängigkeit:** Für die Import-Funktionen muss Microsoft Outlook (Classic) installiert sein.

---

## ⚖️ Lizenz & Nutzungsbedingungen

**Copyright © 2026 Malte Speck**

Dieses Softwareprodukt ist **proprietär**. Die Nutzung ist an folgende Bedingungen geknüpft:

> 1.  **Private Lizenz:** Die Software darf ausschließlich von Privatpersonen für persönliche Zwecke genutzt werden.
> 2.  **Keine kommerzielle Nutzung:** Der Einsatz in Unternehmen, Behörden oder für gewerbliche Zwecke ist strengstens untersagt. Die Software enthält technische Schutzmaßnahmen (Domain-Check), um dies durchzusetzen.
> 3.  **Weitergabe:** Das Kopieren, Modifizieren oder Verteilen des Quellcodes oder der Binärdateien ist ohne schriftliche Genehmigung des Urhebers nicht gestattet.

---

## ⚠️ Haftungsausschluss

Die Nutzung der Software erfolgt auf eigene Gefahr. Der Entwickler übernimmt keine Haftung für Datenverlust, Korruption von Outlook-Profilen oder andere Schäden, die aus der Nutzung der Software entstehen könnten. Es wird empfohlen, regelmäßige Backups der `.db` Dateien durchzuführen.

---

*Erstellt mit ❤️ und .NET 8 © 2026 Malte Speck*
