# Filstruktur

Beskriver katalogstrukturen för repot. Används som referens vid omstrukturering och vid tillkomst av nytt material.

---

## Toppnivå

```
00. Arbetsmaterial/
01. Publicerat/
```

Gränsen är skarp: allt under `00. Arbetsmaterial/` är intern arbetsyta – utkast, noter, resonemang. Allt under `01. Publicerat/` är färdigt material avsett att läsas.

Projektinfrastruktur (`CLAUDE.md`, `STYLEGUIDE.md`) ligger kvar i roten.

---

## 00. Arbetsmaterial/

Intern arbetsyta. Speglar i möjligaste mån numreringen under `01. Publicerat/` – material som hör hemma i exempelvis `80. Äventyr/` när det är klart ligger under samma mappnamn i Arbetsmaterial. Det gör flytten till Publicerat trivial.

Där en direkt mappning inte är naturlig (stöddokument, etymologier, resursfiler, vision) ligger materialet löst eller i egna mappar utan krav på nummermatchning.

### Exempel på mappning Arbetsmaterial → Publicerat

| Arbetsmaterial | Publicerat |
|---|---|
| `10. Världsbok/` | `01. Publicerat/10. Världsbok/` |
| `11. Regioner/` | `01. Publicerat/11. Regioner/` |
| `20. Arkivet/` | `01. Publicerat/20. Arkivet/` |
| `30. Spelledarboken/` | `01. Publicerat/30. Spelledarboken/` |
| `80. Äventyr/` | `01. Publicerat/80. Äventyr/` |
| `90. Regelbok/` | `01. Publicerat/90. Regelbok/` |

---

## 01. Publicerat/

Numrering följer kontoplansprincipen: relaterat material klustrar sig i tiotal, med luft för framtida tillägg inom varje kluster.

### 10. Världsbok
Globalt och kosmologiskt material – det alla i världen vet. Kosmologi, tideräkning, Prima-översikt, gemensamma koncept. Skrivet som encyklopedi, ingen specifik avsändare.

### 11. Regioner
Geografiskt nedbrutet material i Hârn-stil. Hierarkin kan vara hur djup som helst: kontinent → region → stad → by. Varje nivå är en mapp; en sourcebook om en enskild stad är en fil i rätt undermapp.

```
11. Regioner/
    Ardenar/
        Nordmark/
        Meridia/
        ...
    Kyrathis/
    Serthara/
    Ythea/
    Aeloria/
```

*(12–19 ledigt för besläktat världsboksmaterial)*

### 20. Arkivet
Edrion Lomars samling – brev, krönikor, observationsloggar, marginalanteckningar. Organiserat efter dokumenttyp och proveniens, inte geografi. Spänner över hela världen.

*(21–29 ledigt)*

### 30. Spelledarboken
Material riktat till spelledaren: hemligheter, modulverktyg, råd om hur arkivet används i spel.

*(31–79 ledigt)*

### 80. Äventyr
Färdiga äventyrsmoduler.

*(81–89 ledigt)*

### 90. Regelbok
Regler för magi, folkslag, yrken och övrig spelmekanik. Placerad sist – världen är kärnan, reglerna är verktyget.

*(91–99 ledigt)*
