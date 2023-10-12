---
title: "Markdown Guide"
url: "/markdown-guide"
---

Markdown-Guide für Deine Webseite

# Einführung

Markdown ist eine einfache und intuitive Auszeichnungssprache, die für das Schreiben von Inhalten in Hugo-Webseiten verwendet werden kann. Hugo ist ein statischer Website-Generator, der Markdown-Dateien in HTML umwandelt.

## Überschriften

Verwende  `#` für Überschriften. Je mehr `#`, desto tiefer die Ebene. Zum Beispiel:


```
# Das ist eine Überschrift der Ebene 1

## Das ist eine Überschrift der Ebene 2

### Das ist eine Überschrift der Ebene 3
```

# Das ist eine Überschrift der Ebene 1

## Das ist eine Überschrift der Ebene 2

### Das ist eine Überschrift der Ebene 3

#### Das ist eine Überschrift der Ebene 4

##### Das ist eine Überschrift der Ebene 5  

&nbsp;

## Listen

Unsortierte Liste:
```
- Punkt 1
- Punkt 2
- Punkt 3
```
- Punkt 1
- Punkt 2
- Punkt 3

Sortierte Liste:
```
1. Erster Punkt
2. Zweiter Punkt
3. Dritter Punkt
```

1. Erster Punkt
2. Zweiter Punkt
3. Dritter Punkt

## Textformatierung

Fett: `**fetter Text**`
**fetter Text**

Kursiv: `*kursiver Text*`
*kursiver Text*

Kombiniert: `***fetter kursiver Text***`
***fetter kursiver Text***

Verwende `~~durchgestrichener Text~~` für ~~durchgestrichenen Text~~.

## Zeilenumbruch

In Markdown wird ein einfacher Zeilenumbruch nicht durch bloßes Drücken der "Enter"- oder "Return"-Taste erzeugt. 
Stattdessen benötigst Du zwei Leerzeichen am Ende einer Zeile, um einen Zeilenumbruch zu erzeugen.

Beispiel:
```
Erste Zeile  
Zweite Zeile
```

Das Ergebnis wird sein:
Erste Zeile  
Zweite Zeile

Die beiden Leerzeichen am Ende der ersten Zeile erzeugen den Zeilenumbruch.

## Leere Zeile

Um in Markdown eine leere Zeile zu erzeugen, musst du einfach zweimal die "Enter" oder "Return"-Taste drücken. Das bedeutet, dass du zwischen den zwei Zeilen keinen Text oder Inhalt schreiben sollst. Hier ist ein einfaches Beispiel:

```
Das ist der Text in der ersten Zeile.

Das ist die zweite Zeile, und hier beginnt ein neuer Abschnitt.
```

Das Ergebnis wird sein:

Das ist der Text in der ersten Zeile.

Das ist die zweite Zeile, und hier beginnt ein neuer Abschnitt.

Sollte dies nicht klappen, dann gibt es noch die Möglichkeit eine leere Zeile mit HTML einzufügen.  

HTML Leerzeile: ```&nbsp;```


## Links

Im gleichen Fenster: `[Linktext](http://example.com)`
[Linktext](http://example.com)

Auf Deiner eigenen Seite: `[Linktext](/url)`
[Linktext](/url)

In einem neuen Fenster:
```
{{</* targetblank href="http://example.com" title="Link in neuem Fenster" */>}}
```
{{< targetblank href="http://example.com" title="Link in neuem Fenster" >}}

Externe Links solltest Du immer in einem neuen Fenster öffnen, sonst leitest Du Besucher von Deiner Webseite weg.

## Bilder

```
![Bildbeschreibung](images/bild-url.jpg)
```
Bei Deiner webseite liegen die Bilder im "images" Ordner. Du musst also den Ordnernamen vor den Bildnamen setzen. 

## Horizontale Linien

Eine horizontale Linie wird durch drei aufeinanderfolgende Minuszeichen `---` erstellt.

---

## Zitate

Zitatblock:
```
> Dies ist ein Zitat.
```

> Dies ist ein Zitat.

##### Mehrzeilige Zitate mit Blockzitaten:

```
> Das ist ein Zitat.
> Hier ist eine weitere Zeile im Zitat.

Und hier ist der Name der zitierten Person
```

> Das ist ein Zitat.  
> Hier ist eine weitere Zeile im Zitat.

Und hier ist der Name der zitierten Person

Der direkte Text nach einem Zitat wird rechtsbündig und nahe am Zitat dargestellt. 
Sollte dies nicht gewünscht sein, dann sollte das Zitat von einer linien mit 2 leerzeichen und einem 
 `&nbsp;` und einer Leerzeile gefolgt werden.

```
> Das ist ein Zitat.
> Hier ist eine weitere Zeile im Zitat.
  
&nbsp;

Es gibt keinen Namen der dem Zitat zugeordnet werden soll. 
```

> Das ist ein Zitat.  
> Hier ist eine weitere Zeile im Zitat.
  
&nbsp;

Es gibt keinen Namen, der dem Zitat zugeordnet werden soll.

## Tabellen

Erstellen einer Tabelle mit Spaltenüberschriften und Inhalt. 
Das `|` wird zur Trennung der Spalten verwand.

```
| Spalte 1 | Spalte 2 | Spalte 3 |
|----------|----------|----------|
| Inhalt 1 | Inhalt 2 | Inhalt 3 |
| Inhalt 4 | Inhalt 5 | Inhalt 6 |
```

| Spalte 1 | Spalte 2 | Spalte 3 |
|----------|----------|----------|
| Inhalt 1 | Inhalt 2 | Inhalt 3 |
| Inhalt 4 | Inhalt 5 | Inhalt 6 |



## Fußnoten

Füge Fußnoten hinzu, indem Du `[^1]` für den Verweis und `[^1]: Fußnotentext` für den Fußnotentext verwendest.

```
Das ist ein Text mit einer Fußnote.[^1]

[^1]: Hier ist die Fußnote.
```

Das ist ein Text mit einer Fußnote. Gehe zum Ende der Seite um sie zu sehen. [^1]

[^1]: Hier ist die Fußnote.



## YouTube-Videos

Du kannst YouTube-Videos in deine Seite einbetten:

```
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
```

Ersetze `VIDEO_ID` durch die tatsächliche YouTube-Video-ID.

## Kommentare

Du kannst Kommentare einfügen, die im Text Deiner Webseite nicht angezeigt werden:

```
<!-- Dies ist ein Kommentar und wird nicht angezeigt -->
```
