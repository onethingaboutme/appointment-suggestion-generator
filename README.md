# appointment-suggestion-generator
🗓️ Privacy-first appointment scheduler for Nextcloud/DAVx5 users.   ✨ Open-Source (GPLv3) | 📱 Android-Only | 🔒 No trackers, no cloud!  

# Terminhelfer / Appointment Assistant  
**🇩🇪 Privatsphäre-freundliche Terminfindung** | **🇬🇧 Privacy-first meeting scheduler** 

### 🇩🇪 Warum diese App?  
**Das Problem**:  
- Terminfindung per E-Mail/Chat ist umständlich ("Wann passt dir? 14 Uhr? Nein, dann...")  
- Kalender-Apps zeigen deine Verfügbarkeit oft Drittanbietern  

**Die Lösung**:  
- 🔒 **Lokale Analyse** deines Android-Kalenders (via Nextcloud/DAVx5-Sync)  
- 🤖 **Automatische Vorschläge** für freie Zeitfenster  
- 📤 **Teilen per Text** (z.B. Signal, E-Mail) – Empfänger:in braucht *keine* App  

### 🇬🇧 Why This App?  
**The Problem**:  
- Coordinating meetings via email/chat is tedious ("How about 2pm? No? Then 3pm?")  
- Calendar apps often expose your availability to third parties  

**The Solution**:  
- 🔒 **Local analysis** of your Android calendar (via Nextcloud/DAVx5 sync)  
- 🤖 **Auto-generated suggestions** for free time slots  
- 📤 **Share via text** (e.g. Signal, email) – no app required for recipients  

---

## 🇩🇪 Kernfunktionen / 🇬🇧 Key Features  
| 🇩🇪 | 🇬🇧 |  
|-----|-----|  
| 🛡️ **Offline-Zuerst** – Keine Internetverbindung nötig | 🛡️ **Offline-First** – No internet required |  
| 📅 **3-Schritte-Workflow**:<br>1. Zeitraum wählen<br>2. Vorschläge generieren<br>3. Teilen & Bestätigen | 📅 **3-Step Workflow**:<br>1. Pick time window<br>2. Generate slots<br>3. Share & Confirm |  
| 🗑️ **Automatisches Aufräumen** – Vorläufige Termine werden bei Bestätigung gelöscht | 🗑️ **Auto-Cleanup** – Tentative events get removed on confirmation |  

---

## 🇩🇪 Technische Details / 🇬🇧 Tech Stack  
**Architekturprinzipien**:  
- 🔐 **Datensparsamkeit**: Keine Berechtigungen außer Kalenderzugriff  
- 📱 **Android-Only**: Optimiert für DAVx5-Nutzer:innen  
- 🧩 **Modularer Code**: Einfache Erweiterbarkeit  

**Tools**:  
```plaintext
Python 3.9+ | KivyMD (UI) | ics.py (Kalenderdaten) | PyJNIus (Android-APIs)
