# Machine-Learning-Projekt: Aufgabe

*Deutsche Version von `01_assignment.md`.*

Das ist euer zweites Projekt. Als Team bringt ihr einen echten Datensatz von den Rohdaten bis zu einem funktionierenden Machine-Learning-Modell und einer Präsentation für Stakeholder (Auftraggeber). Ziel ist es, gemeinsam den ganzen Data-Science-Lebenszyklus zu üben: ein Problem formulieren, eine Baseline bauen, mit Fehleranalyse verbessern (**iterate with error analysis**) und die Ergebnisse einem Publikum ohne Technikwissen vermitteln.

Dieses Template-Repository ist euer Startpunkt. Es bringt eine fertig eingerichtete Umgebung mit und ein Beispiel-Notebook, das ein einfaches Modell mit minimaler Bereinigung und Feature-Auswahl trainiert. Seht es als Gerüst (**scaffolding**) für euer eigenes Projekt.

Arbeitet die Abschnitte unten der Reihe nach durch: zuerst ein Projekt wählen, dann auf einem Board planen, bauen und verbessern, und zum Schluss die Abgabe vorbereiten.

## Ein Projekt wählen

Wählt als Team eine Option. Sucht euch ein Problem mit einem klaren Stakeholder und einem klaren Geschäftsnutzen (**business value**).

### Option A: Zindi-Challenge (leicht bis fortgeschritten)

Wählt eine Challenge auf [Zindi](https://zindi.africa/competitions). Erfüllt die Anforderungen der Challenge und bereitet zusätzlich eine Präsentation für Stakeholder vor.

1. [Tanzania Tourism Prediction](https://zindi.africa/competitions/tanzania-tourism-prediction/data) (leicht, 2 Personen)
2. [Fraud Detection in Electricity and Gas Consumption](https://zindi.africa/competitions/fraud-detection-in-electricity-and-gas-consumption-challenge) (mittel, mit Starter-Notebook, 2 bis 3 Personen)
3. [Urban Air Pollution Challenge](https://zindi.africa/competitions/zindiweekendz-learning-urban-air-pollution-challenge) (mittel bis fortgeschritten, 3 Personen und etwas Fachwissen)
4. [Flight Delay Prediction](https://zindi.africa/competitions/flight-delay-prediction-challenge) (mittel, 3 Personen; Flughafendaten über [airportsdata](https://pypi.org/project/airportsdata/))
5. [Financial Inclusion in Africa](https://zindi.africa/competitions/financial-inclusion-in-africa) (leicht, 2 Personen)

### Option B: Erfolg von Kickstarter-Projekten (mittel)

In den letzten Jahren sind die Möglichkeiten, Projekte von Einzelpersonen und kleinen Firmen zu finanzieren, stark gewachsen. Neben Ersparnissen, Bankkrediten und Geld von Freunden und Familie ist **Crowdfunding** (Schwarmfinanzierung) zu einer beliebten und leicht zugänglichen Alternative geworden.

Kickstarter wurde 2009 gegründet und ist eine bekannte Crowdfunding-Plattform. Sie arbeitet nach dem Alles-oder-nichts-Prinzip: Ein Projekt wird nur finanziert, wenn es sein Zielbetrag erreicht. Sonst zahlen die Unterstützer (**backers**) nichts.

Viele Faktoren tragen zum Erfolg oder Misserfolg eines Projekts bei, allgemein und auch auf Kickstarter. Einige davon lassen sich messen oder in Kategorien einteilen. Dadurch kann man ein Modell bauen, das vorhersagt, ob ein Projekt erfolgreich sein wird. Ziel dieses Projekts ist es, so ein Modell zu bauen und Kickstarter-Daten allgemein auszuwerten. So könnt ihr möglichen Projektgründern helfen einzuschätzen, ob Kickstarter für sie eine gute Finanzierungsmöglichkeit ist und wie ihre Erfolgschancen stehen.

Daten: [Kickstarter Projects auf Kaggle](https://www.kaggle.com/datasets/kemical/kickstarter-projects).

### Option C: Andere Tabellendaten (Kaggle)

Strukturierte Tabellendaten von echten Firmen mit einem klaren Geschäftsfall. Wählt ein Regressions- oder ein Klassifikationsproblem.

**Regression (stetige Zielvariable):**

- [Zillow Prize: Home Value Prediction](https://www.kaggle.com/competitions/zillow-prize-1): den logarithmischen Fehler zwischen Zillows automatischer Preisschätzung und dem echten Verkaufspreis vorhersagen. Zielvariable: `logerror`.
- [Mercedes-Benz Greener Manufacturing](https://www.kaggle.com/competitions/mercedes-benz-greener-manufacturing): vorhersagen, wie lange ein Auto aufgrund seiner Ausstattung auf dem Prüfstand braucht. Zielvariable: Testdauer (`y`).
- [Santander Value Prediction Challenge](https://www.kaggle.com/competitions/santander-value-prediction-challenge): einen stetigen Kundenwert aus anonymisierten Daten vorhersagen. Zielvariable: `target`.
- [Allstate Claims Severity](https://www.kaggle.com/competitions/allstate-claims-severity): die Kosten von Versicherungsschäden vorhersagen. Zielvariable: `loss`.
- [Expedia Hotel Recommendations](https://www.kaggle.com/competitions/expedia-hotel-recommendations) (Regressionsvariante): die Wahrscheinlichkeit vorhersagen, dass ein Nutzer eine Hotelgruppe bucht.

**Klassifikation (kategoriale Zielvariable):**

- [Porto Seguro Safe Driver Prediction](https://www.kaggle.com/competitions/porto-seguro-safe-driver-prediction): vorhersagen, ob ein Fahrer im nächsten Jahr einen Schaden meldet. Zielvariable: binär (0/1).
- [Santander Customer Transaction Prediction](https://www.kaggle.com/competitions/santander-customer-transaction-prediction): vorhersagen, welche Kunden eine bestimmte Transaktion machen. Zielvariable: binär.
- [Expedia Hotel Recommendations](https://www.kaggle.com/competitions/expedia-hotel-recommendations): einordnen, welche Hotelgruppe ein Nutzer am wahrscheinlichsten bucht. Zielvariable: mehrere Klassen (`hotel_cluster`).
- [Avito Demand Prediction](https://www.kaggle.com/competitions/avito-demand-prediction): vorhersagen, ob eine Anzeige erfolgreich ist (Nachfrage). Zielvariable: Klassifikation.
- [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk): vorhersagen, ob ein Kreditnehmer seinen Kredit nicht zurückzahlt. Zielvariable: binär (`TARGET`).

## Zeitplan und Meilensteine

Das Projekt läuft über vier Tage. Verfolgt euren Fortschritt auf einem Kanban-Board auf GitHub. Wie man das Board einrichtet, steht in [02_kanban_board_DE.md](02_kanban_board_DE.md).

| Meilenstein | Was es ist | Termin |
| --- | --- | --- |
| Milestone 0 | Daten laden (**Data Ingestion**) | Tag 1, 12:00 |
| Milestone 1 | EDA | Tag 2, 12:00 |
| Milestone 2 | Erstes Modell, die Baseline | Tag 3, 12:00 |
| Milestone 3 | Ein Modell mit Fehleranalyse | Tag 4, 12:00 |
| Milestone 4 | Abgabe und Präsentation | Tag 5, 14:00 |

Schreibt für jeden Meilenstein zwei Dinge in das GitHub-Issue:

1. Was erledigt werden muss, damit der Meilenstein fertig ist.
2. Die **Definition of Done**: wie euer Ergebnis aussieht, wenn der Meilenstein fertig ist.

### Beispiel für ein Baseline-Modell (Milestone 1)

*Hinweis: In der Tabelle oben ist die Baseline Milestone 2. Maßgeblich ist die Tabelle.*

Eine Baseline ist das Einfachste, was funktionieren könnte. Sie liefert euch einen Score, den ihr schlagen müsst. Ein Beispiel für ein Projekt zur Betrugserkennung:

- **Wert des Produkts:** betrügerische Transaktionen finden, Geld sparen, Rufschaden vermeiden und Geldwäsche verhindern.
- **Vorhersage:** ob eine Transaktion betrügerisch ist.
- **Evaluationsmetrik:** F1-Score. Wir wollen Verluste durch Betrug möglichst klein halten und gleichzeitig vermeiden, Kunden fälschlich zu beschuldigen (und sie vielleicht zu verlieren). False Positives und False Negatives haben beide starke negative Folgen, darum passt eine ausgewogene Metrik wie der F1-Score.
- **Baseline-Modell:** Wir nehmen an, dass Transaktionen um Mitternacht wahrscheinlich betrügerisch sind.
- **Score:** F1-Score = 0,1.

## Woran ihr denken solltet

Behaltet beim Bauen und Verbessern eurer Modelle diese Punkte im Kopf:

- Prüft, ob die Daten **unausgewogen** sind (**data imbalance**).
- Was ist die richtige Metrik für euer Problem: Precision, Recall, Accuracy, F1-Score oder etwas anderes? (Denkt an die **True Positive Rate**, also den Anteil der gefundenen Positiven.)
- Probiert **mindestens drei verschiedene Machine-Learning-Algorithmen** aus, um zu sehen, welcher am besten ist, jeweils mit **Kreuzvalidierung** und **Hyperparameter-Tuning**.

## Abgabe (Final Deliverables)

1. Ein **Foliensatz** (PDF, auf GitHub hochgeladen) für Stakeholder ohne Technikwissen, der eure Ergebnisse, Empfehlungen und nächsten Schritte zeigt. Er begleitet eine Präsentation von **10 Minuten**.
2. Ein **Jupyter Notebook** nach **PEP 8** (Python-Stilregeln) für ein Data-Science- und Technik-Publikum. Das Notebook sollte gut dokumentiert und **reproduzierbar** sein, einen klaren roten Faden haben und Diagramme enthalten, die eure Ergebnisse stützen. Es soll auf GitHub hochgeladen werden.
3. **Eine Folie** über ein mögliches **Datenprodukt**: Wie könnte man die Vorhersagen nutzen?

## Hilfreiche Quellen

Wenn euer Datensatz unausgewogen ist, sind das gute Startpunkte:

- [8 Tactics to Combat Imbalanced Classes](https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/) (8 Taktiken gegen unausgewogene Klassen)
- [Random Oversampling and Undersampling for Imbalanced Classification](https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/) (zufälliges Über- und Unterabtasten bei unausgewogener Klassifikation)
