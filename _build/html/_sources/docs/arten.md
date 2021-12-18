# Arten wissenschaftlicher Arbeiten

Bei der Erstellung einer wissenschaftlichen Arbeit kann zwischen verschiedenen Arten unterschieden werden. Bitte beachten Sie, dass lediglich Arbeiten der folgenden Art betreut werden:

- Erstellung einer technologischen Lösung (bspw. im Bereich Machine Learning, Analytics, Data Engineering, Dashboards, ...): `Design Science Research Methode`.

- Erstellung eines statistischen Modells und/oder Prüfung von Hypothesen (bspw. im Rahmen eines A/B-Tests): `Quantitative empirische Arbeit`.

Unten finden Sie Hinweise zu den beiden Arten.

## Hinweise zu Kooperationen

Unabhängig von der Art der wissenschaftlichen Arbeit besteht jeweils die Möglichkeit, diese in **Kooperation mit einem Unternehmen** zu verfassen. Bei einer Kooperation wird von Seiten des Unternehmens typischerweise eine spezifische Fragestellung formuliert, die im Rahmen der wissenschaftlichen Arbeit bearbeitet werden soll. In diesem Fall eignt sich in der Regel die Anwendung der `Design Science Research Methode`.

Wichtige Hinweise zu Arbeiten mit Unternehmen:

- Die theoretische Fundierung der Arbeit ist auch im Rahmen einer Kooperation zwingend erforderlich (Literaturanalyse etc.).
- Eine Verallgemeinerbarkeit über das behandelte Unternehmen hinaus muss gegeben sein.

## Design Science Research

Sollen im Rahmen der Arbeit mit Hilfe von Technologien (bspw. Python, R, Open Source Software, Microsoft Power BI, ...) Lösungen für eine bestimmte Fragestellung erstellt werden, eignet sich die Verwendung der Desing Science Research Methode (DSRM), die auch als "gestaltungsorientierte Forschung" bezeichnet wird (im Kontext der DSRM werden Lösungen als "Artefakte" bezeichnet). 

Hevner et. al. (2004) zufolge besteht die Zielsetzung des DSRM darin, mithilfe neuartiger Artefakte unternehmensrelevanten Problemstellungen zu lösen und gleichzeitig durch deren systematischer Dokumentation dem theoretischen Wissenszuwachs zuträglich zu sein. Der hierfür konzipierte  Kreislauf dreier Zyklen - Rigorosität, Relevanz und Design – ist als konzeptioneller Ordnungsrahmen zu verstehen (Hevner, 2007): 

```{image} ../_static/img/dsrm-cycles.png
:alt: dsrm
:class: bg-primary mb-1
:width: 600px
:align: center
```

- Relevanz-Zyklus: Unternehmensumwelt wird mit dem Forschungsvorhaben verzahnt und auf diese Weise sowohl die Problemstellung als auch die Anforderungen an die Artefakte spezifiziert. Ein Artefakt kann dabei eine Technologie, eine Methode, ein Modell ect. darstellen. 

- Rigor-Zyklus: Erstellung des Artefakts unter Berücksichtigung bereits bestehender Wissensbasis (Literatur, Best Practice Ansätze). 
  
- Design-Zyklus: Erstellung der Artefakte (Modelle, Methoden, ... ) unter Einbeziehung der in den beiden anderen Zyklen gewonnenen Erkenntnisse.  8

Peffers et al. (2007) überführten die Zyklen in einen Prozess, der in der nachfolgenden Abbildung dargestellt ist. In dieser ist der Prozess der DSRM für ein Beispiel, in welchem ein Data Warehouse entwickelt werden soll, dargestellt:

```{image} ../_static/img/dsrm-process.png
:alt: dsrm
:class: bg-primary mb-1
:width: 600px
:align: center
```

<br>

Die Vorgehensweise folgt typischerweise diesem Schema:

1. Beschreibung der Problemstellung und Motivation
2. Recherche und Aufarbeitung der relevanten Literatur (Theorien, Best Practice Ansätze, State of the Art Ansätze)
3. Definition der Zielsetzung und Erstellung eines Anforderungskatalogs (was ist der gewünschte Funktionsumfang der Artefakte?)
4. Design und Entwicklung der Artefakte
5. Demonstration und Evaluation der Artefakte
6. Kommunikation (optional)

```{admonition} Literatur
:class: tip

- [Process of Design Science Research Methodology (Peffers et al., 2007)](https://drive.google.com/file/d/1gZPittSxfb1t5AM2lBVPOW4tr_FLZxdn/view?usp=sharing)

- [Design Science Research Guidelines (Hevner et al., 2004)](https://drive.google.com/file/d/1CC7Q-4avgoS7Z1SreuM_Jz5tuat6rjNt/view?usp=sharing)

- [A Three Cycle View of Design Science Research (Hevner, 2007)](https://drive.google.com/file/d/1Ocy0UkjFSEyeiI4RVvBbQc2P1pxNuzEZ/view?usp=sharing)

```

## Quantitative empirische Arbeit: Prüfung von Hypothesen

Im Rahmen einer quantitativen empirischen Arbeit werden mit Hilfe von Daten und Analysen Hypothesen untersucht. In diesem Zusammenhnang können auch statistische Modelle wie die Regression oder Klassifikation zum Einsatz kommen.

Die Vorgehensweise folgt typischerweise diesem Schema:

1. Beschreibung der Problemstellung und Zielsetzung
2. Darstellung der relevanten Grundlagen
3. Recherche und Aufarbeitung der relevanten Literatur
4. Formulierung von Hypothesen (id.R. 2 bis 5)
5. Definition der erforderlichen Stichprobe und Daten (für die Prüfung der Hypothesen)
6. Erhebung der Daten (bspw. mittels Umfrage, Experiment oder quantitativer Inhaltsanalyse mittels Web-Scraping oder mit API's)
7. Deskriptive Analysen
8. Prüfung der Hypothesen und/oder Erstellung eines Modells
9. Interpretation der Ergenisse
10. Fazit