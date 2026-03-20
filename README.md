🔵 MERBLA MEDNASS

MERBLA MEDNASS https://codepen.io/Felix-Schmidt2025/pen/bNwrRBX ist ein hochperformantes, isometrisches Geschicklichkeitsspiel, das als Hommage an den Arcade-Klassiker Marble Madness entwickelt wurde. Das gesamte Spiel – inklusive Engine, 6 Leveln, Physik und synthetisiertem Sound – ist in einer einzigen, abhängigkeitsfreien HTML-Datei untergebracht.

🚀 Features

Single-File Architecture: Keine externen Assets, Bilder oder Libraries. Alles wird prozedural generiert.

Retro Glow Aesthetic: CRT-Scanlines, Bloom-Effekte und dynamische isometrische Schatten für echtes Arcade-Feeling.

Synthetisierter Audio-Engine: Echtzeit-Generierung von Soundeffekten (Rollen, Aufprall, Zerbrechen) über die Web Audio API.

Präzise Physik: Simulation von Trägheit, Hangabtriebskraft, Reibung (inkl. Eis-Level) und Kollisionen.

6 Herausfordernde Level: Von "Practice" bis zum "Nightmare Race" mit steigendem Schwierigkeitsgrad.

Cross-Platform: Volle Unterstützung für Tastatur (Desktop) und Touch-Gesten (Mobile).

🕹 Steuerung

Eingabe

Aktion

W, A, S, D / Pfeiltasten

Murmel steuern

Enter / Space

Menü-Auswahl bestätigen

Zahlen 1 - 6

Direkte Level-Anwahl im Menü

Touch / Drag

Intuitive Steuerung auf Mobilgeräten

🛠 Technische Details

Isometrische Engine

Das Spiel nutzt eine klassische isometrische Transformation zur Darstellung der 3D-Welt auf einem 2D-Canvas. Ein spezieller Tiefensortierungs-Algorithmus sorgt dafür, dass die Murmel korrekt mit Wänden, Rampen und Hindernissen interagiert.

Physik & Hindernisse

Rampen: Beeinflussen die Beschleunigung basierend auf der Neigungsrichtung.

Eis: Reduzierte Reibung und verzögerte Steuerung.

Pyramiden: Wirken als Bumper und stoßen die Murmel ab.

Säure: Sofortige Zerstörung der Murmel.

Gegner: Slimes und Stahlkugeln mit individuellen Patrouillen-Pfaden.

Web Audio Synthese

Statt statische Dateien zu laden, nutzt das Projekt Oszillatoren:

Das Rollgeräusch ist ein bandpass-gefiltertes weißes Rauschen, dessen Frequenz proportional zur Geschwindigkeit variiert.

Zerbrech-Sounds nutzen Square-Waves mit schnellem Decay.

🔓 Entwickler-Schnittstelle (API)

Das Spiel exponiert ein globales Objekt window.MarbleMadness, über das man via Browser-Konsole (F12) eingreifen kann:

// Level manuell laden
MarbleMadness.loadLevel(5);

// Physik zur Laufzeit anpassen
MarbleMadness.setPhysics({ targetSpeed: 0.1, slopeGravity: 0.01 });

// Aktuelle Leveldaten als JSON exportieren
const levelData = MarbleMadness.exportJSON();


📦 Installation

Keine Installation notwendig.

Klone das Repository oder kopiere die index.html.

Öffne die Datei in einem modernen Webbrowser.

git clone [https://github.com/dein-benutzer/merbla-mednass.git](https://github.com/dein-benutzer/merbla-mednass.git)
cd merbla-mednass
open index.html


📄 Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert. Frei zur Nutzung, Modifikation und Distribution.

Entwickelt mit Leidenschaft für Retro-Gaming und sauberen Code.
