# Kachelduell

Ein rundenbasiertes Match-3-Duell für den Browser, komplett in einer einzigen HTML-Datei mit Canvas-Grafik. Das Spielgefühl orientiert sich an PvP-Match-3-Spielen wie Match Masters, Grafik und Inhalte sind eigenständig gestaltet.

## Spielen

`index.html` im Browser öffnen. Es gibt keine Abhängigkeiten und keinen Build-Schritt, nur die Schriften werden von Google Fonts geladen.

Online spielen über GitHub Pages: unter **Settings → Pages** als Quelle den Branch `main` und den Ordner `/ (root)` wählen. Das Spiel ist danach unter `https://<benutzer>.github.io/kachel/` erreichbar.

## Regeln

- Zwei Spieler ziehen abwechselnd auf **demselben Brett**, jede Runde mit **2 Zügen**.
- Jeder zerstörte Stein ist **1 Punkt**. Wer nach der letzten Runde mehr Punkte hat, gewinnt.
- **4 oder mehr** Steine auf einmal geben einen **Extrazug**.
- Spezialsteine:
  - 4 in einer Reihe: **Pfeil**, räumt Reihe oder Spalte
  - L- oder T-Form: **Bombe**, räumt ein 3×3-Feld
  - 5 in einer Reihe: **Blitz**, trifft zufällige Steine
  - Zwei Spezialsteine tauschen löst eine Kombo aus.
- Blaue Sterne laden deinen **Booster**, rote Kreise den des Gegners. Ist die Kugel voll, wird der Booster per Antippen gezündet.
- **Hammer** und **Mischen** gibt es je einmal pro Spiel. Booster, Karten und Werkzeuge kosten keinen Zug.

## Funktionen

- Spielmodi: Gegen einen Rivalen, Turnier (3 Gegner im K.-o.-System), Tagesbrett, Zwei Spieler an einem Gerät
- Vier Rivalen mit eigenem Spielstil, drei Schwierigkeitsstufen, 3, 5 oder 7 Runden
- Vier Booster: Farbsturm, Kreuzfeuer, Meteorschauer, Blitzgewitter
- 16 besondere Karten in vier Seltenheiten, Deck aus 3 Karten, Kartenpacks im Shop, Sammelalbum
- Münzen, Level, Ränge, 12 Erfolge, Statistik, Tagesbonus
- Original-Regeln oder Bonus-Regeln mit Kreisel, Eis, Gold, Kettenbonus und doppelter Finalrunde
- Zugtimer, Pause, automatisches Speichern, Tipps, Tastaturkürzel, Sound, Kontrastmodus, drei Brett-Designs

Fortschritt und Spielstand werden im `localStorage` des Browsers gespeichert.

## Tastatur

| Taste | Aktion |
| --- | --- |
| Pfeiltasten, Leertaste | Cursor bewegen, Stein wählen |
| 1–3 | Karte spielen |
| B | Booster |
| H | Hammer |
| M | Mischen |
| T | Tipp |
| F | Rivalenzug vorspulen |
| P, Esc | Pause |
