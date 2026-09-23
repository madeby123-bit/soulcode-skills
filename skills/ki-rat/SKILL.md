---
name: ki-rat
description: >
  Der KI-Rat. Nutzen für wichtige Entscheidungen, Strategiefragen oder den
  Feinschliff eines wichtigen Textes. Mehrere unabhängige Experten-Perspektiven
  beantworten die Frage, bewerten sich gegenseitig anonym, ein Vorsitzender zieht
  ein klares Fazit. Aufruf zum Beispiel: "frag den KI-Rat", "KI-Rat: soll ich ...",
  "lass den Rat über diesen Text schauen". Inspiriert von Andrej Karpathys llm-council.
license: MIT
compatibility: any-agent
allowed-tools:
  - Agent
  - Read
  - Write
  - WebSearch
  - WebFetch
---

# Der KI-Rat

Ein Beratungsgremium für dich. Statt einer einzelnen Antwort lässt du mehrere
unabhängige Perspektiven auf die Frage schauen, gegeneinander abwägen und am Ende
ein klares Fazit ziehen. Gut für Entscheidungen, Strategie, Positionierung und den
Feinschliff wichtiger Texte.

## Wann einsetzen

- Wichtige Entscheidung mit mehreren Optionen (Preis, Angebot, Ausrichtung).
- Strategiefrage, bei der eine Meinung zu wenig ist.
- Ein wichtiger Text (Verkaufsseite, Buchkapitel, Newsletter), der den letzten Schliff braucht.

Für Kleinkram nicht nötig, da reicht eine normale Antwort.

## Die drei Stufen

### Stufe 1: Die Ratsmitglieder antworten unabhängig

Wähle 3 bis 5 Perspektiven, die zur Frage passen. Jede antwortet für sich, ohne die
anderen zu kennen. Nutze für echte Unabhängigkeit den Agent-Tool und lass die Mitglieder
parallel laufen, oder spiele sie sauber getrennt nacheinander durch.

Passende Ratsmitglieder je nach Frage:
- **Die Strategin:** denkt in Positionierung, Zielgruppe, langfristigem Wachstum.
- **Die Verkäuferin:** denkt in Conversion, Angebot, Preis, Kaufpsychologie.
- **Die Skeptikerin:** sucht die Schwachstelle, das Risiko, den übersehenen Haken.
- **Die Zielkundin:** die spirituelle Frau, die kauft oder eben nicht. Was fühlt sie?
- **Die Markenhüterin:** passt das zur eigenen Stimme, warm, kleines "du", echt?
- **Die Zahlenfrau:** was ist realistisch, was kostet es, was bringt es?

Wähle die Mitglieder passend zur Frage. Bei einem Text zum Beispiel: Zielkundin,
Markenhüterin, Skeptikerin, plus eine Lektorin.

### Stufe 2: Peer-Review, anonym

Lege alle Antworten anonym nebeneinander (Mitglied A, B, C, ohne Rollennamen). Jedes
Ratsmitglied bewertet jetzt die anderen Antworten nach Stärke und Ehrlichkeit und benennt
die beste Idee und die größte Schwäche. Niemand bewertet sich selbst. So verhinderst du,
dass eine laute Meinung gewinnt statt der besten.

### Stufe 3: Die Vorsitzende zieht das Fazit

Eine letzte Instanz, die Vorsitzende, liest alle Antworten und Bewertungen und liefert:

1. **Klare Empfehlung** in ein bis zwei Sätzen. Nicht die diplomatische, die echte.
2. **Warum**, die 2 bis 3 stärksten Gründe.
3. **Der Haken**, das größte Risiko oder der wichtigste Vorbehalt.
4. **Nächster Schritt**, eine konkrete Handlung.

## Regeln

- Echte Meinungsvielfalt, nicht dieselbe Antwort in fünf Farben. Die Mitglieder dürfen
  sich widersprechen.
- Ehrlich vor höflich. Die Skeptikerin muss wirklich stechen.
- Am Ende steht eine klare Empfehlung, kein "kommt drauf an".
- Kein langer Strich in der Ausgabe.
  Doppelpunkt, Komma oder Punkt.
- Nach einer wichtigen Rats-Sitzung das Ergebnis als Karteikarte in Obsidian speichern
  (passender Projektordner in den eigenen Notizen).

## Ausgabeformat

```
## Die Frage
[kurz]

## Stimmen aus dem Rat
- Strategin: [Kernaussage]
- Verkäuferin: [Kernaussage]
- Skeptikerin: [Kernaussage]
- [weitere]

## Wo sich der Rat einig war / uneinig war
[kurz]

## Fazit der Vorsitzenden
Empfehlung: [klar]
Warum: [Gründe]
Der Haken: [Risiko]
Nächster Schritt: [konkret]
```
