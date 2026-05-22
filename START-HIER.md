# Welkom Lotte! Start hier.

> Hé Lotte! Dit is jouw onboarding voor Barry, onze AI-assistent. Lees dit een keer rustig door, neem je tijd. Daarna ga je samen met Tim of Niek aan de slag. Het is veel, dus niet schrikken. Je hoeft niet alles in één keer te begrijpen.

---

## 1. Wat is dit eigenlijk

Barry is geen ChatGPT. Het is een AI-assistent die op je Mac geïnstalleerd staat en die echt dingen voor je kan doen:

- Bestanden lezen en opslaan op je Mac
- Door je browser klikken (Instagram, Google Drive, alles)
- Foto's bekijken en beoordelen
- Captions schrijven die echt passen bij een zaak
- 25 Instagram-posts analyseren om de juiste toon te begrijpen

Wij hebben Barry geleerd hoe BWC werkt. Nu gaan we hem ook KO leren. En dat is jouw rol: jij bent degene die hem stap voor stap KO's zaken bijbrengt, en daarna helpt 'ie jou met posten.

**Wat we hier hebben gebouwd:** twee skills (skills = wat Barry weet hoe te doen). Eentje om een nieuwe zaak in kaart te brengen, en eentje om posts te maken voor zaken die 'ie al kent.

| Skill | Wat doet 'ie |
|---|---|
| `brand-mapper` | Leert Barry hoe een nieuwe zaak praat, eruit ziet, en welke regels er gelden. Doe je 1 keer per zaak. |
| `social-media-poster` | Maakt posts voor een zaak die Barry al kent. Doe je elke keer als je iets wil posten. |

De bedoeling: jij hoeft straks niet meer voor elke post na te denken over "hoe schreef ik ook alweer voor Aspen Valley". Barry weet dat. Jij geeft een brief, hij levert foto's + captions, jij keurt goed.

---

## 2. Wat je nodig hebt

Hieronder de checklist. Het lijkt veel, maar veel staat al voor je klaar. Je hebt het meeste alleen 1x nodig om in te stellen.

**Een Mac** ✓ (Sarah's oude MacBook Pro 16-inch, die kun je gebruiken)

**De Claude desktop app**
- Gratis download op claude.ai (kies "Download for Mac")
- Na installatie open je 'm en log je in

**Inloggegevens voor het KO Claude Teams account**
- Krijg je van Tim
- Dat is "Melissa" (zo noemen we het account intern)
- Hier kun je tot 5 mensen op, jij krijgt een eigen seat

**Een werkmail met `ko` of `bwc` in de naam**
- De skills checken bij eerste gebruik of je mail dat erin heeft
- Bijvoorbeeld `lotteko@gmail.com` of `lotte@ko-company.nl`
- Tim regelt welke je krijgt

**Chrome browser**
- Die heb je vast al
- Belangrijk: niet Safari, want we hebben een specifieke Chrome-extensie nodig

**Claude in Chrome extensie**
- Dit is wat Barry gebruikt om door je browser te klikken
- Installeren via de Chrome Web Store (Tim of Niek helpt je)
- Hierdoor kan Barry Instagram en Google Drive openen alsof hij jou is

**Google Drive ingelogd met je werkmail**
- Toegang tot alle KO-mappen (foto's, brandbooks, alles)
- Tim zorgt dat je toegang krijgt tot alles wat KO heeft

**Instagram ingelogd in Chrome**
- Anders crasht Barry na een paar posts omdat Instagram je een login-popup geeft
- Log gewoon in met je eigen Instagram of met KO's beheer-account, maakt niet veel uit

**Een mapje op je bureaublad voor Cowork**
- Hoort `Lotte Co-work` te heten (zonder hoofdletter Co, ja Co met hoofdletter, doe net zoals Tim's "Claude Co-work")
- Dit is waar Barry al jouw bestanden, brand-contexts en chats organiseert
- **Je hoeft 'm niet vooraf zelf aan te maken.** Cowork doet dat de eerste keer dat je hem start. Maar mocht ie het niet doen: maak dan zelf een mapje aan op je bureaublad met de naam `Lotte Co-work`

**Geen GitHub-account nodig**
- Onze skills staan online publiek (op github.com/BWC-Barry/social-media-toolkit)
- Je kunt 'm gewoon installeren zonder dat je daar een account voor nodig hebt

---

## 3. Welke toestemmingen Barry vraagt (en wat ze betekenen)

Bij de eerste keer dat je Barry start, vraagt 'ie om allerlei toegang. Dat ziet er soms eng uit ("Barry wil toegang tot je bestanden") maar het is allemaal nodig om zijn werk te kunnen doen. Hieronder wat elke toestemming inhoudt en wat je antwoordt:

| Wat Barry vraagt | Wat het betekent | Wat doe je |
|---|---|---|
| **Toegang tot bestanden** | Barry mag jouw `Lotte Co-work` mapje lezen en schrijven | Sta toe |
| **Toegang tot terminal / shell** | Barry mag commando's uitvoeren op je Mac (zoals een bestand kopiëren) | Sta toe |
| **Chrome MCP / Claude in Chrome** | Barry mag in jouw Chrome klikken, lezen en typen | Sta toe |
| **Toegang tot specifieke websites** | Barry vraagt soms expliciet of 'ie naar instagram.com of drive.google.com mag | Sta toe |
| **Plugin installatie** | Barry mag onze toolkit-skills downloaden en installeren | Sta toe |

**Belangrijk:** alles wat Barry doet, doet hij lokaal op jouw Mac. **Niets wordt gedeeld met Anthropic** (het bedrijf achter Claude) behalve de chats zelf om antwoord te kunnen geven. Geen bestanden, geen foto's, geen captions, geen brand-contexts. Alles blijft van jou.

Daarom: **je kunt rustig overal "sta toe" op klikken.** Het is allemaal nodig en niks gaat naar buiten dat niet hoort.

---

## 4. Hoe Barry zichzelf organiseert (zodat jij niks hoeft te onthouden)

Dit vond ik zelf wel cool toen ik 't doorhad:

- **Elke chat met Barry wordt automatisch opgeslagen.** Geen knoppen om op te drukken.
- **Barry schrijft zelf een `MEMORY.md` bestand** waarin 'ie de belangrijkste dingen onthoudt die jullie ooit hebben besproken. Bijvoorbeeld: jouw mail, dat je liever korte captions wil, dat Aspen Valley altijd in caps schrijft, alles. Hij gebruikt dat geheugen in elke nieuwe chat.
- **Alles wordt netjes georganiseerd in `Lotte Co-work` op je bureaublad.** Per project een mapje, per brand een file. Je hoeft 't niet zelf bij te houden.

**Belangrijk in elke nieuwe chat:** als Barry vraagt of je iets uit een specifiek mapje wilt gebruiken, vink dan altijd het `Lotte Co-work` mapje aan. Dat is waar al je werk in staat. Anders weet 'ie niet waar 'ie moet zoeken.

---

## 5. De toolkit installeren (2 minuten)

Doe dit samen met Tim of Niek de eerste keer, zodat ze meekijken als er iets vastloopt.

1. Open de **Claude desktop app**
2. Ga naar **Customize** (knop in het hoofdmenu)
3. Klik op **Browse plugins**
4. Klik op het tabblad **Personal**
5. Klik op het **plusje** (+) om een nieuwe plugin toe te voegen
6. Plak deze regel in het veld:

   ```
   BWC-Barry/social-media-toolkit
   ```

7. Bevestigen (Enter)
8. Klik op **Install**
9. Bevestig dat je beide skills installeert (brand-mapper en social-media-poster)
10. Klaar. Barry weet nu hoe 'ie deze twee skills moet gebruiken.

**Hoe weet je dat het werkte?**

Open een nieuwe chat met Barry en typ:

> "Barry, welke skills heb je nu beschikbaar?"

Hij zou onder andere `brand-mapper` en `social-media-poster` moeten noemen.

---

## 6. Eerste echte run: Aspen Valley in kaart brengen

Dit is meteen het belangrijkste moment. We gaan Barry leren wat Aspen Valley is. Dit duurt 30 tot 45 minuten en doen we samen.

**Voor je start:**

- Zorg dat je `Lotte Co-work` mapje is aangemaakt en aangevinkt in de chat
- Zorg dat Chrome open is en je bent ingelogd op Instagram en Google Drive
- Pak een kop koffie, want we gaan even goed nadenken samen

**Hoe je de sessie start:**

In een nieuwe chat met Barry typ je:

> "Hé Barry, we gaan Aspen Valley in kaart brengen voor de social media. Kun je de brand-mapper skill draaien? Stel zoveel mogelijk vragen, dan weet je precies wat je nodig hebt."

Die laatste zin is belangrijk. Daar kom ik in stap 7 op terug.

**Wat er dan gebeurt:**

1. Barry stelt eerst een paar basisvragen (welke zaak precies, IG-handle, brandbook beschikbaar?)
2. Barry opent Chrome en gaat naar de Instagram van Aspen Valley
3. Hij leest de laatste 25 posts en analyseert ze (welke woorden komen terug, welke emojis, hoe lang zijn de captions, hoe sluiten ze af)
4. Hij leest het brandbook als we 't aanleveren (vraag aan Tim waar dat staat in Drive)
5. Hij stelt jullie een hoop vragen: "wat vind jij echt een goede caption van Aspen?" en "wat moet er nooit in?" en "wie taggen we altijd?"
6. Antwoord eerlijk en gewoon. Geen goed of fout. Niet weten mag ook, dan denkt Barry mee.
7. Op het eind maakt 'ie een bestand: `brand-context-aspen-valley-enschede.md` in je `Lotte Co-work/brand-contexts/` mapje
8. Hij vraagt: "wil je dit delen met het team via GitHub?" Antwoord: ja (Tim wil dat ook). Daar bouwt 'ie dan op door.

**Daarna gaan we meteen testen** met de tweede skill (zie stap 8).

---

## 7. Hoe je het beste tegen Barry praat

Dit is het belangrijkste tip van de hele documentatie. Lees twee keer.

**Wees zo gedetailleerd mogelijk.** Echt waar. Je denkt soms: "dit weet 'ie wel". Hij weet niks. Hij leest letterlijk wat je schrijft. Hoe meer context, hoe beter het resultaat.

Slecht voorbeeld:

> "Maak een post voor zaterdag"

Beter voorbeeld:

> "Maak een post voor Aspen Valley Enschede voor zaterdag 25 mei. Het is een hardstyle-avond met DJ Vortex (@djvortex_official) en DJ Wave (@djwave). Sfeerimpressie, geen ticketpush, want we zijn bijna uitverkocht en het zou onnodig wervend overkomen. Carrousel format, 5 foto's, donker en energetisch. Caption in het Nederlands, max 6 regels."

Het tweede voorbeeld is langer, maar Barry levert dan in 1 keer iets wat klopt. Bij het eerste vraagt 'ie nog 10 dingen of raadt 'ie verkeerd.

**Stel je voor: je legt het uit aan een klein kind.** Niet omdat Barry dom is, maar omdat hij geen aannames maakt. Vertel het hele plaatje.

**De magische zin om aan elke eerste prompt toe te voegen:**

> "Stel zoveel mogelijk vragen voordat je begint."

Dit triggert Barry om eerst na te denken over wat 'ie nog niet weet en het aan jou te vragen, in plaats van iets te raden en het fout te doen. Dat scheelt enorm veel correctierondes. Doe het standaard, ook bij brand-mapper, ook bij posts maken, ook bij andere taken.

**Andere tips:**

- Als iets niet klopt: gewoon eerlijk zeggen. "Nee, dat is te kort." Of "die foto's vind ik niet leuk, zoek anders." Hij past zich aan.
- Als 'ie ergens vastloopt: vraag waar 'ie staat en wat 'ie verwacht. Hij legt 't uit.
- Casual praten mag. Hoeft niet formeel. "Joh, dit is niks, doe nog een keer met meer pit" werkt prima.
- Foutjes maken mag. Hij vergeet niks blijvend, je kunt altijd zeggen "nee wacht, vergeet wat ik net zei, ik bedoelde dit".

---

## 8. Direct na Aspen Valley: testen met social-media-poster

Zodra brand-mapper klaar is, draaien we meteen de tweede skill om te checken of alles goed werkt. In dezelfde chat (of een nieuwe, maakt niet uit, Barry onthoudt 't) typ je:

> "Barry, maak een test-post voor Aspen Valley Enschede voor komende zaterdag. Sfeerbeeld, ticketpush is OK want we hebben nog veel tickets. Stel zoveel mogelijk vragen voordat je begint."

Hij gaat dan:

1. Het zojuist gemaakte brand-context bestand lezen
2. De Instagram-feed van Aspen kort scannen om te kijken wat recent al gepost is
3. Naar Google Drive gaan en foto's zoeken van de laatste editie
4. Controleren of ze al gepost zijn (geen dubbelen)
5. 4 tot 6 foto's downloaden naar een werkmap op je Mac
6. 2 tot 3 captionvarianten schrijven
7. Een checklist geven met alle posts-regels (likes uit, wie taggen, etc.)

**Resultaat:** je hebt foto's en captions klaarstaan om te posten op Instagram. Je opent gewoon de Instagram-app of de browser, uploadt de foto's, plakt de caption die je het mooist vindt, en klaar.

Bij dit eerste testje gaat misschien iets niet helemaal goed. Dat is OK. We bespreken samen wat aangepast moet en passen het direct aan in de brand-context.

---

## 9. Wat Barry NIET kan (verwachtingen managen)

Belangrijk om vooraf te weten, zodat je niet teleurgesteld bent:

- **Barry post niet op Instagram voor je.** Hij levert foto's + caption. Jij uploadt en publiceert.
- **Barry bewerkt geen foto's.** Geen filters, geen CapCut-werk, geen Photoshop. Dat blijf jij doen.
- **Barry maakt geen video's of reels.** Stills wel, video niet (nog niet).
- **Barry maakt geen stories met overlays of stickers.** Sticker-werk doe jij in de IG app.
- **Barry beantwoordt geen DM's.** Live response is jouw werk.
- **Barry weet niets van Aspen Valley voordat je 'm in kaart hebt gebracht.** Eerst brand-mapper, dán pas posten.

Voor wat hij wel doet, ben je goed bezig.

---

## 10. Eerste dagen: tips uit de praktijk

- **Pak één zaak per keer.** Niet Aspen + Fifth Avenue tegelijk inrichten. Eerst Aspen helemaal klaar, dan Fifth. Anders raakt iedereen (jij en Barry) in de war.
- **Maak fouten.** De eerste dag is leren. Niets is definitief. Brand-contexts kunnen we altijd aanpassen.
- **Als iets raar gaat, zeg het hardop tegen Barry.** "Hé wacht, dat klopt niet, kun je opnieuw beginnen?" werkt prima.
- **Houd het werkmapje opgeruimd.** Niet nodig om alles weg te gooien, maar als je iets niet meer nodig hebt: weg ermee. Barry doet anders niet altijd handig.
- **Vraag domme vragen.** Echt waar. "Barry, wat doe je nu eigenlijk?" is een goede vraag. Hij legt het uit.
- **Vier de wins.** Eerste keer een caption die in 1 keer goed is = champagne. Niet flauw. Dit is nieuw voor iedereen.

---

## 11. Hulp nodig?

Volgorde van proberen:

1. **Vraag 't aan Barry zelf.** Hij weet vaak waarom iets niet werkt. "Hé Barry, je deed net X, dat ging fout, wat ging er mis?"
2. **Lees deze file opnieuw.** Vaak staat het antwoord hier en het was even ontschoten.
3. **Bel of app Tim of Niek.** Geen drempel. Wij verwachten dat je dingen niet weet, dat is normaal.
4. **Bij echte bugs:** maak een screenshot van wat er fout gaat, stuur naar Tim. Dan kan 'ie het patchen in de skill.

---

## 12. Hoe het straks gaat werken voor jou

Vooruitkijkend, hoe een normale werkweek er straks uit ziet:

**Maandag ochtend:** Je opent Barry, check je `Lotte Co-work` mapje. Eventueel kijk je in je memory wat de laatste status was. Daarna pak je de eerste post van de week. Bijvoorbeeld: weekendrecap voor Aspen Valley.

**Een post maken:** Je typt iets als "Barry, maak weekendrecap voor Aspen voor de feed, carrousel, 4 foto's, nadruk op de sfeer". Barry levert binnen 5-10 minuten foto's + caption. Jij review, eventueel feedback ("caption te lang, halveer 'm"). Klaar in 15 min.

**Een nieuwe zaak toevoegen:** Doe je 1 keer voor elke zaak in een sessie van 30-45 min. Daarna staat 'ie permanent in onze toolkit en kun je er voortaan dagelijks posts voor maken in 10-15 min.

**Per week verwachten we:** dat je sneller en makkelijker werkt dan voor je wereldreis. Daardoor heb je tijd over voor het leuke werk: strategie, campagnes, contentplanning, brainstormen.

---

## Welkom (nog een keer)

Welkom terug. We hebben er zin in om met je te werken. Mocht je iets willen veranderen aan deze workflow of aan Barry zelf, zeg het. Niks ligt vast. Alles wat we hebben gebouwd, kunnen we aanpassen aan hoe jij het beste werkt.

Veel succes met de eerste sessie.

— Tim, Niek & Barry
