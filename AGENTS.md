# Robotjagt – fælles udviklingsregler

## Projekt
Robotjagt er et browserbaseret spil, der udgives på https://keha.dk/robotjagt.

GitHub-repository: `kenh-zealand/robotjagt`.

Undersøg projektets eksisterende kode, struktur og afhængigheder, før du foretager ændringer.

## GitHub og udvikling
- `mobil` er den aktive udviklings- og udgivelsesgren.
- Udviklerne må arbejde direkte på `mobil`.
- Der kræves ikke Pull Requests eller godkendelse.
- `backup-stabil` er en sikkerhedskopi og må ikke ændres uden udtrykkelig tilladelse.
- `udvikling-soen` er en tidligere testgren og skal ikke bruges til almindelig udvikling.
- Kontrollér altid den aktive gren, før du ændrer kode.
- Brug aldrig force-push uden udtrykkelig tilladelse.

## Udgivelse
- Spillet udgives automatisk fra GitHub-grenen `mobil`.
- Push til `mobil` påvirker derfor det offentlige spil på keha.dk.
- Test ændringer før commit og push.
- Brug beskrivende commit-beskeder.
- Du må committe og pushe testede ændringer direkte til `mobil`, når brugeren har bedt om at implementere dem.
- Push ikke automatisk, hvis brugeren kun har bedt om analyse, forslag eller forklaring.

## Kodekvalitet
- Bevar eksisterende funktioner, medmindre ændringen kræver andet.
- Undgå unødvendig omskrivning af fungerende kode.
- Kontrollér funktionalitet på både computer og mobil.
- Undersøg afhængigheder og mulige sideeffekter.
- Forklar væsentlige ændringer.
- Angiv tydeligt, hvis noget ikke er testet.

## Sikkerhed og backup
- Beskyt eksisterende Git-historik.
- Ændr ikke `backup-stabil` uden tilladelse.
- Gem aldrig API-nøgler, adgangskoder eller tokens i GitHub.
- Ved fejl skal du undersøge Git-historikken og foreslå en sikker tilbageførsel.

## Samarbejde
Projektet udvikles fra forskellige computere og med forskellige AI-assistenter, herunder Claude Code og Cline.

Alle assistenter skal følge disse fælles regler.

## Forhåndsvisning og test
- Start den lokale testserver med `python3 -m http.server 8000`, hvis den ikke allerede kører.
- Brug Codespaces' forhåndsvisning på port 8000 til at teste spillet.
- Vis ændringer i browseren, før de udgives.
- Foretag ikke automatisk `git push` efter kodeændringer.
- Vent på brugerens besked om at udgive, før der pushes til `mobil`.
- Når ændringerne er godkendt af brugeren, må de committes og pushes direkte til `mobil`.

## Arbejdsgang for ændringer
- Foretag ændringen i Codespaces.
- Lad brugeren teste resultatet i forhåndsvisningen.
- Undlad at committe eller pushe ændringen, før brugeren udtrykkeligt beder om at udgive.
- Hvis brugeren afviser ændringen, fortryd kun de ændringer, der hører til den aktuelle opgave.
- Bevar alle tidligere godkendte ændringer.
- Udgiv aldrig automatisk en ændring på keha.dk, blot fordi en opgave er afsluttet.


