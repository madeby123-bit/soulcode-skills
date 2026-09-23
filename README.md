# Soul Code Skills

Meine Sammlung an **Skills** und **Assistenten** für Claude, gebaut für spirituelle Coaches, Beraterinnen, Heilerinnen und alle, die ihr Business selbst aufbauen.

Ein **Skill** ist eine Anleitung, die Claude automatisch lädt, sobald sie zu deiner Aufgabe passt. Du musst nichts auswendig lernen. Du schreibst, was du brauchst, und Claude weiß, wie es geht.

Ein **Assistent** ist eine Rolle mit eigenem Wissen, zum Beispiel eine Texterin, eine SEO-Fachfrau oder ein Business-Coach. Du sprichst ihn direkt an, und er arbeitet in seinem Fachgebiet für dich.

Von Jennifer Gräser, [Soul Code Marketing](https://www.soulcode-marketing.de).

---

## Was drin ist

| Ordner | Inhalt |
|---|---|
| `skills/` | 65 deutschsprachige Skills, von mir gebaut |
| `agents/` | 16 Assistenten mit eigenem Fachgebiet |
| `marketing-skills-englisch/` | 49 englische Marketing-Skills aus einem fremden Projekt, MIT-lizenziert, siehe `HERKUNFT.md` in dem Ordner |

---

## Einbauen

Du brauchst **Claude Code**. Die Anleitung zur Installation steht unter https://docs.claude.com/claude-code.

### Alles auf einmal

Öffne das Terminal und gib das hier ein:

```bash
git clone https://github.com/madeby123-bit/soulcode-skills.git
cp -R soulcode-skills/skills/* ~/.claude/skills/
cp -R soulcode-skills/agents/* ~/.claude/agents/
```

Die englischen Marketing-Skills kommen nur mit, wenn du sie willst:

```bash
cp -R soulcode-skills/marketing-skills-englisch/*/ ~/.claude/skills/
```

### Ohne Terminal

Klick oben rechts auf den grünen Knopf **Code** und dann auf **Download ZIP**. Entpacke die Datei und kopiere die Ordner `skills` und `agents` in deinen Ordner `~/.claude/`. Den findest du im Finder über **Gehe zu → Gehe zum Ordner** und der Eingabe `~/.claude`.

### Prüfen, ob es geklappt hat

Starte Claude Code neu und tippe `/`. Dann sollten die Skills in der Liste auftauchen.

---

## Wie du sie benutzt

**Skills** starten von selbst, sobald sie passen. Du kannst sie auch direkt aufrufen, etwa `/blogartikel` oder `/ig-reel`.

**Assistenten** sprichst du an, indem du sagst, wen du brauchst: „Frag die SEO-Managerin, wie ich für diesen Begriff ranke" oder „Lass die Ghostwriterin einen Newsletter schreiben".

---

## Die Skills im Überblick

| Aufruf | Wofür |
|---|---|
| `/ad-budget` | Gibt Empfehlungen zu Budget-Aufteilung und Skalierung von Kampagnen. |
| `/ad-creative` | Entwickelt Creative-Konzepte/Angles fuer Ads (Bild-/Video-Ideen pro Winkel). |
| `/ad-test` | Erstellt einen sauberen A/B-Test-Plan (eine Variable pro Test) fuer Anzeigen. |
| `/ad-zielgruppe` | Definiert Ad-Targeting: Interessen, Lookalikes, Custom Audiences, Ausschluesse. |
| `/ai-reel` | Erstellt ein komplett neues KI-Avatar-Reel mit Jennifers geklonter Stimme und Aussehen via HeyGen. Nutzen wenn Jennifer ein neues Reel will, das sie N |
| `/angebot` | Entwickelt ein verkaufbares Angebot mit dem Angebots-Baukasten (Name/Versprechen/Form/Preis). |
| `/audio-clean` | Saeubert Video-Audio mit ffmpeg: Lautheit normalisieren und lange Stillen kuerzen. |
| `/b-roll` | Erstellt eine Schnitt-/B-Roll-Liste zu einem Skript (welche Bilder/Clips wann). |
| `/bio-optimieren` | Optimiert das Instagram-/TikTok-Profil: Name, Bio, Highlights, Link. |
| `/blogartikel` | Schreibt einen SEO-optimierten Blogartikel mit Struktur, Keyword und CTA. |
| `/brand-voice` | Zentrale Referenz fuer Jennifers Markenstimmen (Buch vs. Marketing). Von allen Content-Skills genutzt. |
| `/buch-kapitel` | Der Riesen-Skill: schreibt oder vertieft ein komplettes Buchkapitel (~18-22 Seiten) in Jennifers Stimme. |
| `/buch-plan` | Entwickelt Konzept und Detail-Gliederung fuer ein neues Buch (Titel, Versprechen, Kapitel). |
| `/caption-cta` | Formuliert starke Call-to-Actions und Caption-Schluesse in mehreren Varianten. |
| `/captions-style` | Definiert und wendet Untertitel-Styles im CapCut-Look an (Farbe, Groesse, Position, Marke). |
| `/content-batch` | Produziert einen kompletten Wochen-Content-Batch (mehrere Posts fertig) und legt sie postbereit ab. |
| `/content-plan` | Erstellt einen Redaktionsplan/Content-Kalender fuer einen Zeitraum ueber alle Kanaele. |
| `/cut-clip` | Schneidet mit ffmpeg einen Abschnitt aus einem Video (Start/Ende), verlustfrei oder neu kodiert. |
| `/dashboard` | Zeigt und aktualisiert das Marketing-Dashboard: Ziele, KPIs, 90-Tage-Fortschritt, Content-Queue, naechste Schritte. |
| `/funnel` | Baut einen kompletten Marketing-Funnel (Aufmerksamkeit -> Vertrauen -> Angebot) mit Assets pro Stufe. |
| `/google-ad` | Schreibt Google-Search-Ads (Responsive Search Ad: Headlines + Descriptions). |
| `/growth-plan` | Erstellt einen 90-Tage-Marketing-Wachstumsplan mit Zielen, Phasen und Wochen-Tasks. Nutzen fuer Strategie/Planung von Grund auf. |
| `/growth-track` | Verfolgt den Fortschritt des 90-Tage-Plans, traegt neue Zahlen ein und gibt die naechsten Schritte. Woechentlicher Check-in. |
| `/hashtags` | Stellt gezielte Hashtag-Sets fuer die Zielgruppe zusammen (Mix aus Groessen). |
| `/highlight-finder` | Findet aus einem Transkript die staerksten Kurz-Clips (Hook/Aha/Emotion) als Short-Kandidaten. |
| `/hook-cut` | Baut einen packenden Eroeffnungs-Schnitt fuer die ersten Sekunden (Pattern-Interrupt). |
| `/hooks` | Liefert eine Hook-Bibliothek: viele Scroll-Stopper-Erstzeilen fuer ein Thema. |
| `/humanizer` | | |
| `/ig-karussell` | Erstellt ein Instagram-Karussell Slide fuer Slide (Hook-Slide bis CTA-Slide). |
| `/ig-post` | Schreibt einen Instagram-Feed-Post: Hook, Caption, CTA, Hashtags. |
| `/ig-reel` | Schreibt ein Instagram-Reel-Skript (Hook, gesprochener Text, On-Screen-Text, CTA). |
| `/ig-story` | Schreibt eine Instagram-Story-Sequenz mit Interaktion (Umfrage/Frage/Slider). |
| `/insta` | Instagram-Content für Jennifers Zielgruppe spiritueller Frauen/Coaches erstellen (Caption, Reel-Skript, Karussell, Hook-Ideen). Nutzen wenn Jennifer S |
| `/ki-rat` | > |
| `/kpi` | Definiert die richtigen KPIs und Startwerte fuers Tracking und traegt sie ins Dashboard ein. |
| `/landingpage-ad` | Schreibt eine Landingpage passend zu einer Anzeige (Message-Match, ein Ziel). |
| `/launch` | Plant einen Produkt-/Angebots-Launch (z.B. Kurs, Buch, Coaching) mit Phasen und Content. |
| `/lead-magnet` | Entwirft ein Freebie/Lead-Magnet mit schnellem Ergebnis und Bruecke zum Angebot. |
| `/lektorat` | Lektoriert Text: Konsistenz, Ton, Rechtschreibung, grosses/kleines Du, keine Gedankenstriche. |
| `/meta-ad` | Schreibt Meta- (Facebook/Instagram) Werbeanzeigen-Copy mit mehreren Angles. |
| `/newsletter` | Schreibt eine E-Mail / einen Newsletter: eine Story, ein Gedanke, ein CTA. |
| `/positionierung` | Schaerft Positionierung und USP: wofuer steht Soul Marketing, was macht es einzigartig, klare Botschaft. |
| `/retargeting` | Baut eine Retargeting-Sequenz fuer warme Zielgruppen (Viewer/Besucher/Warenkorb). |
| `/security-audit` | Security audit of a codebase — web apps, APIs, services, CLI tools, libraries, daemons, and more. Use when asked to find security bugs, do a security  |
| `/short-aus-video` | Erstellt aus einem Langvideo einen 9:16-Short: Abschnitt schneiden, auf 1080x1920 bringen, Untertitel einbrennen. |
| `/thumbnail-frame` | Extrahiert mit ffmpeg einen Einzelframe aus einem Video als Thumbnail-Bild. |
| `/tiktok-ad` | Schreibt ein TikTok-Ad-Skript im nativen Creator-Stil (Spark-Ad-tauglich). |
| `/tiktok-skript` | Schreibt ein TikTok-Skript im nativen, ungeschliffenen Stil mit starkem Hook. |
| `/tiktok-trend` | Adaptiert einen aktuellen TikTok-Trend/Sound auf Jennifers Thema und Marke. |
| `/ugc-brief` | Erstellt ein Creator-/UGC-Brief fuer Content, den andere fuer die Marke produzieren. |
| `/untertitel` | Erzeugt Untertitel (.srt) aus einem Video per Whisper-Transkription (Deutsch). |
| `/untertitel-burn` | Brennt Untertitel im CapCut-Stil fest ins Video ein (grosse fette weisse Schrift mit Outline). |
| `/verkaufsseite` | Schreibt eine komplette Verkaufsseite / ein VSL-Skript nach bewaehrter Struktur. |
| `/wettbewerb` | Analysiert Wettbewerber/Vorbilder im spirituellen Coaching-Markt und findet Luecken. |
| `/yt-beschreibung` | Schreibt eine SEO-optimierte YouTube-Videobeschreibung mit Keywords, Links und Kapiteln. |
| `/yt-community` | Schreibt YouTube-Community-Posts / Umfragen zur Bindung zwischen Videos. |
| `/yt-hook` | Schreibt starke Video-Hooks fuer die ersten 15 Sekunden (Lang) bzw. 2 Sekunden (Short). |
| `/yt-kapitel` | Erstellt YouTube-Kapitelmarken (Timecodes) aus einem Skript oder Transkript. |
| `/yt-seo` | Fuehrt einfache YouTube-Keyword-Recherche durch und liefert Tags/Suchbegriffe. |
| `/yt-serie` | Plant eine YouTube-Content-Serie / Playlist-Strategie fuer nachhaltiges Wachstum. |
| `/yt-short` | Schreibt ein YouTube-Shorts- oder Reel-Skript unter 60 Sekunden im 9:16-Format. |
| `/yt-thumbnail` | Entwirft Thumbnail-Konzepte (Bildidee, Gesichtsausdruck, Text-Overlay, Farben). |
| `/yt-titel` | Optimiert YouTube-Titel auf hohe Klickrate (CTR) mit mehreren Varianten. |
| `/yt-video` | Schreibt ein komplettes YouTube-Langvideo-Skript (8-15 Min) inkl. Packaging (Titel/Thumbnail) und Ableitungen. |
| `/zielgruppe` | Erstellt eine praezise Zielgruppen-/Wunschkundin-Analyse (Avatar) mit Schmerz, Sehnsucht, Sprache, Einwaenden. |

---

## Die Assistenten

| Assistent | Wofür |
|---|---|
| **ad-manager** | Performance-Marketing-Manager für bezahlte Werbung auf Meta (Facebook/Instagram), TikTok und Google. Nutzen für Ad-Copy, Creative-Konzepte, Targeting, |
| **businessaufbau** | Experte für Businessaufbau für spirituelle Frauen und selbstständige Unternehmerinnen. Nutzen für Geschäftsmodell, Angebote und Preise, Positionierung |
| **dashboard** | Marketing-Dashboard und Growth-Analyst. Nutzen um den Marketing-Status, KPIs, den 90-Tage-Plan-Fortschritt und die nächsten Aufgaben zu sehen und zu a |
| **ghostwriter** | Ghostwriter, Lektor und Content-Autor für Jennifer. Der Riesen-Skill fürs Schreiben — Bücher, weitere Kapitel, Lektorat, Blogartikel, Newsletter, Lead |
| **manifestation-weiblich** | Experte für Manifestation in Weiblichkeit für Jennifer und ihre Zielgruppe. Nutzen für Manifestations-Arbeit, weibliche Energie, anziehen statt jagen, |
| **mindset-energie** | Experte für Mindset und Energie für Jennifer und ihre Zielgruppe spiritueller Frauen. Nutzen für Money-Mindset und Selbstwert, Ängste und Blockaden, F |
| **online-marketing** | Experte für Online Marketing für Jennifers Zielgruppe spiritueller Frauen und Coaches. Nutzen für Marketing-Strategie, Funnel, E-Mail-Marketing, Ads-G |
| **persoenlichkeit** | Experte für Persönlichkeitsentwicklung für Jennifer und ihre Zielgruppe spiritueller Frauen. Nutzen für persönliches Wachstum, Selbstwert, Glaubenssät |
| **seo-manager** | SEO- & ClickRank-Manager für Jennifers Websites. Nutzen für On-Page-SEO, ClickRank-Verwaltung, Meta-Tags/Titel/Descriptions, Keywords, Schema, Alt-Tex |
| **sichtbarkeit** | Experte für Sichtbarkeit für spirituelle Frauen und Coaches. Nutzen für Sichtbarkeits-Strategie, den Mut sich zu zeigen, Personal Branding, Positionie |
| **social-content** | Social-Media-Content-Creator für Instagram, TikTok, Reels und Karussells. Nutzen für Captions, Reel-/TikTok-Skripte, Karussell-Slides, Stories, Hooks, |
| **spirit-copy** | Marketing-Texterin für Jennifers Agentur Soul Marketing (spirituelle Berater, Heiler, Coaches). Nutzen für Website-Texte, Landingpages, Newsletter, Ve |
| **strategist** | Online-Marketing-Stratege für Jennifers Agentur Soul Marketing. Nutzen für Strategie, Positionierung, Zielgruppe, Funnel, 90-Tage-Wachstumsplan und de |
| **video-cutter** | Video-Cutter mit eingebrannten Untertiteln im CapCut-Stil. Nutzen zum Schneiden von Videos, Erstellen von Shorts/Reels aus Langvideos, Untertitel gene |
| **youtube-producer** | YouTube-Produzent für Jennifer — Langvideos UND Shorts. Nutzen für Video-Ideen, Skripte, Titel, Thumbnails, Beschreibungen, YouTube-SEO und Serien-Pla |
| **youtube-social** | Experte für YouTube und Social Media Marketing für spirituelle Frauen und Coaches. Nutzen für Content-Strategie über YouTube, Instagram, TikTok, Reels |

---

## Lizenz und Nutzung

Die Inhalte in `skills/` und `agents/` stammen von mir. Du darfst sie für deine eigenen Projekte und dein eigenes Business frei nutzen und anpassen. Siehe `LIZENZ.md`.

Die Inhalte in `marketing-skills-englisch/` stammen von jemand anderem und stehen unter der MIT-Lizenz. Herkunft und Lizenztext liegen in dem Ordner.

---

## Fragen

Schreib mir über [soulcode-marketing.de/kontakt](https://www.soulcode-marketing.de/kontakt/).
