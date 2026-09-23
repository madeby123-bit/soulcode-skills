---
name: buch-kapitel
description: Der Riesen-Skill: schreibt oder vertieft ein komplettes Buchkapitel (~18-22 Seiten) in Jennifers Stimme.
---

# Buchkapitel schreiben (Riesen-Skill)

Delegiere an `ghostwriter` (Konsistenzpruefung ueber `lektorin`).

## Regeln
- Buchinnentext: **grosses „Du“**, erzaehlend, warm, KEINE Gedankenstriche.
- Zielumfang ~18-22 Buchseiten (~3500 Woerter) durch echte Substanz.
- Aufbau: **Szene/Geschichte -> Erkenntnis -> Lehre mit Unterabschnitten -> Werkzeug(e)/Uebung(en) -> „Was Du aus diesem Kapitel mitnimmst“ -> Bruecke zum naechsten Kapitel.**
- Vertiefen mit: anonymen Klientinnen-Szenen, Beispielen, Einwaenden, mehreren Uebungen (inkl. „Vertiefung“).

## Fuer „Erlaube es dir“ (bestehendes Buch)
Kanonische Fakten & Kapitel-Kontinuitaet wahren (siehe `lektorin`). Fuer ein NEUES Buch zuerst `/buch-plan`.

## Ins Manuskript
Content in `book_content*.py` (Ordner „Desktop/ECO STOLZ“) einarbeiten, dann bauen via `/buch-build` (`build_pdf.py`/`build_print.py`/`build_book.py`). Kein Node/LibreOffice, nur python3+reportlab+python-docx.
