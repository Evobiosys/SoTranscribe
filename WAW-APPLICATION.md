# WAW Innovation Funding Application — SoTranscribe

**Submission deadline**: 30. April 2026, 23:59 Vienna
**Project entity**: SoTranscribe GmbH (in Gründung)
**Project value**: € 60,000
**Requested grant**: € 42,000 (Base 27,000 + Frauenbonus 10,000 + Gründungsbonus 5,000)
**Project duration**: 1. September 2026 – 31. August 2027 (12 months)
**Co-Projektleitung**: Katherine Colquitt + Jakob Possert-Bienzle

---

## 0. Eckdaten / Project basics

```
Projekttitel:    SoTranscribe — souveräne Audio-Transkription
                 mit Hosting in Österreich und Open-Source-Pipeline
Antragstellerin: SoTranscribe GmbH (in Gründung)
                 Sitz: Wien, Österreich
Projektzeitraum: 01.09.2026 – 31.08.2027 (12 Monate)
Projektkosten:   € 60.000,–
Beantragte Förderung: € 42.000,– (€ 27.000 Basis + € 10.000 Frauenbonus
                                  + € 5.000 Gründungsbonus)

Co-Projektleitung:
  Katherine Colquitt (Co-Projektleiterin, Commercial Lead, 26% Anteil)
  Jakob Possert-Bienzle (Co-Projektleiter, Technical Lead, 74% Anteil)
```

---

## 1. Projektfinanzierung

```
Zu finanzierende Gesamtprojektkosten (excl. Gemeinkosten):  60.000,00 €
─────────────────────────────────────────────────────────
Kassa und Bankguthaben:                                          0,00 €
Eigenmittelzufuhr (USDC-Liquidation):                        5.000,00 €
Cashflow (Beta-Erlöse während Projektlaufzeit):              9.000,00 €
Kurzfristige Kredite (Privatdarlehen Familie):               4.000,00 €
Langfristige Kredite:                                            0,00 €
Akonto Wirtschaftsagentur (50% von 42.000):                 21.000,00 €
Andere öffentliche Zuschüsse:                                    0,00 €
Sonstiges (Restförderung WAW nach Endabrechnung):           21.000,00 €
─────────────────────────────────────────────────────────
Summe:                                                      60.000,00 €

ZUSÄTZLICH ANGESTREBT (außerhalb dieses Antrags):
  ~15.000 € weitere Förderungen aus Sustainability- und
  Sovereignty-Initiativen (NGI Zero Commons Fund, Open Collective,
  KLIEN-Klimaschutz). Werden separat beantragt; nicht Teil dieser
  Finanzierung.
```

---

## 2. Sachkosten / Project costs breakdown

```
EXTERNE DIENSTLEISTUNGEN:                              10.000 €
  Steuer-/Rechtsberatung GmbH-Gründung                  3.000 €
  Sicherheits-Audit der Pipeline                        2.000 €
  Notarkosten Gesellschaftsvertrag                      1.500 €
  Compliance-Beratung (DSGVO, Markenrecht EUIPO)        1.500 €
  Web-Design + Infrastructure Setup                     1.500 €
  Sonstige Beratung                                       500 €

INVESTITIONSKOSTEN MATERIELL/IMMATERIELL:              18.000 €
  Custom Linux-Workstation (Threadripper + RTX 4090,    4.500 €
    R&D + Inferenz-Validierung)
  Server-Hardware für Anexia-Kolokation Klagenfurt
    (1U mit RTX 4090, ECC RAM, redundant PSU)            4.500 €
  Mac Mini M4 64GB (Apple Silicon Validierung)          2.500 €
  RISC-V Dev-Kits (HiFive Premier P550 + Milk-V Megrez
    + DC-ROMA AI PC, Multi-Architektur-R&D)              1.500 €
  Intel Mini-PC NUC (Compatibility Test)                  800 €
  Hallenmiete-Setup für Kolokation
    (Racks, Verkabelung, Cooling, einmalig)             2.500 €
  Camera-Readout-Sicherheits-Forschungsrig               1.000 €
  Misc Hardware (Adapter, Kabel, ECC RAM-Module)           700 €

SACH- UND MATERIALKOSTEN:                               5.000 €
  Nitrokey-Phone (sovereign GrapheneOS-Phone)           1.000 €
  Pixel 10 Pro Fold (mod für Mikrofonloss-Test)         2.000 €
  Audio-Hardware (Mikrofone, Wearables, Test-Captures)  1.000 €
  Sonstige Sachkosten / Verbrauchsmaterial              1.000 €

BAULICHE MAßNAHMEN:                                         0 €

PERSONALKOSTEN:                                        18.000 €
  Jakob Possert-Bienzle: 312h × € 41,67/h              13.000 €
  Katherine Colquitt: 120h × € 41,67/h                  5.000 €
  (Stundensatz nach WAW-Pauschalierung: € 41,67/h)
+ GEMEINKOSTENZUSCHLAG (20% auf Personalkosten):        3.600 €

(Restbudget für Kontingenz / Buffer:                    5.400 €)

─────────────────────────────────────────────
SUMME ANERKANNTE PROJEKTKOSTEN:                        60.000 €
```

---

## 3. Arbeitspakete (8 packages)

### AP1 — Pipeline Engineering: Whisper + pyannote-Integration
- **Stunden**: Jakob 80h | Katherine 0h
- **Inhalte**: Integration faster-whisper (CTranslate2), pyannote.audio, FFmpeg-Vorverarbeitung, Rust-Backend, React-Frontend.
- **Ziele**: Funktionierende End-to-End-Pipeline mit Akkuratheit äquivalent zu Whisper Large v3 Referenz; >90% Test-Coverage.
- **Verifizierbar**: Public GitHub-Repo mit grünen CI-Builds, Benchmark-Report.
- **Abhängigkeiten**: keine (Erstphase).

### AP2 — Hosting-Infrastruktur Österreich
- **Stunden**: Jakob 80h | Katherine 0h
- **Inhalte**: Kolokation in Anexia Klagenfurt (Österreich); Hardware-Aufstellung; Encrypted Storage; Monitoring; SLA-Setup.
- **Ziele**: Standort operativ; SLA 99,5% verfügbar; öffentliche Status-Page live.
- **Verifizierbar**: Public Uptime-Status-Page; Traffic-Logs.
- **Abhängigkeiten**: AP1 muss laufen.

### AP3 — Open-Source-Release + Dokumentation
- **Stunden**: Jakob 60h | Katherine 0h
- **Inhalte**: 1.0-Release unter EvoBioSys-Lizenz / MPL-2.0; User-Docs; Contribution Guide; Self-Host Tutorial.
- **Ziele**: GitHub-Release Tag 1.0; Dokumentation auf sotranscribe.com.
- **Verifizierbar**: Release-Tag, Docs-Pages live.
- **Abhängigkeiten**: AP1.

### AP4 — Hardware-Kompatibilitäts-R&D (Multi-Architektur)
- **Stunden**: Jakob 30h | Katherine 0h
- **Inhalte**: Pipeline-Validierung auf Apple Silicon (Mac Mini M4), Intel-Mini-PC, RISC-V (HiFive Premier P550, Milk-V Megrez, DC-ROMA). Performance-Benchmarks pro Architektur.
- **Ziele**: Mind. 3 Architekturen erfolgreich validiert; öffentlicher Benchmark-Bericht.
- **Verifizierbar**: Benchmark-Report auf sotranscribe.com/advanced.
- **Abhängigkeiten**: AP1.

### AP5 — Old-Laptop-Recovery-Programm (USP)
- **Stunden**: Jakob 30h | Katherine 20h
- **Inhalte**: Rechtliche AGB für Hardware-Tausch-Modell; Intake-Prozess; erste Geräte-Annahme und Integration in Kolokation; Renewable-Energy-Pairing.
- **Ziele**: Signierte AGB; mindestens 5 angenommene Geräte; Klimaimpact-Bericht erste Tonne CO₂eq.
- **Verifizierbar**: AGB-Dokument; Hardware-Inventarliste; CO₂-Report.
- **Abhängigkeiten**: AP2 muss laufen.

### AP6 — Beta-Programm + Customer Development (Kat-led)
- **Stunden**: Jakob 12h | Katherine 50h
- **Inhalte**: Beta-Wartelisten-Onboarding; Kund*innen-Interviews; Pricing-Iteration; B2B-Akquise (Kanzleien, Praxen).
- **Ziele**: 50 zahlende Beta-Kund*innen.
- **Verifizierbar**: Kund*innen-Liste; NPS-Survey-Ergebnisse.
- **Abhängigkeiten**: AP2 + AP3.

### AP7 — Markenrecht + Kommerzieller Launch
- **Stunden**: Jakob 10h | Katherine 30h
- **Inhalte**: Markenanmeldung "SoTranscribe" beim EUIPO; AGB für Enterprise-Tarife; Live-Pricing-Page.
- **Ziele**: EUIPO-Marke angemeldet; Enterprise-Pricing live.
- **Verifizierbar**: EUIPO-Anmeldungsbestätigung; Live-Pricing-Page.
- **Abhängigkeiten**: AP6 läuft.

### AP8 — Projektmanagement + Berichterstattung
- **Stunden**: Jakob 10h | Katherine 20h
- **Inhalte**: Halbjahresbericht 1 (März 2027); Halbjahresbericht 2 (Sept 2027 = Endbericht); Endabrechnung; Stundenaufzeichnung.
- **Ziele**: Form- und fristgerechte Berichte an Wirtschaftsagentur Wien.
- **Verifizierbar**: Eingereichte Berichte.
- **Abhängigkeiten**: zieht sich über alle APs.

```
─────────────────────────────────────────────
GESAMTSTUNDEN: Jakob 312h + Katherine 120h = 432h
GESAMTKOSTEN PERSONAL: € 18.000 (vor Gemeinkostenzuschlag)
DAVON VON FRAUEN GELEISTET: 120h (27,8%)
CO-PROJEKTLEITUNG: Jakob Possert-Bienzle + Katherine Colquitt
                   (qualifizierte weibliche Co-Projektleitung als
                   Voraussetzung für Frauenbonus erfüllt)
```

---

## 4. Projektbeschreibung (max 5000 Z.)

**AUSGANGSSITUATION**

SoTranscribe schließt eine konkrete Lücke im Weltmarkt für Audio-Transkription. Der Großteil aller Transkriptionsdienstleistungen erfolgt heute über US-Anbieter (Otter, Rev, Descript) oder die OpenAI Whisper API. Diese Dienste fallen sämtlich unter den US CLOUD Act 2018, der US-Behörden weltweiten Zugriff auf gespeicherte Daten gewährt — auch wenn die Daten physisch in der EU liegen. Audio-Aufnahmen von Meetings, Therapiesitzungen, Interviews oder vertraulichen Gesprächen sind besonders sensible Inhalte, die unter DSGVO explizit als schutzwürdig gelten.

Die Marktlücke: ein praktikabler, nicht rein technisch-orientierter Transkriptionsdienst, der außerhalb des CLOUD-Act-Bereichs operiert und gleichzeitig Open-Source-Quellcode für Selbsthoster bereitstellt. Existierende europäische Privacy-Lösungen (Whisperit, Swiss Transcript) sind beide Closed-Source und in der Schweiz gehostet — deren rechtliche Situation verschlechtert sich durch die anstehende VÜPF-Revision (Schweizer Bundesrat-Verordnung 2025/2026, mit Decryption-Pflicht für Provider und Daten-Retention ab 5.000 Nutzer*innen).

**KONKRETE PROBLEME, DIE WIR ADRESSIEREN**

1. Jurisdiktionsproblem: Sensitive Audio-Inhalte unterliegen heute zwingend US-Recht. Schweizer Alternativen verlieren ihren Vorteil durch die VÜPF-Revision (Proton verlagert seine Infrastruktur bereits in die EU).
2. Praktikabilitätsproblem: Open-Source-Lösungen erfordern technische Installation und laufende Wartung — nicht zumutbar für Endnutzer.
3. Hardware-Kosten-Problem: Whisper Large v3 benötigt eine GPU der RTX-3090-Klasse, was viele potenzielle Nutzer abschreckt.
4. Hardware-Sovereignty-Problem: Open-Source-Software läuft heute überwiegend auf x86 (Intel ME, AMD PSP), was eine vollständige Vertrauenskette erschwert.

**TECHNISCHES UND FACHLICHES PROBLEM ZUR LÖSUNG**

Wir entwickeln eine produktreife Open-Source-Pipeline (Whisper Large v3 + pyannote-Sprecherdiarisation) sowohl als Self-Host-Lösung als auch als gehosteten Dienst auf Servern in Österreich. Zentrale technische Herausforderungen: Aufbau einer leistungsfähigen, kostengünstigen Multi-Tenant-Infrastruktur am Standort Klagenfurt; Entwicklung eines Multi-Architektur-Pipeline-Designs (RISC-V, Apple Silicon, Intel, AMD); Validierung eines neuartigen "Hardware-Kreislauf"-Modells, bei dem Nutzer eigene Altgeräte gegen Transkriptions-Credits einbringen können (gepaart mit erneuerbarer Energie für Klimaimpact).

**STAND DER EIGENEN PROJEKTENTWICKLUNG (vor Antragstellung)**

- Marketing-Site live: sotranscribe.com (deployed 2026-04-30)
- Technischer Prototyp lokal funktionsfähig (Whisper Large v3 + pyannote)
- Brand-Identität, Visual Design, Imprint, DSGVO-konforme Datenschutz­erklärung erstellt
- Beta-Wartelisten-System aktiv (connect@sotranscribe.com)
- Open-Source-Lizenz vorbereitet (EvoBioSys-Lizenz, MPL-2.0-Sublizenz)
- Sovswitch.com (Schwesterprojekt) live mit SoTranscribe als zentralem Produkt

**ZIELE UND ERGEBNISSE BIS 31.08.2027**

- Produktreifer Open-Source-Release der gesamten Pipeline
- Aktiver Beta-Hosting-Service mit dedizierter Hardware in Anexia Klagenfurt
- Mindestens 50 zahlende Beta-Kund*innen
- EUIPO-Markenanmeldung "SoTranscribe"
- Validierung von mindestens drei alternativen Hardware-Architekturen (RISC-V, Apple Silicon, x86) für die Transkriptions-Pipeline
- Öffentlich dokumentierter Tech-Stack ohne ein einziges US-jurisdiktions­rechtliches Element in der Datenpfadkette
- Aufbau einer Wiener Betriebsstätte mit Vorbereitung auf zwei zukünftige Festanstellungen (technische Mitwirkung + Kund*innen­betreuung) ab Q1 2028

**NACHHALTIGE ÖKONOMISCHE WERTSCHÖPFUNG IN WIEN**

Die SoTranscribe GmbH (in Gründung) wird ihren Sitz dauerhaft in Wien haben. Sämtliche Anstellungen erfolgen am Standort Wien. Hosting-Kolokation in Anexia Klagenfurt (Österreich). Knowhow-Aufbau in Wien.

---

## 5. Umsetzung, Methodik und Herausforderungen (max 5000 Z.)

**UMSETZUNGSANSATZ**

Wir gliedern das Projekt in acht Arbeitspakete (siehe AP-Übersicht), die teilweise sequentiell und teilweise parallel abgearbeitet werden. Die Methodik folgt einem iterativen Open-Source-Entwicklungsmodell mit halbjährlichen öffentlichen Releases.

**TECHNISCHE LÖSUNGSANSÄTZE**

1. *Transkriptions-Pipeline (Kern)*
Open-Source-Stack: faster-whisper (CTranslate2-optimiert) für Whisper Large v3 und Distil-Whisper-v3, pyannote.audio für Sprecher-Diarisation, FFmpeg für Audio-Vorverarbeitung. Backend in Rust für Performance und Speicherverwaltung; Frontend in React. Containerisiert via Podman (open-source, rootless, kein Docker-Daemon).

2. *Österreichisches Hosting (USP)*
Kolokation eigener Hardware in Anexia Klagenfurt (Österreich, ISO-14001-zertifiziert, 100% Ökostrom). Encrypted Storage; Monitoring; SLA-Setup. Standort wurde bewusst über Schweiz gewählt: österreichische Rechtsordnung (§ 134/135a StPO) erlaubt nur richterlich verfügte, einzelfallbezogene Auskunft — niemals Massenüberwachung. Schweizer VÜPF-Revision erodiert den traditionellen Schweizer Vorteil aktuell deutlich (Proton verlegt Infrastruktur bereits in die EU).

3. *Multi-Architektur-Validierung*
Test-Pipelines für: x86_64 (Intel/AMD, Baseline), Apple Silicon (Mac Mini M4), RISC-V (SiFive HiFive Premier P550 + Milk-V Megrez als Bootstrapping-Plattform). Talos II (POWER9, Raptor Computing Systems) als Roadmap-Item für die Phase nach Produktionsreife.

4. *Old-Laptop-Recovery-Programm (USP)*
Nutzer*innen können funktionierende Notebooks mit RTX-3060-Klasse-GPU oder besser einbringen. Im Gegenzug erhalten sie unlimitierte Transkriptions-Credits. Die Hardware wird in unsere Kolokation integriert und zusätzlich für ungenutzte Compute-Slots in Multi-Tenant-Modus genutzt. Pairing mit erneuerbarer Energie (Anexia 100% Ökostrom). Klimaschutz-Aspekt: Verlängerung der Hardware-Nutzungsdauer ohne Neukauf, plus Verwertung idle Compute-Kapazität.

**MÖGLICHE HERAUSFORDERUNGEN UND ENTWICKLUNGSRISIKEN**

*Technisches Risiko 1 (GPU-Skalierung)*: Whisper Large v3 erfordert ~10 GB VRAM. Mitigation: Beta-Phase mit limitierter Concurrency; schrittweiser Hardware-Ausbau aus Erlösen und Förderung; Old-Laptop-Programm als Skalierungs-Hilfe.

*Technisches Risiko 2 (RISC-V-Inferenz-Performance)*: RISC-V-CPUs leisten heute deutlich weniger als x86. Mitigation: RISC-V wird zunächst als Forschungs- und Bootstrapping-Plattform behandelt, nicht als primäres Hosting.

*Technisches Risiko 3 (Old-Laptop-Heterogenität)*: unterschiedliche Hardware aus Endnutzer-Hand erhöht Wartungsaufwand. Mitigation: minimale Hardware-Spezifikation für Annahme; standardisierter Linux-basierter Stack; geräteweise Capacity-Planning.

*Ökonomisches Risiko (Konkurrenz)*: Whisperit (CH, juristisch fokussiert) und Swiss Transcript (CH, generalistisch). Mitigation: Open-Source-Differenzierung, AT-Jurisdiktion (zielgerichtete Auskunfts­pflicht statt VÜPF-Decryption-Mandat), Multi-Architektur-Test, Old-Laptop-Programm.

*Wirtschaftliches Risiko (Zahlungsbereitschaft)*: Mitigation: drei Tarifstufen (Self-Host gratis, Beta günstig, Enterprise individuell); mittelfristig Kollektivhosting-Modell auf der Roadmap.

**PRODUKTION**

Da es sich um Software- und Service-Entwicklung handelt, erfolgt die "Produktion" (Code, Hosting-Setup, Dokumentation) vollständig im eigenen Unternehmen am Standort Wien. Hardware-Beschaffung erfolgt extern, Konfiguration intern. Externe Dienstleistungen werden gezielt für rechtliche Beratung, Steuerberatung, Sicherheits-Audits und Markenanmeldung in Anspruch genommen.

Die Angaben zur Projektumsetzung spiegeln sich vollständig in den definierten Arbeitspaketen (AP1–AP8) wider.

---

## 6. Alleinstellungsmerkmal, Konkurrenz, Markt (max 5000 Z.)

**ALLEINSTELLUNGSMERKMAL VON SOTRANSCRIBE**

Wir kombinieren vier Eigenschaften, die in dieser Kombination am Weltmarkt nicht existieren:

1. **Open-Source unter klarer Lizenz** (EvoBioSys-Lizenz, MPL-2.0-Sublizenzierung). Konkurrenten Whisperit und Swiss Transcript sind beide Closed-Source.

2. **Österreichisches Hosting in einer Zeit, in der die Schweiz jurisdiktionellen Boden verliert.** Die anstehende Schweizer VÜPF-Revision (Bundesrat-Verordnung, voraussichtlich 2026 in Kraft) führt eine Decryption-Pflicht für Provider (Artikel 50a), Daten-Retention ab 5.000 Nutzer*innen, und Identifikations­pflicht ein. Proton (Schweizer Privacy-Pionier) hat bereits öffentlich angekündigt, Infrastruktur in die EU zu verlagern. Österreich hingegen folgt § 134/135a StPO: Auskunfts­pflicht nur auf richterlich verfügter, einzelfallbezogener Basis — niemals Massenüberwachung. Verfassungs­gerichtshof-Urteil 2014 (G47/2012) verbot allgemeine Vorrats­datenspeicherung. Quick-Freeze-Verfahren wurde vom Parlament nicht angenommen.

3. **Multi-Architektur-Validierung.** Wir testen die Pipeline auf x86, Apple Silicon und RISC-V. Konkurrenten arbeiten ausschließlich auf x86 in vermieteter Cloud-Infrastruktur. Sovereignty als Wahlmöglichkeit, nicht als Ideologie.

4. **Old-Laptop-Recovery-Programm.** Einzigartiges "Hardware-im-Tausch-für-Service"-Modell mit Klimaschutz-Komponente: Nutzer*innen geben funktionsfähige Altgeräte ab, wir nutzen sie in Kolokation mit erneuerbarer Energie, idle Compute-Kapazität wird zusätzlich für andere Projekte verwendet.

**STAND DER TECHNIK / KONKURRENZÜBERSICHT**

- *Whisperit (CH)*: Closed-Source, fokussiert auf Recht/Medizin, Pricing intransparent, kein Self-Host. Schweizer Hosting verliert 2026 Vorteile (VÜPF).
- *Swiss Transcript (CH)*: Closed-Source, generalistisch, ausschließlich Schweizer Hosting, kein Self-Host. Selbe VÜPF-Problematik.
- *Otter, Rev, Descript (USA)*: Branchenführer, Closed-Source, US-Jurisdiktion (CLOUD Act), EUR 10–30/Monat.
- *OpenAI Whisper API (USA)*: API-only, US CLOUD Act, auch bei "EU-Region"-Nutzung.
- *faster-whisper / WhisperX (Bibliotheken)*: keine Service-Schicht, technische Installation erforderlich.

**MARKTGRÖßE UND MARKTENTWICKLUNG**

Der globale Transkriptionssoftware-Markt wird 2026 auf rund USD 4,4 Mrd. geschätzt (Grand View Research) bei einer prognostizierten CAGR von 14,6% bis 2030. Der europäische Anteil liegt bei ca. 24% (USD 1,06 Mrd.); davon entfallen ca. 5–8% auf datenschutz-sensitive Use-Cases (Recht, Medizin, Journalismus, NGOs).

Mittelfristige Markttreiber:
- DSGVO-Verschärfungen seit 2024 erhöhen Druck auf US-Cloud-Nutzung
- Wachsendes Bewusstsein für CLOUD-Act-Implikationen (Schrems II, FISA-Verlängerung 2024)
- Schweizer VÜPF-Revision treibt aktiv Privacy-Provider und ihre Kund*innen aus der Schweiz heraus → Akquise-Chance für Österreich
- Verbreitung von Wearables und KI-Assistenten erzeugt persönliche Audio-Korpora
- Anstieg "souveräner KI"-Initiativen (NGI, Sovereign Tech Fund, NLnet)

Wir adressieren konservativ einen erreichbaren Markt von rund EUR 50 Mio. in der DACH-Region. Realistisches Marktanteilsziel in den ersten drei Jahren: 0,1% (~EUR 50.000–100.000 ARR).

---

## 7. Schutzstrategie (max 5000 Z.)

**EIGENES GEISTIGES EIGENTUM**

Die Pipeline-Architektur, die Old-Laptop-Recovery-Logik und die Multi-Tenant-Hosting-Konfiguration sind eigenes geistiges Eigentum. Schutzansatz:

1. *Open-Source-Veröffentlichung als geschäftliches Asset*
Der Quellcode wird unter der EvoBioSys-Lizenz (MPL-2.0-Sublizenzierung) veröffentlicht. Bewusste strategische Entscheidung: Open Source schützt vor proprietärer Vereinnahmung durch Großunternehmen und schafft Vertrauen bei datenschutz-sensitiven Zielgruppen. Wertschöpfung erfolgt nicht über Lizenzgebühren, sondern über Hosting, Support und Spezialisierung der Pipeline.

2. *Markenrecht*
Die Marken "SoTranscribe" und das zugehörige Logo werden als EU-Unionsmarken (EUIPO) angemeldet. Die Domain sotranscribe.com ist bereits in unserem Besitz.

3. *Geschäftsgeheimnis-Schutz*
Multi-Tenant-Hosting-Konfiguration, Customer-Liste, Beta-Programm-Daten und kommerzielle Verträge bleiben geschützt durch Vertraulichkeits­regelungen und Geschäftsgeheimnis-Schutz nach UWG.

4. *Trade Secret auf Hardware-Recovery-Verfahren*
Die operative Logik des Old-Laptop-Recovery-Programms (Annahme-Kriterien, Capacity-Planning, Idle-Compute-Vermarktung) bleibt vorerst Trade Secret. Patentanmeldung wird nicht in der Projektphase verfolgt, sondern bewusst in spätere Phasen verschoben.

5. *Network-Effects als ökonomischer Moat*
Die Beta-Kund*innen-Beziehungen, die EU-Payment-Stack-Integrationen (Mollie, Lago, GoCardless) und die etablierten Open-Source-Community-Kanäle bilden Lock-in-freie aber dennoch wertvolle Network-Effects.

**FREMDES GEISTIGES EIGENTUM**

Wir nutzen Open-Source-Komponenten, deren Lizenzen vollständig eingehalten werden:
- OpenAI Whisper Large v3 (MIT-Lizenz, kommerziell nutzbar)
- pyannote.audio (MIT)
- faster-whisper (MIT)
- CTranslate2 (MIT)
- FFmpeg (LGPL/GPL je nach Build)
- React (MIT)
- Rust + zugehörige Crates (MIT/Apache-2.0)

Sämtliche Drittlizenzen werden in einer öffentlichen NOTICE-Datei dokumentiert. Es werden KEINE proprietären Komponenten von US-Anbietern verwendet (Stripe, Google Fonts, Google Analytics explizit ausgeschlossen — siehe Datenschutzerklärung).

**LIZENZIERUNGSSTRATEGIE FÜR DRITTNUTZER**

Drittnutzer können den Source unter EvoBioSys-Lizenz / MPL-2.0 verwenden. Kommerzielle Nutzer mit jährlichen Ressourcen über EUR 10.000 erwerben optional eine Enterprise-Lizenz mit Support-Verpflichtung. Open-Core-Modell, strukturell verträglich mit der GPL-Familie und nachhaltig finanzierungstauglich.

---

## 8. Kund*innennutzen und Zielgruppe (max 5000 Z.)

**KUND*INNENNUTZEN**

SoTranscribe bietet konkreten, messbaren Nutzen: vertrauliche Audio-Aufnahmen werden in durchsuchbare Texte umgewandelt, ohne dass die Daten US-jurisdiktionsrechtliche Anbieter durchqueren. Mit dem Standort Österreich entgehen Kund*innen zusätzlich der anstehenden Schweizer VÜPF-Decryption-Pflicht.

Nutzen je Zielgruppe:

1. **Anwaltskanzleien, Mediziner*innen, Therapeut*innen**
Schutz von Mandantengesprächen, Patientenakten, Therapieaufzeichnungen vor unbefugter Datenherausgabe. DSGVO-konform mit nachweisbarer Datensparsamkeit. Keine US-Jurisdiktion, keine VÜPF-Backdoor-Pflicht.

2. **Journalist*innen, Investigativrecherche**
Quellenschutz bei Interviews und Hintergrundgesprächen. Stärkerer Schutz als bei US-Cloud-Lösungen oder bei sich verändernden Schweizer Anbietern.

3. **NGOs, Stiftungen, EU-geförderte Forschung**
DSGVO-Pflicht zur Datenminimierung; AVV mit nachvollziehbarer EU-Wertschöpfungs­kette.

4. **Tech-Privatpersonen, "Quantified Self"-Nutzer*innen**
Persönliche Audio-Archive (Voice-Memos, Wearables) werden durchsuchbar — ohne Cloud-Eigentum durch Big Tech.

5. **Selbsthoster, Open-Source-Communities**
Kostenfreier Zugang zur Pipeline. Beitragsmöglichkeiten zur Codebase.

6. **Hardware-Einbringer*innen (Old-Laptop-Programm)**
Tausch von Altgeräten gegen unlimitierte Transkriptions-Credits. Einsparung gegenüber Neukauf, Hardware-Lebensverlängerung, Klimaimpact.

**CHARAKTERISIERUNG DER ZIELGRUPPEN**

Primärer Markt (DACH, Beta-Phase Q4 2026 – Q3 2027):
20.000–30.000 datenschutz-sensitive Kanzleien und Praxen in Österreich, Deutschland, Schweiz. Geschätzte Zahlungsbereitschaft: EUR 15–60/Monat. Schweizer Kund*innen verstärkt akquirierbar durch VÜPF-Migration.

Sekundärer Markt (EU-weit, ab Q4 2027):
Mittelständische Unternehmen mit DSGVO-Compliance-Druck (~50.000 Unternehmen). Open-Source-Communities (kostenfreier Self-Host als Akquisekanal).

Tertiärer Markt (Hardware-Einbringer*innen):
Tech-affine Privatpersonen mit Interesse an Sustainability-Themen und Climate-Action.

**KONKRETES KUND*INNEN­INTERESSE HEUTE**

- Beta-Wartelistensystem aktiv über connect@sotranscribe.com
- Erste Anfragen seit Veröffentlichung der Site (sotranscribe.com, live seit 30.04.2026)
- Sondierungsgespräche mit Wiener Datenschutz­kanzleien laufen
- Strategisches Pre-Seed-Backing durch privaten US-basierten Angel-Investor (Kevin Triplett)

Geplante Beta-Programm-Größe bis 31.08.2027: 50–100 zahlende Beta-Nutzer*innen, davon mindestens 60% aus dem DACH-Raum.

---

## 9. Preismodell und Umsatzerwartung (max 5000 Z.)

**PREISMODELL**

Drei Tarifstufen plus Hardware-Tausch-Option:

1. **Self-Host (kostenlos)** — Open-Source-Quellcode unter EvoBioSys-Lizenz. Akquisekanal für Hosted-Tarife.

2. **Beta-Hosting** (Indikation EUR 15–35/Monat) — Gehosteter Service auf Servern in Österreich. Pricing transparent über Open Collective Europe entwickelt.

3. **Enterprise** (custom, Indikation EUR 200–800/Monat) — Maßgeschneiderte Integration, größere Volumina, Support-Vertrag, signiertes AVV.

**Hardware-Tausch-Option**: Nutzer*innen, die ein funktionsfähiges Notebook mit GPU der RTX-3060-Klasse oder besser einbringen, erhalten 24 Monate unlimitierte Transkriptions-Credits. Pairing mit erneuerbarer Energie (Anexia 100% Ökostrom).

**PLAN-UMSATZ FÜR DREI JAHRE NACH PROJEKTENDE**

Jahr 1 (2027/28):
- 50 Beta-Nutzer*innen × € 25/Monat × 12 = € 15.000
- 5 Enterprise-Kunden × € 400/Monat × 12 = € 24.000
- **GESAMT JAHR 1: ~€ 39.000**

Jahr 2 (2028/29):
- 200 Beta-Nutzer*innen × € 25/Monat × 12 = € 60.000
- 20 Enterprise-Kunden × € 500/Monat × 12 = € 120.000
- **GESAMT JAHR 2: ~€ 180.000**

Jahr 3 (2029/30):
- 600 Beta-Nutzer*innen × € 30/Monat × 12 = € 216.000
- 60 Enterprise-Kunden × € 600/Monat × 12 = € 432.000
- **GESAMT JAHR 3: ~€ 648.000**

**ANNAHMEN UND KALKULATIONEN**

- Wachstumsrate Beta: 4× pro Jahr (B2B-SaaS-Benchmarks im EU-Markt)
- Wachstumsrate Enterprise: 4× pro Jahr (Word-of-Mouth aus DSGVO-sensitiven Sektoren)
- Conservative Pricing-Hypothese: Mid-Market-SaaS-Muster
- Schweizer Migrations-Akquise als Anfangs-Schub: ~10–15 Customers aus Proton-Nachfolge-Markt
- Kostenstruktur: ~30% Hosting/Hardware, ~50% Personal, ~20% Marketing/Sonstiges
- Break-Even erwartet im Q4 2028

---

## 10. Vertriebs- und Marketingmodell (max 5000 Z.)

**VERTRIEBSSTRATEGIE**

Dreigleisige Vertriebsstruktur:

1. **Direktvertrieb (Beta + Enterprise)** — Über sotranscribe.com mit Wartelistensystem. Persönliche Beratungs­gespräche für Enterprise-Anfragen über connect@sotranscribe.com. Hauptansprech­person: Katherine Colquitt (Co-Projektleiterin / Commercial Lead).

2. **Open-Source-Distribution (Self-Host)** — Source-Repository auf GitHub, mittelfristig auf selbstgehostetem GitLab in der EU. Dokumentation auf der Website unter /self-host. Community-Support über E-Mail und Matrix-Kanal.

3. **Partnerschaftsvertrieb (mittel- bis langfristig)** — DSGVO-Beratungs­unternehmen (Empfehlungs­partnerschaften), Mesh-Netzwerk-Communities (Funkfeuer Wien) für lokale Glaubwürdigkeit, Datenschutz­kanzleien als Multiplikatoren.

**MARKETINGSTRATEGIE**

Vier Hauptkanäle:

1. **Inhaltliches Marketing** — Technischer Blog auf sovswitch.com (Schwester-Projekt), Konferenz­beiträge (FOSDEM 2027 in Brüssel, Open-Source-Tracks), Whitepaper zur österreichischen Auskunftspflicht-Regelung versus Schweizer VÜPF als juristisches Differenzierungs­merkmal.

2. **Community-Aufbau** — Mastodon-Präsenz auf einer EU-Instanz, Bluesky für broader-public Sichtbarkeit, Veröffentlichung der Pipeline auf Hacker News und Lobsters bei jedem Release.

3. **Direkte B2B-Akquise (Kanzleien, Praxen)** — Personalisierte Kaltakquise durch Katherine Colquitt; Präsentationen bei Wiener und Berliner Kanzlei­netzwerken; DSGVO-Compliance-Webinare als Lead-Magnete; Schweizer Migrations-Akquise (Privacy-Provider und ihre Kund*innen, die aus der Schweiz wegziehen).

4. **Partnermarketing** — Co-Marketing mit Open-Source-Allies (Hylo, ungleich, Funkfeuer); Erwähnungen in Privacy-Guides (privacyguides.org, EFF, NOYB).

**ZIELMARKTANSPRACHE**

Primär DACH (Deutsch + Englisch). Ab Jahr 2 Erweiterung auf Französisch und Spanisch. Marketing-Tonalität: pragmatisch, nicht ideologisch — Sovereignty als Wahlmöglichkeit, nicht als Glaubensfrage.

**FINANZIELLE UND PERSONELLE RESSOURCEN**

Marketing-Budget in der Förderphase: EUR 0 (nicht förderbar — wird aus Eigenleistung erbracht). Personell: Katherine 10–15 h/Monat, Jakob 5–10 h/Monat.

Post-Projektende: dediziertes Marketing-Budget aus Beta-/Enterprise-Erlösen.

---

## 11. Umwelt (max 3000 Z.)

**POSITIVE AUSWIRKUNGEN**

1. *Hardware-Lebensverlängerung durch Old-Laptop-Recovery-Programm*
Funktionsfähige Notebooks, die sonst entsorgt würden, werden in unsere Kolokation in Klagenfurt integriert. Zusätzlich werden idle-Compute-Kapazitäten dieser Geräte für andere klimafreundliche Compute-Aufgaben verwendet (z.B. öffentliche-Forschungs-Compute, Climate-Modeling). Pro Gerät werden geschätzt 200 kg CO₂eq Embedded-Emissionen gespart (Apple Environmental Report 2024). Bei 100 Geräten in den ersten 12 Monaten: ~20 Tonnen CO₂eq.

2. *Erneuerbarer Strombezug*
Kolokation bei Anexia Klagenfurt: nachweislich zertifizierter Ökostrom (ISO 14001, 100% erneuerbar). Vermeidung des US-Hyperscaler-Strommixes (Texas, fossiler Anteil hoch).

3. *Vermeidung von Cloud-Redundanz-Overhead*
Im Vergleich zu US-Hyperscalern mit kontinentaler Geo-Redundanz läuft unser Workload auf einem fokussierten Standort. ~30% weniger Energieverbrauch pro Transkription durch eingesparte Datenreplikation.

4. *Förderung lokaler Wertschöpfung*
Wiener Standort, lokale Beschäftigung, lokale Hardware-Beschaffung soweit möglich. Klagenfurt für Hosting (Kärnten-Wertschöpfung).

5. *Bahn-priorisierte Reisetätigkeiten*
Wien-Klagenfurt per Bahn (3:45 h, ~2 kg CO₂eq) statt Flug. Wien-Berlin Nachtzug. Wien-Zürich (post-Migration der Kund*innen) per Railjet.

**NEGATIVE AUSWIRKUNGEN (transparent benannt)**

1. *Hardware-Neubeschaffung im Projektrahmen*
R&D-Hardware (RISC-V-Boards, Mac Mini, Server) im Wert von ca. EUR 18.000. Geschätzte Embedded-Emissionen: ~1,5 Tonnen CO₂eq. Mitigation: Hardware bleibt im Unternehmen, wird im Old-Laptop-Programm später möglicherweise weitergegeben.

2. *Strombedarf der Hosted-Tier*
Whisper Large v3 ist GPU-intensiv. Pro Stunde Audio: ~0,3 kWh. Mitigation: ausschließlich Hosting bei Ökostrom-Anbietern.

**VERGLEICH ZUM IST-ZUSTAND**

Bestehende Anwendungen (Whisper API von OpenAI, Otter.ai) hosten in den USA bei gemischtem Strommix. Unser Setup spart pro Transkription geschätzt 40–60% Energie ein durch effizientere Modellgrößen, lokales Hosting und erneuerbare Energie. Mittelfristig zusätzlicher Faktor durch Old-Laptop-Programm.

**KREISLAUFWIRTSCHAFT**

Old-Laptop-Programm IST Kreislaufwirtschaft im Kern: Hardware, die sonst entsorgt würde, wird Teil produktiver Compute-Infrastruktur, gepaart mit erneuerbarer Energie.

---

## 12. Diversität auf Projektebene (max 3000 Z.)

**ZUSAMMENSETZUNG DES PROJEKTTEAMS**

Das Gründungsteam ist in zentralen Diversitätsdimensionen ausgewogen:

- *Geschlecht*: 50/50 Co-Foundership. Katherine Colquitt (weiblich) ist Co-Projektleiterin, Mit-Gesellschafterin (26%), Co-Geschäftsführerin. Jakob Possert-Bienzle (männlich) ist Co-Projektleiter / Technical Lead. In einer Branche, in der Frauenanteile in technischen Führungspositionen typischerweise unter 15% liegen, ist diese Zusammensetzung deutlich überdurchschnittlich.

- *Herkunft*: USA (Cornell-Absolventin) + Österreich (Minerva-Absolvent). Transatlantische Co-Foundership bringt komplementäre kulturelle Perspektiven in einen US-dominierten Markt.

- *Alter*: Beide Gründer*innen unter 35.

**DIVERSITÄTSASPEKTE IN DER PROJEKTUMSETZUNG**

1. *Zielgruppen-Diversität* — Zielgruppen umfassen sowohl finanzkräftige Enterprise-Kunden als auch Privatnutzer*innen mit niedrigerem Budget (Self-Host kostenlos). Old-Laptop-Recovery-Programm ermöglicht insbesondere finanziell schwächeren Personen (Studierende, NGO-Mitarbeitende) Zugang ohne monetären Einsatz.

2. *Sprachliche Diversität* — Whisper Large v3 unterstützt ~100 Sprachen. Priorität in Phase 1: Englisch + Deutsch. Phase 2: Französisch + Spanisch (Inklusion lateinamerikanischer und afrikanischer Diasporas in Europa).

3. *Barrierefreiheit* — Website mit Atkinson Hyperlegible (entwickelt vom Braille Institute für sehbehinderte Nutzer*innen). WCAG-2.1-AA-Konformität ist Designziel. Audio-Transkription selbst ist eine Barrierefreiheits-Technologie (Untertitelung, Schwerhörigen-Unterstützung).

**DIVERSITÄT BEI ZUKÜNFTIGEN ANSTELLUNGEN**

Bei den geplanten zwei zukünftigen Festanstellungen wird aktiv um diverse Kandidat*innen geworben. Wir nutzen Frauenförder-Netzwerke (FemTech Wien, Women in Tech) und Migrant*innen-fokussierte Tech-Initiativen (CodeFactory).

**NEGATIVE AUSWIRKUNGEN**

Wir sehen keine erkennbar negativen Diversitäts­auswirkungen. Sollte sich das Old-Laptop-Programm überproportional auf männliche Tech-Affinität korrelieren (gängige Hardware-Hortungs-Demographie), werden wir aktiv weibliche und nicht-binäre Nutzer*innen ansprechen.

---

## 13. Beschäftigungseffekte (max 5000 Z.)

**AKTUELLE MITARBEITER*INNEN-SITUATION**

SoTranscribe GmbH (in Gründung) hat zum Antragstellungs­zeitpunkt zwei Gründer*innen:
- Katherine Colquitt (Co-Projektleiterin / Commercial Lead, 120h über 12 Monate)
- Jakob Possert-Bienzle (Co-Projektleiter / Technical Lead, 312h über 12 Monate)

Beide werden während der Projektlaufzeit über Geschäftsführer­bezug (Katherine) bzw. Werkvertrag aus dem bestehenden Einzelunternehmen (Jakob) im Rahmen der projekteigenen Personalkosten­positionen vergütet (Stundensatz nach WAW-Pauschalierung: € 41,67/h).

**GEPLANTE ANSTELLUNGEN WÄHREND DER PROJEKTLAUFZEIT**

Während der 12-monatigen Projektlaufzeit ist KEINE Festanstellung geplant. Begründung: Ein 12-monatiges Projekt mit EUR 60.000 Gesamt­budget rechtfertigt keine Vollzeit-Festanstellung. Die Entwicklung erfolgt durch die Gründer*innen sowie über punktuelle externe Dienstleistungen.

**GEPLANTE ANSTELLUNGEN NACH PROJEKTABSCHLUSS (Q4 2027 – Q4 2028)**

Sofern die Beta-Phase erfolgreich verläuft (Ziel: 50+ zahlende Kund*innen zum Projektende, ARR ~EUR 40.000), planen wir die Aufnahme von zwei Mitarbeiter*innen in den 12 Monaten nach Projektabschluss:

1. **Software Engineer / DevOps (Vollzeit, Q1 2028)**
Aufgaben: Pipeline-Wartung, Skalierungs­entwicklung, Release-Management, Old-Laptop-Programm-Operationen. Ziel: technisches Know-how von Jakob auf eine zweite Person übertragen, sodass Jakob für strategische Aufgaben (Produkt­entwicklung, Hardware-Sovereignty-R&D, Finanzierungsrunden) freigesetzt wird.
Geschätztes Gehalt: EUR 55.000–70.000 brutto/Jahr.
Rekrutierung: Mastodon, Hacker News, Wiener TU-Alumni-Netzwerke.

2. **Customer Success / Beta Support (Teilzeit oder Vollzeit, Q3 2028)**
Aufgaben: Onboarding der Beta-Nutzer*innen, Tier-1-Support, Community-Aufbau (Matrix, Mastodon), Dokumentation. Reporting an Katherine.
Geschätztes Gehalt: EUR 40.000–55.000 brutto/Jahr.
Rekrutierung: Wiener Universitäten (Geisteswissenschaften), Wiedereinsteiger*innen-Netzwerke, NGO-Sektor.

**MITTELFRISTIGE WACHSTUMSPLANUNG (Jahr 3, 2029)**

Bei plangemäßer Umsatzentwicklung: Aufstockung auf 4–6 FTEs in der Wiener Betriebsstätte. Schwerpunkte: zweiter Software-Engineer, Vertriebsmitarbeiter*in, Hardware-Operations für die Kolokation und das Old-Laptop-Programm.

**AUSWIRKUNGEN AUF DEN WIENER STANDORT**

Sämtliche Anstellungen erfolgen am Standort Wien. Die SoTranscribe GmbH (in Gründung) wird ihren Sitz dauerhaft in Wien haben. Beschäftigungs­effekte werden durch die Wirtschaftsagentur-Förderung von Anfang an in Wien verankert. Nachhaltige ökonomische Wertschöpfung in Wien.

---

## 14. Gründungsteam und Vorkenntnisse (max 2000 Z.)

**KATHERINE COLQUITT** — Co-Projektleiterin / Commercial Lead / Mit-Gesellschafterin (26%) / Co-Geschäftsführerin

Cornell University Absolventin. Strategic Communications Manager bei Edelman Smithfield in New York mit Spezialisierung auf Finanz- und Technologie­kommunikation; zuvor Strategic Communications bei APCO Worldwide. Mehrjährige Projektmanagement-Erfahrung mit komplexen Stakeholder-Konstellationen, Investor Relations, B2B-Positionierung und transatlantischen Kommunikations­strategien. Bringt für SoTranscribe das kommerzielle Fundament: Markteinführung, Beta-Programm-Aufbau, Partnerschafts­entwicklung, Investor-Vorbereitung.

**JAKOB POSSERT-BIENZLE** — Co-Projektleiter / Technical Lead / Mit-Gesellschafter (74%) / Co-Geschäftsführer

Minerva University Absolvent (transdisziplinäres systemisches Denken, globaler Studienverlauf). Mehrjährige Entwicklung souveräner Wissens­infrastruktur-Tools: produktionsreifes Memory-System, Logseq-Plugin für Cross-Graph-Föderation, Tana-zu-Jekyll-zu-ActivityPub-Pipeline (POSSE-Architektur). Vertieftes Know-how in Rust, Python, GPU-Inferenz, verteilten Systemen, Open-Source-Lizenzdesign. Erfahrung als Berater für sustainability-orientierte Technologie-Initiativen. Hauptverantwortlich für SoTranscribe-Pipeline (Whisper Large v3 + pyannote), Hosting-Infrastruktur Anexia Klagenfurt, Open-Source-Veröffentlichung. Wohnsitz Wien.

**KOMPLEMENTARITÄT DES TEAMS**

Katherine bringt Marktverständnis, Stakeholder-Sprache und kommerzielles Disziplinen-Know-how. Jakob bringt technisches Know-how und Sovereignty-Vertiefung. Die Kombination ermöglicht die für SoTranscribe spezifische Mischung aus pragmatischem Markt- und tiefem Tech-Verständnis.

**STRATEGISCHE BACKING**

Frühphasen-Backing durch privaten US-basierten Angel-Investor Kevin Triplett (Pre-Seed). Networking-Backing durch EvoBioSys-Netzwerk und idea2.life-Inkubator.

Lebensläufe sind im Anhang.

---

## 15. Geplante Unternehmensentwicklung (max 2000 Z.)

**PHASE 1 (2026/27 — Projektphase): Produktreife + Beta-Markt**
Im Rahmen des geförderten Projekts: Produktreife der Open-Source-Pipeline; Hosting-Infrastruktur in Anexia Klagenfurt; erste 50–100 zahlende Beta-Kund*innen; EUIPO-Markenanmeldung; erste Old-Laptop-Annahmen.

**PHASE 2 (2027/28): Skalierung + Team + Old-Laptop-Programm-Skalierung**
Aufnahme der ersten zwei Mitarbeiter*innen am Wiener Standort. Erweiterung der Sprachunterstützung (Französisch, Spanisch). Skalierung des Old-Laptop-Programms auf 100+ Geräte mit gepaarter erneuerbarer Energie. Erschließung der DSGVO-sensitiven B2B-Märkte in Deutschland.

**PHASE 3 (2028/29): Geografische Expansion + Sovereignty-Hardware-Roadmap + Hallen-Ausbau**
Markterschließung Frankreich, Spanien, Lateinamerika. Evaluation der POWER9-/Talos-II-Plattform als Flaggschiff-Sovereignty-Hosting-Hardware. Aufstockung auf 4–6 FTEs. Mittelfristig Anmietung einer eigenen Halle (alte Industriehalle mit Renewable-Energy-Anschluss) für den Old-Laptop-Pool — kombiniert mit Solaranlage und/oder grüner Wärme­versorgung.

**GEPLANTE NEUE PRODUKTE/DIENSTLEISTUNGEN**
- Q1 2028: Kollektivhosting-Modell (Self-Hoster werden Community-Hoster für Freunde/Kleinkollektive)
- Q3 2028: Spezialisierte Vertikallösungen für Anwaltskanzleien (juristische Terminologie-Optimierung)
- 2029: SoArchive (durchsuchbares E-Mail-Archiv) und SoMail (sovereign Mail-Hosting) als Nachfolgeprodukte derselben Open-Source-Familie (idea2.life-Lineage)

**SOVEREIGN-SWITCH-STRATEGIE (Schwesterprojekt)**
SoTranscribe ist das erste Produkt einer breiteren Sovereignty-Stack-Strategie unter dem Dach von Sovereign Switch (sovswitch.com): pragmatische, nicht-techniker-gerichtete Migrationspfade weg von Big-Tech-Abhängigkeiten. SoTranscribe finanziert die langfristige Strategie kommerziell.

**KLIMASCHUTZMAßNAHMEN IM UNTERNEHMEN**
- Hardware-Beschaffung bei Anbietern mit Recycling-/Reparatur-Politik
- Bevorzugung erneuerbarer Energie in allen Hosting-Standorten (Anexia 100% Ökostrom)
- Old-Laptop-Programm intern und extern; Halle mit Solaranlage als Mittelfrist-Ziel
- Reisetätigkeiten priorisiert per Bahn statt Flug
- Klimaneutrales Onboarding für neue Mitarbeiter*innen

---

## 16. Anhänge / attachments to include

- ☐ Lebenslauf Jakob Possert-Bienzle (PDF)
- ☐ Lebenslauf Katherine Colquitt (PDF, LinkedIn-Export OK)
- ☐ Letztgültige Einnahmen-Ausgaben-Rechnung (Jakobs EPU)
- ☐ Privatdarlehensvertrag mit Vater (€ 4.000, PDF)
- ☐ Bankauszug (Kontostand-Nachweis)
- ☐ USDC-Wallet-Screenshot (Liquidations­absicht)
- ☐ Link zu Live-Website: https://sotranscribe.com/
- ☐ Link zu Schwesterprojekt: https://sovswitch.com/
- ☐ Optional: Business plan PDF (5–10 Seiten)
- ☐ Optional: Letter of intent von Kevin Triplett (US-Investor)

---

## 17. De-minimis-Erklärung

```
Antragstellerin: SoTranscribe GmbH (in Gründung)
Vertretung: Jakob Possert-Bienzle, Katherine Colquitt
Adresse: [Wiener Adresse]

In den letzten 3 Jahren erhaltene De-minimis-Beihilfen:
KEINE.

Datum: 30.04.2026
Unterschrift: ____________________
```
