# Softwaretechnik Klausurvorbereitung

Dieses Verzeichnis dient der Vorbereitung auf eine Softwaretechnik-Klausur (Universitätskurs "SWT"). In der Klausur ist ein selbst beschriebenes A3-Blatt als Hilfsmittel erlaubt.

## Zentrales Dokument

[fabiuebersicht.txt](fabiuebersicht.txt) ist der Dreh- und Angelpunkt der gesamten Vorbereitung. Es ist die digitalisierte Abschrift des handgeschriebenen A3-Spickzettels eines Kommilitonen ("Fabi") — laut Aussage des Nutzers ein Vorzeigestudent. Der gesamte Stoff, an dem sich die Vorbereitung entlanghangelt, orientiert sich an diesem Dokument.

Wichtige Eigenheiten beim Umgang damit:

- **`[GRAFIK]`-Platzhalter**: Im Original standen an diesen Stellen Diagramme/Skizzen (z. B. Aktivitätsdiagramm, Netzplan, Zweigüberdeckungs-Beispiele, dynamische Modellierung), die beim Digitalisieren nicht übertragen wurden. Diese Lücken sollten bei der Vorbereitung aktiv mit Fachwissen gefüllt werden, nicht ignoriert werden.
- **Ungleichmäßige Informationsdichte**: Manche Blöcke sind nur stichpunktartig, obwohl sie im Original deutlich mehr Platz eingenommen haben. Besonders markiert ist der Entwurfsmuster-Block (Proxy, Befehlsmuster, Abstrakte Fabrik, Strategie, Beobachter, Adapter, Brücke, Fassade, ...) — laut Notiz im Dokument der größte Block auf dem Original-Blatt, hier aber nur in Stichpunkten vorhanden. Diesen Bereich bei Erklärungen entsprechend ausführlicher behandeln.
- Das Dokument ist auf Deutsch und teils in flapsiger Stichpunktform verfasst (eigene Abkürzungen, kleine Tippfehler wie "Zuverlässigkeit" statt vermutlich "Verständlichkeit"). Beim Erklären eher den fachlich korrekten Begriff verwenden und ggf. auf Unstimmigkeiten hinweisen.

## Weitere Materialien

- [vl/](vl/) — Foliensätze der Vorlesungen (VL), nummeriert und thematisch benannt (z. B. `04_UML.pdf`, `11_Entwurfsmuster.pdf`, `17_Prozessmodelle.pdf`). Decken den Stoff deutlich ausführlicher ab als fabiuebersicht.txt.
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

**Was kommt in eine Zusammenfassung?** Nicht der komplette Inhalt einer VL-Folie, sondern nur das, was auch in fabiuebersicht.txt oder in den ub/-Übungen zu dem Thema vorkommt. ub/ und fabiuebersicht.txt sind die Filter, die festlegen, was klausurrelevant ist — wir hangeln uns an ihnen entlang und schreiben die zugehörigen Inhalte aus den ausführlicheren vl/-Folien heraus.

**Ablauf (wird vom Nutzer angestoßen, z. B. "schreibe die Inhalte aus Übung X heraus"):**
1. Prüfen, welche Themen die betreffende ub/-Datei behandelt.
2. Die dazu passende(n) vl/-Datei(en) identifizieren (Nummerierung/Thema stimmen meist ungefähr überein, aber nicht 1:1 — z. B. kann eine Übung mehrere VL-Themen abdecken oder umgekehrt).
3. Aus den vl/-Folien die relevanten Inhalte (zu dem, was in der Übung + ggf. fabiuebersicht.txt vorkommt) extrahieren und als eigene HTML-Datei in summaries/ ablegen.
4. Dateiname orientiert sich am Namen/Thema der VL-Folie (nicht am ub-Dateinamen), z. B. Übung `08_ub_entwurfsmuster.pdf` → Folie `11_Entwurfsmuster.pdf`/`12_Entwurfsmuster2.pdf` → Summary-Datei zu "Entwurfsmuster". Pro VL-Thema eine Datei.
5. Später wird derselbe Prozess mit fabiuebersicht.txt als Filter statt/zusätzlich zu den Übungen wiederholt, um Lücken zu schließen, die die Übungen nicht abdecken.

**Bestehende Summaries nachpflegen:** Es ist gängige Praxis, bereits erstellte Summary-Dateien später zu ergänzen statt nur neue anzulegen. Wenn z. B. nach Durcharbeiten aller Übungen mit fabiuebersicht.txt als Filter weitergemacht wird (Schritt 5), landen dabei häufig Inhalte, die eigentlich zu einem bereits behandelten VL-Thema gehören (z. B. taucht beim Abgleich mit fabiuebersicht.txt ein Punkt zu "Entwurfsmuster" auf, obwohl `summaries/Entwurfsmuster.html` schon existiert). In solchen Fällen die passende bestehende Datei identifizieren und dort ergänzen (an sinnvoller Stelle einfügen, nicht anhängen), statt eine neue/duplizierte Datei zu erzeugen. Vor dem Erstellen einer neuen Summary-Datei daher immer kurz prüfen, ob zum Thema schon eine existiert.

**Index-Seite pflegen:** [index.html](index.html) im Root verlinkt alle Summary-Dateien (relative Links auf `summaries/...`, funktioniert lokal und auf GitHub Pages). Bei jeder neu erstellten Summary-Datei einen Eintrag in index.html ergänzen. Die einzelnen Summary-Dateien selbst brauchen keine Navigation zurück — dafür reicht der Browser-Zurück-Button.

**Format der HTML-Dateien:** bewusst kein Website-Anspruch — keine Accessibility, kein Responsive Design, kein Framework. Nur einfaches, sehr minimalistisches HTML+CSS zum bequemen Lesen im Browser als persönliche Notizen (klare Überschriften, Listen, ggf. simple Tabellen). Schnell zu erstellen und zu lesen ist wichtiger als Design.

## Wie Claude helfen soll

- Als Lern-/Prüfungscoach fungieren: Konzepte aus fabiuebersicht.txt erklären, Verständnisfragen stellen, Wissen abfragen.
- Bei Bedarf fehlende `[GRAFIK]`-Inhalte fachlich rekonstruieren (z. B. UML-Aktivitätsdiagramm-Notation, Netzplan-Beispiel).
- Zusammenhänge zwischen Stichpunkten herstellen, die im Original nur lose nebeneinanderstehen (z. B. Qualitätssicherung ↔ Testarten ↔ Prozessmodelle).
- Antworten auf Deutsch, da das Vorbereitungsmaterial und der Nutzer auf Deutsch kommunizieren.
- Bei Widersprüchen oder Unklarheiten im Originaldokument nachfragen bzw. transparent machen, statt sie stillschweigend zu glätten.
