# 4x4-Chess-LA1305
# Projekt-Dokumentation

**Dorian Herzig**

| Datum       | Version | Zusammenfassung                                              |
| ----------- | ------- | ------------------------------------------------------------ |
| 03.05.2024  | 0.0.1   | Projektinitialisierung und erste Planungen durchgeführt.     |
| 10.05.2024  | 0.0.2   | Grundlegende Spielregeln und User Stories definiert.         |
| 17.05.2024  | 0.0.3   | Implementierung des Spielbretts und der Figurenbewegungen.   |
| 24.05.2024  | 0.0.4   | Erstellen der Testfälle und erste Tests durchgeführt.        |
| 31.05.2024  | 0.0.5   | Fehlerbehebungen und Verbesserungen basierend auf Testergebnissen. |
| 07.06.2024  | 0.0.6   | Finalisierung der Implementierung und Durchführung weiterer Tests. |
| 14.06.2024  | 1.0.0   | Abschluss des Projekts und Erstellung der Projektdokumentation. |

## 1 Informieren

### 1.1 Ihr Projekt

**Projektname:** 4x4-Schach

**Beschreibung:** Das Projekt "4x4-Schach" zielt darauf ab, eine vereinfachte Version des traditionellen Schachspiels auf einem 4x4-Brett zu entwickeln. Ziel ist es, die grundlegenden Konzepte und Strategien von Schach zu lehren, während die Komplexität des Spiels reduziert wird. Dabei soll eine funktionsfähige Anwendung entstehen, die von jedem genutzt werden kann, um Schach in seiner einfachsten Form zu spielen.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ         | Beschreibung                                        |
| ---- | --------------- | ----------- | --------------------------------------------------- |
| 1    | Muss            | Funktional  | Als Spieler möchte ich ein 4x4-Schachbrett sehen, damit ich das Spiel starten kann. |
| 2    | Muss            | Funktional  | Als Spieler möchte ich meine Figuren bewegen können, damit ich das Spiel spielen kann. |
| 3    | Muss            | Funktional  | Als Spieler möchte ich die Züge meines Gegners sehen, damit ich auf diese reagieren kann. |
| 4    | Muss            | Funktional  | Als Spieler möchte ich eine Sieg- oder Niederlagenanzeige sehen, damit ich weiss, wann das Spiel endet. |
| 5    | Kann            | Qualität    | Als Spieler möchte ich eine Anleitung haben, damit ich die Regeln des 4x4-Schachs lernen kann. |
| 6    | Kann            | Funktional  | Als Spieler möchte ich mein Spiel speichern und laden können, damit ich später weiterspielen kann. |

### 1.3 Testfälle

| TC-№ | Ausgangslage                          | Eingabe                       | Erwartete Ausgabe                          |
| ---- | ------------------------------------- | ----------------------------- | ------------------------------------------ |
| 1.1  | Spiel wird gestartet                  | Spielbrett anzeigen           | Ein 4x4-Schachbrett wird angezeigt.        |
| 2.1  | Spielbrett ist angezeigt              | Figur von A2 nach A3 bewegen  | Die Figur bewegt sich von A2 nach A3.      |
| 3.1  | Spieler hat Zug gemacht               | Gegner zieht Figur von B2 nach B3 | Die gegnerische Figur bewegt sich von B2 nach B3. |
| 4.1  | Eine Spielfigur erreicht die letzte Reihe | -                             | Siegmeldung wird angezeigt.                |
| 5.1  | Startbildschirm                       | Anleitung aufrufen            | Die Regeln des 4x4-Schachs werden angezeigt. |
| 6.1  | Während des Spiels                    | Spiel speichern               | Das Spiel wird erfolgreich gespeichert.    |


## 2 Planen

| AP-№ | Frist     | Zuständig   | Beschreibung                                    | geplante Zeit |
| ---- | --------- | ----------- | ----------------------------------------------- | ------------- |
| 1.A  | 03.05.2024| Dorian Herzig| Projektinitialisierung und Definition des 4x4-Schachbretts | 45'           |
| 2.A  | 10.05.2024| Dorian Herzig| Implementierung der Figurenbewegungen           | 90'           |
| 3.A  | 17.05.2024| Dorian Herzig| Implementierung der Gegnerzüge                  | 60'           |
| 4.A  | 24.05.2024| Dorian Herzig| Sieg- und Niederlagenanzeige implementieren     | 45'           |
| 5.A  | 31.05.2024| Dorian Herzig| Erstellung der Spielanleitung                   | 45'           |
| 6.A  | 07.06.2024| Dorian Herzig| Implementierung der Speicher- und Ladefunktion  | 90'           |
| 7.A  | 14.06.2024| Dorian Herzig| Durchführung und Dokumentation von Tests        | 60'           |

Total: 435'

## 3 Entscheiden

**Entscheidungen und Annahmen:**

- Das Schachbrett wird auf eine 4x4-Grösse reduziert, um das Spiel schneller und einfacher zu gestalten.
- Die grundlegenden Regeln von Schach werden beibehalten, aber es wird keine Rochade oder en passant geben.
- Das Spiel wird als Einzelspieler gegen einen einfachen Computergegner implementiert.
- Eine grafische Benutzeroberfläche (GUI) wird verwendet, um das Schachbrett und die Figuren darzustellen.

## 4 Realisieren

| AP-№ | Datum       | Zuständig    | geplante Zeit | tatsächliche Zeit |
| ---- | ----------- | ------------ | ------------- | ----------------- |
| 1.A  | 03.05.2024  | Dorian Herzig | 45'           | 45'               |
| 2.A  | 10.05.2024  | Dorian Herzig | 90'           | 90'               |
| 3.A  | 17.05.2024  | Dorian Herzig | 60'           | 75'               |
| 4.A  | 24.05.2024  | Dorian Herzig | 45'           | 60'               |
| 5.A  | 31.05.2024  | Dorian Herzig | 45'           | 45'               |
| 6.A  | 07.06.2024  | Dorian Herzig | 90'           | 100'              |
| 7.A  | 14.06.2024  | Dorian Herzig | 60'           | 60'               |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum       | Resultat | Tester        |
| ---- | ----------- | -------- | ------------- |
| 1.1  | 24.05.2024  | bestanden| Dorian Herzig |
| 2.1  | 24.05.2024  | bestanden| Dorian Herzig |
| 3.1  | 24.05.2024  | bestanden| Dorian Herzig |
| 4.1  | 24.05.2024  | bestanden| Dorian Herzig |
| 5.1  | 24.05.2024  | bestanden| Dorian Herzig |
| 6.1  | 24.05.2024  | nicht bestanden| Dorian Herzig |


### 5.2 Exploratives Testen

| BR-№ | Ausgangslage          | Eingabe                    | Erwartete Ausgabe            | Tatsächliche Ausgabe |
| ---- | --------------------- | -------------------------- | ---------------------------- | -------------------- |
| I    | Während des Spiels    | Figur ausserhalb des Brettes bewegen | Fehlerhinweis oder keine Aktion | Fehlerhinweis        |
| II   | Während des Spiels    | Ungültiger Zug             | Fehlerhinweis oder keine Aktion | Fehlerhinweis        |

## 6 Auswerten

Die Auswertung kann im Maharaportfolieo gefunden werden gefunden werden.
