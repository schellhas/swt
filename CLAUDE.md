# Softwaretechnik Klausurvorbereitung

Dieses Verzeichnis dient der Vorbereitung auf eine Softwaretechnik-Klausur (Universitätskurs "SWT"). In der Klausur ist ein selbst beschriebenes A3-Blatt als Hilfsmittel erlaubt.

## Zentrales Dokument

[uebersicht.txt](uebersicht.txt) ist der Dreh- und Angelpunkt der gesamten Vorbereitung (hieß früher "fabiuebersicht.txt" — falls das an anderer Stelle noch auftaucht, ist der aktuelle Dateiname gemeint). Es ist die digitalisierte Abschrift des handgeschriebenen A3-Spickzettels eines Kommilitonen ("Fabi") — laut Aussage des Nutzers ein Vorzeigestudent. Der gesamte Stoff, an dem sich die Vorbereitung entlanghangelt, orientiert sich an diesem Dokument.

**Aktueller Stand:** Alle ub/-Übungen sind durchgearbeitet (Schritt 1-4 des Workflows unten abgeschlossen). Schritt 5 (uebersicht.txt als aktiver Filter) läuft: ein erster Lückenschluss-Durchgang über das gesamte Dokument wurde bereits gemacht, jetzt wird zusätzlich systematisch in 8 Teilen (siehe Tabelle unten) nachgearbeitet, analog zum ub/-Workflow.

Wichtige Eigenheiten beim Umgang damit:

- **`[GRAFIK]`-Platzhalter**: Im Original standen an diesen Stellen Diagramme/Skizzen (z. B. Aktivitätsdiagramm, Netzplan, Zweigüberdeckungs-Beispiele, dynamische Modellierung), die beim Digitalisieren nicht übertragen wurden. Diese Lücken sollten bei der Vorbereitung aktiv mit Fachwissen gefüllt werden, nicht ignoriert werden.
- **Ungleichmäßige Informationsdichte**: Manche Blöcke sind nur stichpunktartig, obwohl sie im Original deutlich mehr Platz eingenommen haben. Besonders markiert ist der Entwurfsmuster-Block (Proxy, Befehlsmuster, Abstrakte Fabrik, Strategie, Beobachter, Adapter, Brücke, Fassade, ...) — laut Notiz im Dokument der größte Block auf dem Original-Blatt, hier aber nur in Stichpunkten vorhanden. Diesen Bereich bei Erklärungen entsprechend ausführlicher behandeln.
- Das Dokument ist auf Deutsch und teils in flapsiger Stichpunktform verfasst (eigene Abkürzungen, kleine Tippfehler wie "Zuverlässigkeit" statt vermutlich "Verständlichkeit"). Beim Erklären eher den fachlich korrekten Begriff verwenden und ggf. auf Unstimmigkeiten hinweisen.

## Weitere Materialien

- [vl/](vl/) — Foliensätze der Vorlesungen (VL), nummeriert und thematisch benannt (z. B. `04_UML.pdf`, `11_Entwurfsmuster.pdf`, `17_Prozessmodelle.pdf`). Decken den Stoff deutlich ausführlicher ab als uebersicht.txt.
- [ub/](ub/) — Foliensätze/Aufgaben der Übungen (UB), ebenfalls nummeriert (z. B. `08_ub_entwurfsmuster.pdf`, `09_ub_ocl.pdf`).
- [other/](other/) — sonstige Materialien der Vorlesung: externe Paper/Buchkapitel, die von einzelnen Übungen als Pflichtlektüre referenziert werden (z. B. `NusEas00-RE-roadmap.pdf` für Übung 4, `Brooks_No Silver Bullet.pdf` für Übung 1), sowie ergänzende Foliensätze zu Themen, die in vl/ nicht (vollständig) behandelt werden (z. B. `statecharts_activitydiagrams.pdf` für die in VL08 fehlende Aktivitätsdiagramm-Notation). Kein festes Namensschema — Inhalt und Bezug zu ub/vl beim Lesen erschließen.
- Alle drei Ordner sind **read-only** — Dateien darin nicht verändern, umbenennen oder löschen.
- Bei jeder neuen Übung prüfen, ob other/ passendes Material enthält (Dateinamen/Themen mit der Übung abgleichen), nicht nur vl/. Wurde eine Übung schon ohne Berücksichtigung von other/ bearbeitet, gilt dieselbe Nachpflege-Praxis wie unten beschrieben.

## Workflow: summaries/

[summaries/](summaries/) enthält die selbst erstellten Zusammenfassungen — hier entsteht die eigentliche Arbeit.

**Kernzweck — Single Point of Truth zum Büffeln:** Die summaries/-Dateien sind für den Nutzer (den Lernenden) die einzige Quelle, mit der später gelernt wird — nicht die Original-PDFs. Sinn der ganzen Übung ist es, aus den ausführlichen, redundanten, teils schwer lesbaren Foliensätzen genau das Wichtige herauszudestillieren, sodass am Ende **weniger Text als in den Folien** übrig bleibt und der Nutzer nur noch die Summaries pauken muss, ohne je wieder in vl/ oder ub/ nachschauen zu müssen. Das heißt konkret:
- Destillieren statt kopieren: eigene, knappe Formulierungen statt Folienfüllwörter/Redundanzen 1:1 zu übernehmen.
- Nichts Prüfungsrelevantes weglassen (siehe Filterregel unten), aber auch nichts Prüfungsirrelevantes aus Vollständigkeitsdrang mitschleppen.
- Im Zweifel gilt: lieber eine Spur zu ausführlich als eine Lücke lassen — aber straffen, wo es ohne Informationsverlust geht, statt Folienabschnitte breitzutreten.

**Was kommt in eine Zusammenfassung?** Nicht der komplette Inhalt einer VL-Folie, sondern nur das, was auch in uebersicht.txt oder in den ub/-Übungen zu dem Thema vorkommt. ub/ und uebersicht.txt sind die Filter, die festlegen, was klausurrelevant ist — wir hangeln uns an ihnen entlang und schreiben die zugehörigen Inhalte aus den ausführlicheren vl/-Folien heraus.

**Ablauf (wird vom Nutzer angestoßen, z. B. "schreibe die Inhalte aus Übung X heraus"):**
1. Prüfen, welche Themen die betreffende ub/-Datei behandelt.
2. Die dazu passende(n) vl/-Datei(en) identifizieren (Nummerierung/Thema stimmen meist ungefähr überein, aber nicht 1:1 — z. B. kann eine Übung mehrere VL-Themen abdecken oder umgekehrt).
3. Aus den vl/-Folien die relevanten Inhalte (zu dem, was in der Übung + ggf. uebersicht.txt vorkommt) extrahieren und als eigene HTML-Datei in summaries/ ablegen.
4. Dateiname orientiert sich am Namen/Thema der VL-Folie (nicht am ub-Dateinamen), z. B. Übung `08_ub_entwurfsmuster.pdf` → Folie `11_Entwurfsmuster.pdf`/`12_Entwurfsmuster2.pdf` → Summary-Datei zu "Entwurfsmuster". Pro VL-Thema eine Datei.
5. Später wird derselbe Prozess mit uebersicht.txt als Filter statt/zusätzlich zu den Übungen wiederholt, um Lücken zu schließen, die die Übungen nicht abdecken.

**8-Teile-Einteilung von uebersicht.txt (für Schritt 5):** Um uebersicht.txt aus Token-Budget-Gründen häppchenweise abzuarbeiten (analog "nächste Übung"), ist es in 8 Teile aufgeteilt — an thematischen Blockgrenzen (Leerzeilen im Dokument), sodass nie ein einzelner Block zerrissen wird. Aufruf z. B. mit "arbeite jetzt übersicht Teil 3 ab":

| Teil | Zeilen | Themen |
|---|---|---|
| 1 | 1–49 | Aufgaben der SWT, Akteure/Stakeholder, Arten von Anforderungen, Validierung, Verifizierung, Wie baut man SW (Entwurfsprinzipien), Systemzerlegung, UML-Sichtbarkeit, Information Hiding |
| 2 | 51–96 | OCL (Einstieg), Tests (Grundbegriffe), Wer soll testen?, 2 Stile von PM, Ziele der Softwareentwicklung, Prozesse (konventionell/agil), Aktivitätsdiagramm |
| 3 | 98–142 | Anwendungsfall (Template), Wirkung von Modularisierung, Module beurteilen, OCL iterate, Qualitätssicherung (Überblick) |
| 4 | 144–189 | Arten von Tests (Black-/White-Box, Zweigüberdeckung), Aufgaben des PM, Aufgabenzerlegung, Risiko, Anwendungs-/Technische Domäne |
| 5 | 191–254 | Normales-/Radikales Vorgehen, Testverfahren-Notiz, Arten von Tests (Benutzbarkeit/Last/Leistung/Stress/Akzeptanz), Netzplan, Taxonomie "Die Welt der Softwaretechnik" |
| 6 | 256–302 | Analysten/Entwerfer, Software/SWT-Definitionen, Dynamische Modellierung, Anwendungs-/Lösungsdomänenklasse, Problem-/Lösungsbereich, Anforderungsdokument, Architekturstile, Design by Contract, Entwurfsmuster-Block, Statische Verfahren |
| 7 | 304–341 | Methoden für Anforderungserhebung, Konstruktive QS (Prozessmgmt-Leitlinien), Iterative Prozessmodelle (inkl. Scrum/XP), Universelle Prozessmodelle, Wiederverwendung |
| 8 | 343–380 | Prinzipien zur Wiederverwendung, Softwareprozess/Prozessmodelle, Wasserfallmodell, Schwächen Wasserfallmodell, Strikte/Agile Modelle, Schlussgrafik |

Teil 5 ist bewusst größer (der Taxonomie-Block ist mit 43 Zeilen allein schon fast ein ganzer Teil und gehört inhaltlich untrennbar zu "Normales/Radikales Vorgehen" direkt davor — beide stammen aus derselben Vorlesungseinheit vl/03).

Für jeden Teil gilt derselbe Abgleich wie bei den Übungen: prüfen, was in den bestehenden Summaries schon abgedeckt ist, Lücken identifizieren, passende vl/-Quelle(n) heranziehen, bestehende Dateien ergänzen statt duplizieren (siehe unten).

**Bestehende Summaries nachpflegen:** Es ist gängige Praxis, bereits erstellte Summary-Dateien später zu ergänzen statt nur neue anzulegen. Wenn z. B. nach Durcharbeiten aller Übungen mit uebersicht.txt als Filter weitergemacht wird (Schritt 5), landen dabei häufig Inhalte, die eigentlich zu einem bereits behandelten VL-Thema gehören (z. B. taucht beim Abgleich mit uebersicht.txt ein Punkt zu "Entwurfsmuster" auf, obwohl `summaries/Entwurfsmuster.html` schon existiert). In solchen Fällen die passende bestehende Datei identifizieren und dort ergänzen (an sinnvoller Stelle einfügen, nicht anhängen), statt eine neue/duplizierte Datei zu erzeugen. Vor dem Erstellen einer neuen Summary-Datei daher immer kurz prüfen, ob zum Thema schon eine existiert.

**Index-Seite pflegen:** [index.html](index.html) im Root verlinkt alle Summary-Dateien (relative Links auf `summaries/...`, funktioniert lokal und auf GitHub Pages). Bei jeder neu erstellten Summary-Datei einen Eintrag in index.html ergänzen. Die einzelnen Summary-Dateien selbst brauchen keine Navigation zurück — dafür reicht der Browser-Zurück-Button.

**Format der HTML-Dateien:** bewusst kein Website-Anspruch — keine Accessibility, kein Responsive Design, kein Framework. Nur einfaches, sehr minimalistisches HTML+CSS zum bequemen Lesen im Browser als persönliche Notizen (klare Überschriften, Listen, ggf. simple Tabellen). Schnell zu erstellen und zu lesen ist wichtiger als Design.

## Wie Claude helfen soll

- Als Lern-/Prüfungscoach fungieren: Konzepte aus uebersicht.txt erklären, Verständnisfragen stellen, Wissen abfragen.
- Bei Bedarf fehlende `[GRAFIK]`-Inhalte fachlich rekonstruieren (z. B. UML-Aktivitätsdiagramm-Notation, Netzplan-Beispiel).
- Zusammenhänge zwischen Stichpunkten herstellen, die im Original nur lose nebeneinanderstehen (z. B. Qualitätssicherung ↔ Testarten ↔ Prozessmodelle).
- Antworten auf Deutsch, da das Vorbereitungsmaterial und der Nutzer auf Deutsch kommunizieren.
- Bei Widersprüchen oder Unklarheiten im Originaldokument nachfragen bzw. transparent machen, statt sie stillschweigend zu glätten.
