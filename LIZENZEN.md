# Lizenzen und Quellen

Stand: 07.11.2026 · Sorgfältig recherchiert, aber keine Rechtsberatung.
Einzelheiten mit Fundstellen und Zitaten: `daten/QUELLEN.md`.

## Inhalt

1. Kurzüberblick
2. Gebärdendaten (CC BY-SA 3.0)
3. SignWriting-Schriften (SIL OFL 1.1)
4. Python-Pakete (MIT)
5. Eigene Teile dieses Ordners
6. Pflichten beim Weitergeben
7. Volltext SIL Open Font License 1.1
8. Zusatz Satz-Videos (SignDict)

## 1. Kurzüberblick

| Teil | Lizenz | Weitergabe |
|---|---|---|
| `daten/lexikon_dgs.csv`, `daten/auswahl_protokoll.csv` | CC BY-SA 3.0 Unported (abgeleitet aus SignPuddle DGS) | ja, mit Namensnennung und unter gleicher Lizenz |
| SignWriting-Schriften (Sutton SignWriting Line/Fill/OneD) | SIL Open Font License 1.1 | ja; Lizenztext unten (Abschnitt 7) und in `daten/OFL.txt` |
| Python-Paket `signwriting` (wird per `pip` installiert, nicht mitgeliefert) | MIT | ja |
| `gebaerden.py`, `lesehilfe.py`, `gebaerden_fenster.py`, `app/`, `app_bauen.py`, `skill_paket_bauen.py`, Startdateien, `daten/grundformen.csv`, Anleitungen | MIT (siehe Abschnitt 5) | ja |
| `Gebaerden-App.html` | enthält die Gebärdenbilder aus dem Lexikon → als Ganzes CC BY-SA 3.0; Programmteil MIT | ja, Fußzeile nicht entfernen |
| erzeugte HTML-Seiten | enthalten Gebärden aus dem Lexikon → CC BY-SA 3.0; der Quellenhinweis steht in jeder Seite unten | ja, Fußzeile nicht entfernen |
| `videos.py`, `videos_anforderungen.txt`, `vorschau.py`, `app/videoplayer.js` | MIT | ja |
| Video- und Wort-Verzeichnis (`video_cache/videoindex.json`, `video_cache/woerterindex.json`, eingebettet in `Gebaerden-App.html`) | nur Verweise auf SignDict-Videos mit Zeiten, Urheber und Lizenz – enthält keine Videos | ja |
| Satz-Videos und `video_cache/` (nur bei eingeschalteter Zusatzoption) | Bearbeitungen frei lizenzierter SignDict-Videos → siehe Abschnitt 8 | ja, mit Nachweisen |

**Nicht verwendet:** SignBank+ (github.com/sign-language-processing/signbank-plus) steht unter
CC BY-NC 4.0 (nur nichtkommerziell; Fundstelle: Datei `LICENSE`, Commit 5b643f2). Deshalb wurde
kein Eintrag daraus übernommen; die Gebärden stammen direkt aus der Originalquelle SignPuddle.

## 2. Gebärdendaten (CC BY-SA 3.0)

**Quelle:** SignPuddle Online, „Deutsche Gebärdensprache“ (Puddle 53),
Center for Sutton Movement Writing / Valerie Sutton und Beitragende.
Export https://www.signbank.org/signpuddle2.0/data/spml/sgn53.spml, abgerufen am 07.11.2026
(Stand der Datei 13.10.2025, SHA-256 `3fa48486…6cec8a`).

**Lizenz:** Creative Commons Namensnennung – Weitergabe unter gleichen Bedingungen 3.0 Unported
(CC BY-SA 3.0), https://creativecommons.org/licenses/by-sa/3.0/deed.de.
Fundstelle: https://www.signwriting.org/ (Startseite): SignWriting-Inhalte „are free to use because
they are licensed under … Creative Commons Attribution-ShareAlike 3.0 Unported License“.

**Änderungen:** Auswahl von 298 Einträgen, deutsche Synonyme in Spalte `deutsch` ergänzt,
Glossen-Namen vergeben. Die SignWriting-Codes (Spalte `fsw`) sind unverändert. Jede Zeile nennt
in Spalte `quelle` die Eintrags-ID; `daten/auswahl_protokoll.csv` nennt zusätzlich die Beitragenden.

SignWriting® / GebärdenSchrift: © Valerie Sutton, Center for Sutton Movement Writing, Inc.

## 3. SignWriting-Schriften (SIL OFL 1.1)

Die Bilder werden mit den Schriften „Sutton SignWriting Line“ und „Sutton SignWriting Fill“
(Version 1.1.0) gezeichnet. Sie kommen mit dem Python-Paket `signwriting` auf den Rechner
(Ordner `signwriting/visualizer/`) und liegen diesem Ordner nicht bei.
Copyright (c) 1974–2014 Center For Sutton Movement Writing, Inc., Reserved Font Names
„Sutton SignWriting“ und „Sutton SignWriting Fill“. Lizenz: SIL Open Font License 1.1
(Fundstelle: Namens-Eintrag 0 in den .ttf-Dateien). Volltext: Abschnitt 7.

Die Erklärtexte der Lesehilfe (`lesehilfe.py`) sind eigene Formulierungen nach V. Sutton,
„Lessons in SignWriting“ (signwriting.org/lessons) und der Symbolordnung ISWA 2010
(signbank.org/iswa); es werden keine Texte oder Bilder von dort übernommen, die Beispielzeichen
werden mit den oben genannten Schriften gezeichnet.

## 4. Python-Pakete (MIT)

- `signwriting` 0.1.20 – MIT License, Copyright (c) 2024 Sign Language Processing
  (Fundstelle: `signwriting-0.1.20.dist-info/licenses/LICENSE`; github.com/sign-language-processing/signwriting).
- Das Fingeralphabet (Option „Fingeralphabet“) stammt aus den Daten des Pakets `signwriting`
  (`signwriting/fingerspelling/data/gsg.json`, MIT); in `Gebaerden-App.html` sind diese Buchstaben als Bilder eingebettet.
- `Pillow` und `regex` werden als Abhängigkeiten mitinstalliert (eigene freie Lizenzen: MIT-CMU bzw. Apache 2.0).
- `sutton-signwriting-font` 1.0.1 (MIT, Copyright (c) 2025 Steve Slevinski) wurde geprüft, wird aber nicht benötigt.

## 5. Eigene Teile dieses Ordners

`gebaerden.py`, `lesehilfe.py`, `gebaerden_fenster.py`, `app/regeln.js`, `app/vorlage.html`, `app_bauen.py`,
`Start-Linux.sh`, `Start-Windows.bat`, `Start-Mac.command`, `skill_paket_bauen.py`, `skill/SKILL.md`, `daten/grundformen.csv`,
`LIESMICH.md`, `LIZENZEN.md` und die Beispieltexte in `beispiele/` stehen unter der MIT-Lizenz:

> Copyright (c) 2026 die Verfasser des Projekts „Gebaerden-Piktogramme“
>
> Permission is hereby granted, free of charge, to any person obtaining a copy of this software
> and associated documentation files (the "Software"), to deal in the Software without restriction,
> including without limitation the rights to use, copy, modify, merge, publish, distribute,
> sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in all copies or
> substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
> NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
> NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
> OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
> CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Die erzeugten HTML-Ergebnisse in `beispiele/` enthalten Gebärden aus dem Lexikon und stehen
deshalb unter CC BY-SA 3.0 (Quellen wie in Abschnitt 2).

## 6. Pflichten beim Weitergeben

1. Den ganzen Ordner weitergeben, mindestens mit `LIZENZEN.md`, `daten/QUELLEN.md` und `daten/OFL.txt`.
2. Das Lexikon (auch verändert oder erweitert) nur unter **CC BY-SA 3.0** weitergeben und die
   Quelle nennen: „SignPuddle Online, Deutsche Gebärdensprache (Puddle 53), Center for Sutton
   Movement Writing / Valerie Sutton und Beitragende, CC BY-SA 3.0“.
3. Neue Einträge nur aus einer Quelle mit verträglicher Lizenz übernehmen und in Spalte
   `quelle` belegen. Keine selbst gezeichneten Gebärden ohne Abnahme durch DGS-Kundige.
4. Die Quellen-Fußzeile in erzeugten HTML-Seiten nicht entfernen.
5. Werden die Schriftdateien (.ttf) selbst mitgegeben: `daten/OFL.txt` beilegen; die Schriften nicht
   einzeln verkaufen.
6. Satz-Videos nur zusammen mit den Nachweisen weitergeben (Fußzeile der Ergebnisseite oder
   `video_cache/quellen.csv`), siehe Abschnitt 8.

## 7. Volltext SIL Open Font License 1.1

```
Copyright (c) 1974-2014 Center For Sutton Movement Writing, Inc. (http://signwriting.org),
with Reserved Font Names Sutton SignWriting and Sutton SignWriting Fill.
(Copyright-Inhaber, Jahre und Reserved Font Names aus dem Namens-Eintrag 0 der Fonts
 SuttonSignWritingLine/Fill/OneD.ttf, Version 1.1.0, in die Vorlagezeilen eingesetzt; Lizenztext unten unverändert von
 https://openfontlicense.org/documents/OFL.txt, abgerufen am 07.11.2026.)

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at:
https://openfontlicense.org


-----------------------------------------------------------
SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007
-----------------------------------------------------------

PREAMBLE
The goals of the Open Font License (OFL) are to stimulate worldwide
development of collaborative font projects, to support the font creation
efforts of academic and linguistic communities, and to provide a free and
open framework in which fonts may be shared and improved in partnership
with others.

The OFL allows the licensed fonts to be used, studied, modified and
redistributed freely as long as they are not sold by themselves. The
fonts, including any derivative works, can be bundled, embedded,
redistributed and/or sold with any software provided that any reserved
names are not used by derivative works. The fonts and derivatives,
however, cannot be released under any other type of license. The
requirement for fonts to remain under this license does not apply
to any document created using the fonts or their derivatives.

DEFINITIONS
"Font Software" refers to the set of files released by the Copyright
Holder(s) under this license and clearly marked as such. This may
include source files, build scripts and documentation.

"Reserved Font Name" refers to any names specified as such after the
copyright statement(s).

"Original Version" refers to the collection of Font Software components as
distributed by the Copyright Holder(s).

"Modified Version" refers to any derivative made by adding to, deleting,
or substituting -- in part or in whole -- any of the components of the
Original Version, by changing formats or by porting the Font Software to a
new environment.

"Author" refers to any designer, engineer, programmer, technical
writer or other person who contributed to the Font Software.

PERMISSION & CONDITIONS
Permission is hereby granted, free of charge, to any person obtaining
a copy of the Font Software, to use, study, copy, merge, embed, modify,
redistribute, and sell modified and unmodified copies of the Font
Software, subject to the following conditions:

1) Neither the Font Software nor any of its individual components,
in Original or Modified Versions, may be sold by itself.

2) Original or Modified Versions of the Font Software may be bundled,
redistributed and/or sold with any software, provided that each copy
contains the above copyright notice and this license. These can be
included either as stand-alone text files, human-readable headers or
in the appropriate machine-readable metadata fields within text or
binary files as long as those fields can be easily viewed by the user.

3) No Modified Version of the Font Software may use the Reserved Font
Name(s) unless explicit written permission is granted by the corresponding
Copyright Holder. This restriction only applies to the primary font name as
presented to the users.

4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
Software shall not be used to promote, endorse or advertise any
Modified Version, except to acknowledge the contribution(s) of the
Copyright Holder(s) and the Author(s) or with their explicit written
permission.

5) The Font Software, modified or unmodified, in part or in whole,
must be distributed entirely under this license, and must not be
distributed under any other license. The requirement for fonts to
remain under this license does not apply to any document created
using the Font Software.

TERMINATION
This license becomes null and void if any of the above conditions are
not met.

DISCLAIMER
THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
OTHER DEALINGS IN THE FONT SOFTWARE.
```

## 8. Zusatz Satz-Videos (SignDict)

Gilt nur, wenn die Zusatzoption Satz-Videos eingeschaltet wird (`--videos` bzw. Häkchen).

- **Quelle:** SignDict.org, abgefragt über die öffentliche Schnittstelle
  (https://signdict.org/graphql-api). Jedes Video trägt dort seine eigene Lizenz und den Namen
  der gebärdenden bzw. hochladenden Person. Beides wird mit gespeichert
  (`video_cache/quellen.csv`) und auf jeder Ergebnisseite unten genannt.
- **Auswahl:** Standardmäßig nur Videos unter CC BY, CC BY-SA oder CC0 (Funktion `lizenz_frei`
  in `videos.py`). Videos mit ND (keine Bearbeitung) und Videos ohne Lizenzangabe werden immer
  übersprungen, weil zugeschnitten wird.
- **Auf Wunsch NC (`--videos-nc` / zweites Häkchen):** Dann auch CC BY-NC und CC BY-NC-SA
  (Funktion `lizenz_nc`); freie Videos haben Vorrang. CC BY-SA und CC BY-NC-SA verlangen für
  Bearbeitungen jeweils ihre eigene Lizenz und lassen sich daher nicht sauber zu einem Werk
  verbinden. Sätze mit NC-Videos werden deshalb nicht verschmolzen, sondern als Folge einzelner,
  nur zugeschnittener und angeglichener Clips gespeichert und nacheinander abgespielt; jeder Clip
  steht unter der Lizenz seines Originals. Ergebnisse mit NC-Clips nur nicht kommerziell nutzen
  und weitergeben (Hinweis steht auf der Seite). Sorgfältige Einschätzung, keine Rechtsberatung.
- **Bearbeitung:** Die Einzelvideos werden zugeschnitten, im Bildausschnitt angeglichen und
  mit Überblendungen verbunden. Darauf weist jede Ergebnisseite hin.
- **Lizenz der Satz-Videos:** CC BY-SA verlangt für Bearbeitungen dieselbe oder eine spätere
  Lizenzversion; CC BY 4.0 lässt sich mit CC BY-SA 4.0 verbinden. Die Satz-Videos werden deshalb
  unter **CC BY-SA 4.0** gekennzeichnet. Das ist eine sorgfältige Einschätzung, keine
  Rechtsberatung.
- **Nicht geprüft:** die allgemeinen Nutzungsbedingungen von SignDict über die Videolizenzen hinaus.
- **Persönlichkeitsrecht:** Die Videos zeigen echte Menschen. Sie haben die Videos zur freien
  Nutzung bereitgestellt; trotzdem die Satz-Videos nur für den gedachten Zweck verwenden und
  nicht in fremde Zusammenhänge stellen.
- **Programmteile:** `videos.py` und `vorschau.py` stehen unter MIT. Die per `pip` installierten Pakete
  (`mediapipe`, `opencv-python-headless`, `numpy`, `imageio-ffmpeg`) haben eigene, freie Lizenzen
  (Apache 2.0, Apache 2.0, BSD, BSD-2) und werden nicht mitgeliefert. Das Erkennungsmodell
  „Pose Landmarker lite“ von Google (Apache 2.0) wird beim ersten Mal in `video_cache/modelle/` geladen.
  ffmpeg (über `imageio-ffmpeg` oder vom System) steht unter LGPL/GPL.

### 8a. Videos in der Browser-Seite (seit 07.11.2026 abends)

- Die Browser-Seite (`Gebaerden-App.html`) und daraus gespeicherte Seiten **laden keine Videos
  herunter und verändern sie nicht.** Sie spielen die Originaldateien direkt von SignDict ab
  (Verweis auf die Videoadresse) und springen dabei auf den Abschnitt mit der Gebärde; zwischen
  zwei Clips wird im Browser kurz überblendet. Es entsteht keine Videodatei.
- Ausgewählt wird nach denselben Regeln wie oben (frei vor NC, ND nie); das gilt auch für das
  Wort-Verzeichnis aller SignDict-Wörter (`videos.py --woerter`). NC-Videos sind in der
  Browser-Seite **immer** dabei (Entscheidung E16); die Leiste über den Videos und die Nachweise
  weisen auf „nur nicht kommerziell“ hin. Die Browser-Seite mit Videos ist damit nur für
  nicht kommerzielle Nutzung gedacht.
- Unter den Videos stehen für jedes gezeigte Video Urheber, Lizenz und Link zum SignDict-Eintrag.
- Nicht geprüft: ob SignDict bzw. der Videospeicher (assets.wishlephant.com) das direkte
  Einbinden von Videos in fremde Seiten wünscht oder technisch einschränkt; die allgemeinen
  Nutzungsbedingungen von SignDict (siehe oben). Sorgfältige Einschätzung, keine Rechtsberatung.
- Datenschutz: Beim Abspielen sieht der Videospeicher von SignDict, welche Videos abgerufen
  werden (und damit ungefähr, welche Wörter im Text stehen). Der Text selbst wird nicht übertragen.
