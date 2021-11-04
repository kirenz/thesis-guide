# Design Science Research

Für die Beantwortung einer Forschungsfrage geht der folgende Abschnitt auf die verwendete wissenschaftliche Vorgehensweise ein, deren Qualität seit jeher unter den Gesichtspunkten zweier zentraler Forschungsparadigmen diskutiert wird: Zum einen bedingt eine hohe Forschungsgüte eine wissenschaftlich fundierte Basis (Rigorosität). Zum anderen müssen aufgegriffener Problemstellung sowie erzielten Forschungsergebnissen reale wie praktische Bedeutung nachzuweisen sein (Relevanz). um diesen Ansprüchen zu genügen, orientiert sich das methodische Vorgehen dieser Arbeit am Design Science Research (DSR), zu Deutsch „Gestaltungsorientierte Forschung“. 76 Die Wurzeln des DSR finden sich in den Ingenieurswissen-


Hevner et. al. zufolge verknüpft der DSR dabei die wissenschaftlichen Ziele der Behavioral Science mit jenen der Design Science. 78 Wohingegen sich Behavioral Science zur Problembeschreibung mit der Entwicklung und Validierung von Theorien befasst, adressiert Design Science die Problemlösung mit der Konstruktion und Evaluation von Artefakten. 79 Auf Grundlage dieser sich gegenseitig befruchtenden Symbiose zielt die Nutzung des DSR darauf ab, mithilfe neuartiger Artefakte unternehmensrelevanten Problemstellungen zu begegnen und so dem Aufzeigen von Lösungswegen wie auch dem theoretischen Wissenszuwachs zuträglich zu sein. 80 Der hierfür propagierte Kreislauf dreier ineinander verwobener Zyklen - Rigorosität, Relevanz und Design – sei als konzeptioneller Ordnungsrahmen verstanden und wie folgt skizziert:

Während der Relevanz-Zyklus die Unternehmensumwelt mit dem Forschungsvorhaben verzahnt und auf diese Weise sowohl die Problemstellung als auch die Anforderungen an das Artefakt spezifiziert, stellt der Rigor-Zyklus sicher, dass die Erstellung des Artefakts unter Berücksichtigung bereits bestehender Wissensbasis erfolgt. 81 Als Herzstück des DSR versteht sich allerdings der Design-Zyklus, dem bei Einbeziehung der in den beiden anderen Zyklen gesammelten Erkenntnisse die kreative wie iterative Konstruktion des Artefakts obliegt. 82 Dabei schließt der Terminus des Artefakts nach Hevner und Chatterjee all jenes vom Menschen künstlich Geschaffene – neben Konstrukten auch Modelle und Methoden – ein, das einem ersten Lösungsansatz für ein relevantes Problem oder der spürbaren Aufwertung einer existierenden Lösung dienlich ist.8

Anforderungskatalog

 Grundmuster einer schrittweisen Verfeinerung 229nach initialer Aufnahme der Geschäftsanforderungen (Business Requirements) die sich daraus erge- benden Implikationen für Daten (Data Requirements), Funktionen (Functional Require- ments) und technischen Unterbau (Technical Requirements) ebenso beleuchtet und do- kumentiert wie bestehende Data Shadow Systeme 230und notwendig werdendes


Die folgende Checkliste soll eine Überprüfung dienen, ob das Vorgehen nach Design Science Research korrekt umgesetzt wurde. Die Fragen orientieren sich an der „Design Science Research Checklist“ nach Hevner & Chatterjee (Hevner & Chatterjee, 2010, S. 20) und den “ACM SIGSOFT Empirical Standards nach Ralph et al. (Ralph, 2020).

1. Was ist die Forschungsfrage (Gestaltungsanforderungen)?
2. Was ist das Artefakt? Wie wird das Artefakt dargestellt?
3. Welche Designprozesse werden für die Gestaltung des Artefakts verwendet?
4. Wie werden das Artefakt und die Designprozesse durch die Wissensbasis fundiert? Welche Theorien
 unterstützen, wenn vorhanden, das Design des Artefakts und den Designprozess?
5. Welche Evaluationen werden während der internen Designzyklen durchgeführt? Welche
 Designverbesserungen werden während jedes Designzyklus identifiziert? Werden die Stärken,
 Schwächen und Grenzen des Artefakts diskutiert?
6. Wie wird das Artefakt in die Anwendungsdomäne eingeführt und wie wird es im Feld getestet? Welche
 Metriken werden verwendet, um den Nutzen des Artefakts und die Verbesserung gegenüber früheren
 Artefakten zu demonstrieren?
7. Werden Alternativen auf Basis des Stands der Technik analysiert? Welches neue Wissen wird der
 Wissensbasis hinzugefügt und in welcher Form (z.B. Veröffentlichung, Meta-Artefakte, neue Theorie,
 neue Methode)?
8. Ist die Forschungsfrage zufriedenstellend beantwortet?



Whether you write your book's content in Jupyter Notebooks (`.ipynb`) or
in regular markdown files (`.md`), you'll write in the same flavor of markdown
called **MyST Markdown**.

## What is MyST?

MyST stands for "Markedly Structured Text". It
is a slight variation on a flavor of markdown called "CommonMark" markdown,
with small syntax extensions to allow you to write **roles** and **directives**
in the Sphinx ecosystem.

## What are roles and directives?

Roles and directives are two of the most powerful tools in Jupyter Book. They
are kind of like functions, but written in a markup language. They both
serve a similar purpose, but **roles are written in one line**, whereas
**directives span many lines**. They both accept different kinds of inputs,
and what they do with those inputs depends on the specific role or directive
that is being called.

### Using a directive

At its simplest, you can insert a directive into your book's content like so:

````
```{mydirectivename}
My directive content
```
````

This will only work if a directive with name `mydirectivename` already exists
(which it doesn't). There are many pre-defined directives associated with
Jupyter Book. For example, to insert a note box into your content, you can
use the following directive:

````
```{note}
Here is a note
```
````

This results in:

```{note}
Here is a note
```

In your built book.

For more information on writing directives, see the
[MyST documentation](https://myst-parser.readthedocs.io/).


### Using a role

Roles are very similar to directives, but they are less-complex and written
entirely on one line. You can insert a role into your book's content with
this pattern:

```
Some content {rolename}`and here is my role's content!`
```

Again, roles will only work if `rolename` is a valid role's name. For example,
the `doc` role can be used to refer to another page in your book. You can
refer directly to another page by its relative path. For example, the
role syntax `` {doc}`intro` `` will result in: {doc}`intro`.

For more information on writing roles, see the
[MyST documentation](https://myst-parser.readthedocs.io/).


### Adding a citation

You can also cite references that are stored in a `bibtex` file. For example,
the following syntax: `` {cite}`holdgraf_evidence_2014` `` will render like
this: {cite}`holdgraf_evidence_2014`.

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

````
```{bibliography}
```
````

Resulting in a rendered bibliography that looks like:

```{bibliography}
```


### Executing code in your markdown files

If you'd like to include computational content inside these markdown files,
you can use MyST Markdown to define cells that will be executed when your
book is built. Jupyter Book uses *jupytext* to do this.

First, add Jupytext metadata to the file. For example, to add Jupytext metadata
to this markdown page, run this command:

```
jupyter-book myst init markdown.md
```

Once a markdown file has Jupytext metadata in it, you can add the following
directive to run the code at build time:

````
```{code-cell}
print("Here is some code to execute")
```
````

When your book is built, the contents of any `{code-cell}` blocks will be
executed with your default Jupyter kernel, and their outputs will be displayed
in-line with the rest of your content.

For more information about executing computational content with Jupyter Book,
see [The MyST-NB documentation](https://myst-nb.readthedocs.io/).
