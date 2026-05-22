# Social Media Toolkit

> Universele social media skills voor Barry. Werkt voor elke nachtzaak, festival of horeca-concept op elk Claude-account.

![status](https://img.shields.io/badge/status-stable-green) ![versie](https://img.shields.io/badge/versie-1.0.0-blue)

## Wat zit erin

Twee skills die samen de hele social media workflow afdekken:

| Skill | Wat doet 'ie |
|---|---|
| `brand-mapper` | Brengt een nieuwe zaak volledig in kaart. Analyseert 25 Instagram posts, leest brandbook, extracten visuele identity, interviewt de gebruiker. Output: één markdown-bestand met alles wat de poster nodig heeft. |
| `social-media-poster` | Maakt complete posts (foto's + 2-3 captionvarianten + checklist) op basis van een brand-context bestand. Zoekt foto's in Drive, controleert op dubbelen, downloadt en levert ready-to-post op. |

## Voor wie

- Nightlife- en horecaconcepten met meerdere zaken
- Marketing-teams die per concept consistent willen posten
- Iedereen die niet handmatig 7 verschillende tone-of-voices wil onthouden

Werkt voor BWC, KO en elke andere organisatie waarvan de zaken hier in kaart zijn gebracht.

## Installatie

### Eenmalige setup in Claude (3 minuten)

1. Open de **Claude desktop app**
2. Ga naar **Customize**
3. Klik op **Browse plugins**
4. Tabblad **Personal**
5. Klik op het **plusje** (+)
6. Plak deze regel:

   ```
   BWC-Barry/social-media-toolkit
   ```

7. Bevestigen
8. Klik op **Install**
9. Klaar. Barry heeft nu beide skills paraat.

### Na de install

Probeer:

- "Barry, breng [zaak] in kaart" — start brand-mapper
- "Barry, maak een post voor [zaak] voor zaterdag" — start social-media-poster

## Workflow

```
┌─────────────────┐      ┌──────────────────────────┐      ┌───────────────────────┐
│  Nieuwe zaak    │────▶ │  brand-mapper            │────▶ │ brand-context-[slug] │
│  toevoegen      │      │  (eenmalig per zaak)     │      │ .md                   │
└─────────────────┘      └──────────────────────────┘      └───────────┬───────────┘
                                                                       │
                                                                       │ leest
                                                                       ▼
┌─────────────────┐      ┌──────────────────────────┐      ┌───────────────────────┐
│  Post-brief     │────▶ │  social-media-poster     │────▶ │ Foto's + captions +   │
│  van gebruiker  │      │  (elke post)             │      │ checklist klaar       │
└─────────────────┘      └──────────────────────────┘      └───────────────────────┘
```

## Brand-contexts

Brand-contexts worden in twee plekken opgeslagen:

1. **Lokaal** `~/Desktop/Claude Co-work/brand-contexts/` — meest recente versie voor de huidige gebruiker
2. **Team-shared** `plugins/social-media-toolkit/brand-contexts/` — gedeeld via deze marketplace

Wanneer de brand-mapper een nieuwe context maakt, vraagt 'ie of die naar de marketplace gepusht moet worden. Bij ja: commit + push, en alle team-leden krijgen 'm via de volgende plugin-update.

## Voor Tim: een skill of context updaten

1. Bewerk lokaal in `plugins/social-media-toolkit/skills/[skill-naam]/SKILL.md`
2. Bump het versienummer in `plugins/social-media-toolkit/.claude-plugin/plugin.json`
3. Commit en push:

   ```bash
   git add .
   git commit -m "update brand-mapper: nieuwe interview-vraag"
   git push
   ```

4. Team krijgt update automatisch bij eerstvolgende Cowork-start

## Structuur

```
social-media-toolkit/
├── README.md
├── .claude-plugin/
│   └── marketplace.json           ← marketplace metadata
└── plugins/
    └── social-media-toolkit/
        ├── .claude-plugin/
        │   └── plugin.json        ← plugin metadata
        ├── brand-contexts/        ← team-shared brand contexts
        │   ├── README.md
        │   └── brand-context-*.md
        └── skills/
            ├── brand-mapper/
            │   └── SKILL.md
            └── social-media-poster/
                └── SKILL.md
```

## Support

Iets werkt niet? Stuur Tim een bericht met een screenshot. Bij meerdere meldingen komt het in de FAQ.

---

**Gemaakt door Tim & Barry** · Werkt op alle Claude-accounts met Cowork-mode
