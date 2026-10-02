# Klassik & Oper verstehen

Eine interaktive Lern-App (Single-File HTML) ueber klassische Musik und Oper:
Epochen & Komponisten, Opern-Aufbau & Stimmfaecher, interaktiver Orchester-Sitzplan,
Interpretation & Qualitaetskriterien, beste Orchester & Dirigenten, Quiz und Glossar.

Die App ist komplett auf Deutsch. Oeffne `index.html` im Browser.

**Live:** https://mvonulmerbach-ship-it.github.io/klassik-oper-lern-app/

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | die ganze App (Reiter Musik, Oper, Welt; 575 Fragen) |
| `interpretationen.html` | 100 Werke und ihre Deutungen, oeffnet als Overlay (Karte auf der Startseite, 🎯 in der Quiz-Fussleiste) |
| `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `icon-maskable.png` | Installation als App |
| `sw.js` | Service Worker fuer den Offline-Betrieb |

Hell/Dunkel oben rechts: ◐ System (Standard) · ☀️ Hell · 🌙 Dunkel. Lernstand und Wahl liegen nur im Browser (`localStorage`, Schluessel `klassik_lern_v1`).

## Auf dem Handy installieren

Seite in Chrome oeffnen → Menue ⋮ → „Zum Startbildschirm hinzufuegen“ (Safari: Teilen → „Zum Home-Bildschirm“).

## Offline

Nach dem ersten Oeffnen laeuft die App ohne Netz, auch die Interpretationen (Service Worker, network first mit Cache als Rueckfall).
