 !-- translate="no" lang="en" --
# <span lang="en">Nesting-Challenge</span>
**Serious Game Prototyp zur Portfolioaufgabe UE06 (Aufgabe 2\*)**

Modul E-Learning / Lerntechnologie · TU Dresden · Sommersemester 2026
Björn Födisch · bbQ24 · Juli 2026

---

## Kontext

Dieses Repository begleitet die schriftliche Reflexion zur **Portfolioaufgabe UE06**. Aufgabe 2\* verlangt, das Fehlen eines geeigneten Serious Games für den eigenen Lerngegenstand zu begründen und zu skizzieren, wie eine passgenaue Game-Based-Learning-Umgebung aussehen müsste.

Für die **algorithmische Zuschnittoptimierung in der Holztechnik** (Nesting an der Plattenaufteilsäge) existiert kein solches Spiel, die ausführliche Begründung dafür steht in der schriftlichen Abgabe.

Dieses Repository geht über die geforderte Skizze hinaus: Es enthält einen **tatsächlich spielbaren Prototyp**, der die zentralen Prinzipien der Reflexion exemplarisch umsetzt:

- **Consequential Feedback**: Fehlerhafte Entscheidungen zeigen sich erst beim simulierten Sägeversuch, nicht durch vorbeugende Blockaden
- **Guillotine-Zwang**: Authentische Simulation der Plattenaufteilsäge
- **Reststückmanagement**: Bewusste Trennung zwischen Verschnitt und wiederverwendbarem Reststoff

---

## Was ist das hier?

**Das ist:**
- Eine gegenständliche Machbarkeitsprüfung: Kann eine domänentreue Simulation der Zuschnittplanung als Serious Game funktionieren, ohne auf aufgesetzte Belohnungssysteme (Punkte, Badges) zurückzugreifen?
- Ein funktionsfähiger Prototyp, der die theoretischen Erkenntnisse der Portfolioarbeit technisch umsetzt
- Ein Demonstrator für Learning-by-Doing-Ansätze in der Berufsausbildung

**Das ist nicht:**
- Ein fertiges, produktives Lernspiel
- Ein vollständiges didaktisches Konzept
- Eine Implementierung aller real existierenden Holzwerkstoffe und deren Maserungsregeln

---

## Zentrale Designentscheidungen

### Werkstoff & Format
- Nur Spanplatte spielbar (mit aktuellen Einstellungen)
- Sperrholz und Massivholz als Vorschau hinterlegt, ihre sperrenden Maserrichtungsregeln sind einer späteren Ausbaustufe vorbehalten
- Reales Plattenformat: 2800 × 2070 mm (Egger-Vollformat, Querformat)

### Spielmechanik
- 10 Bauteile pro Runde mit Spielraum statt Volltiling, die Anordnung hat echten Einfluss auf das Ergebnis
- Guillotine-Zwang: Jeder Schnitt muss durchgehend über die gesamte Platte geführt werden, wie an der realen Plattenaufteilsäge
- Schnittfuge: 3,5 mm
- Anschnitt: 30 mm Randverlust wegen Lagerschaden

### Bewertung & Feedback
- Verschnittbewertung nach realistischen Kriterien: Nur tatsächlich unbrauchbarer Kleinabfall zählt als Verschnitt, getrennt vom wiederverwendbaren Reststück
- Vergleich mit automatischem Referenzplan, der Spieler sieht, wie nah er an einem optimalen Schnittplan herangekommen ist
- Kein Verhindern von Fehlern: Eine falsche Anordnung wird nicht vorab blockiert, sie zeigt sich erst beim simulierten Sägeversuch
- Consequential Feedback analog zum Learning-by-Doing-Ansatz (Brown/Collins/Duguid 1989)

---

## Spielen

### Live-Version
Verfügbar hier:
- **[🎮 Direkt im Browser spielen](https://htmlpreview.github.io/?https://github.com/BSLehrer/E-Learning/blob/main/nesting_challenge_4.html)** - Öffnet die HTML-Datei direkt im BrowserLearning/main/nesting_challenge_4.html)** - Öffnet die HTML-Datei direkt im Browser
- **[⬇️ Download](https://github.com/BSLehrer/E-Learning/raw/main/nesting_challenge_4.html)** - Datei herunterladen und lokal spielenherunterladen und lokal spielen

### Lokal spielen
1. `index.html` im Browser öffnen
2. Keine Installation oder externe Abhängigkeiten nötig

---

## Bezug zur schriftlichen Arbeit

Die vollständige theoretische Begründung, Alignment-Analyse und Literaturverankerung steht in der PDF-Abgabe zu UE06. Sie umfasst:

- Lave & Wenger (1991): Communities of Practice und situiertes Lernen
- Brown/Collins/Duguid (1989): Cognitive Apprenticeship und Consequential Feedback
- Gee (2003): Prinzipien effektiver Games für Lernprozesse
- Domänenspezifische Anforderungen der Holztechnik und Zuschnittoptimierung

Dieser Prototyp liefert den technischen Machbarkeitsnachweis für die theoretischen Erkenntnisse.
