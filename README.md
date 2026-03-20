# **🔵 MERBLA MEDNASS (Marble Madness Retro Edition)**

[https://codepen.io/Felix-Schmidt2025/pen/bNwrRBX](https://codepen.io/Felix-Schmidt2025/pen/bNwrRBX)

## **🚀 Highlights**

* **Single-File Engine:** Das gesamte Spiel (Logik, Grafik-Engine, Physik und Sound) ist in einer einzigen Datei unter 1000 Zeilen Code untergebracht.  
* **Isometrische 3D-Welt:** Echtes Depth-Sorting sorgt dafür, dass die Murmel korrekt hinter Wänden und Objekten verschwindet.  
* **CRT-Ästhetik:** Dynamische Glow-Effekte, Scanlines und Screen-Shake simulieren das Gefühl eines alten Arcade-Automaten.  
* **Prozedurales Audio:** Keine externen Assets\! Alle Sounds (Rollen, Aufprall, Ziel-Fanfare) werden via **Web Audio API** in Echtzeit synthetisiert.  
* **Mobile Ready:** Unterstützt sowohl Tastatursteuerung als auch intuitive Touch-Gesten.

## **🕹 Steuerung**

| Eingabe | Aktion |
| :---- | :---- |
| **W, A, S, D** / **Pfeiltasten** | Murmel steuern |
| **Enter** / **Leertaste** | Spiel starten / Menü-Auswahl |
| **Zahlen 1 \- 6** | Level-Direktwahl (im Hauptmenü) |
| **Touch / Drag** | Murmel in die entsprechende Richtung lenken |

## **🏁 Die Rennen (Races)**

Das Spiel beinhaltet **6 verifizierte Level** mit steigendem Schwierigkeitsgrad:

1. **Practice:** Lerne die Grundlagen der Trägheit.  
2. **Intermediate:** Erste Hindernisse und Abgründe.  
3. **Aerial:** Enge Pfade in schwindelerregender Höhe.  
4. **Silly:** Rutschiges Eis und tückische Steigungen.  
5. **Ultimate:** Komplexe Verzweigungen und aggressive Gegner.  
6. **Nightmare:** Die ultimative Herausforderung für deine Feinmotorik.

## **🛠 Technische Details**

### **Physik & Rendering**

Die Engine nutzt eine klassische isometrische Transformation, um 3D-Koordinaten auf den 2D-Canvas zu projizieren. Die Physik simuliert:

* **Hangabtriebskraft:** Beschleunigung auf Rampen.  
* **Materialeigenschaften:** Unterschiedliche Reibungswerte auf Bodenplatten und Eis.  
* **Kollisionserkennung:** Interaktion mit Pyramiden, Stahlkugeln und Schleim-Gegnern.

### **Entwickler-Schnittstelle (API)**

Du kannst das Spiel direkt über die Browser-Konsole (F12) steuern oder modifizieren. Das globale Objekt MarbleMadness bietet folgende Funktionen:

* loadLevel(index): Lädt ein spezifisches Level (0-5).  
* setPhysics(params): Ändert Laufzeitparameter (z.B. maxSpeed oder bounce).  
* exportJSON() / importJSON(data): Erlaubt das Speichern und Laden von Level-Layouts.

## **📦 Installation**

Keine Installation notwendig.

1. Kopiere den Code in eine Datei namens index.html.  
2. Öffne die Datei in einem modernen Webbrowser (Chrome, Firefox, Safari oder Edge).  
3. Fertig\!

---

*Entwickelt mit Leidenschaft für Retro-Gaming und minimalistischen Code.*

---

**Soll ich dir noch eine Kurzanleitung schreiben, wie man die Physik-Parameter im Code so anpasst, dass das Spiel einfacher oder schwieriger wird?**
