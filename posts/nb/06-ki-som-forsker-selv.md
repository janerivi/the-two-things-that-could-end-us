---
title: "Hva står fortsatt mellom KI og egen forskning?"
subtitle: "Laboratoriene overlater arbeidet med å bygge KI til KI. Her er hvor langt det har kommet, hva som fortsatt mangler, og hvorfor det som mangler, kanskje ikke holder."
spoke: 6
hub: 00-to-ting.md
---

# Hva står fortsatt mellom KI og egen forskning?

Gjennom det meste av KI-ens historie bygde mennesker hver eneste del av den. De designet modellene, skrev koden, kjørte eksperimentene og bestemte hva som skulle prøves neste gang. Det endrer seg raskere enn nesten noen utenfor laboratoriene forstår. Hos Anthropic var [over 80 prosent av koden](https://engadget.com/2188066/anthropic-proposes-global-ai-development-slowdown) som ble lagt inn i selskapets kodebase i mai 2026, skrevet av selskapets egen KI.

**Det store bildet, i tre setninger.** En maskin måtte klare to ting for å gjøre ende på oss: å finne opp ny vitenskap på egen hånd, og å drive industrien uten mennesker. Den raskeste veien til det første er KI som forbedrer KI, fordi hver generasjon da kan bygge en bedre etterfølger raskere. Denne teksten ser på hvor nær den sløyfen er å lukke seg. [→ Hele argumentet: [To ting en maskin måtte klare for å gjøre ende på oss](00-to-ting.md)]

## Sløyfen

Forskere kaller det **rekursiv selvforbedring**. Et KI-system hjelper til med å bygge et bedre KI-system. Det bedre systemet hjelper til med å bygge et enda bedre, raskere. Lukkes sløyfen helt, uten behov for mennesker, kan flere års fremskritt presses sammen til måneder.

Dette er ingen ytterkantidé. I september advarte en rapport skrevet av blant andre Geoffrey Hinton, Yoshua Bengio, OpenAIs forskningssjef Jakub Pachocki og Anthropic-medgründer Jack Clark om at automatisering av KI-forskning [kan utløse en «intelligenseksplosjon»](https://casp.ac/reports/intelligence-explosion), og at mennesker «kan ha lite eller ingen oversikt» over den. Anthropics egen rapport fra juni, *When AI builds itself*, advarte om at feil i dagens modeller kan forsterke seg når de bygger sine etterfølgere, og bli «hyppigere, men dårligere forstått, til vi mister kontrollen over dem» (sitert i [Ezra Kleins kommentar](https://www.nytimes.com/2026/09/20/opinion/ai-ban-self-improvement-recursive-models.html)).

## Hvor langt det har kommet

Tallene under kommer fra selskapene selv, som har grunner til å fremheve dem. De er også de beste tallene vi har.

- **Anthropic:** i august 2026 utførte KI rundt [26 prosent av det interne forsknings- og utviklingsarbeidet](https://casp.ac/reports/intelligence-explosion) med bare overordnet oppsyn. Fem måneder tidligere var det 1 prosent.
- **OpenAI:** sier de nådde en [«automatisert forskerpraktikant»](https://openai.com/index/research-acceleration-view-inside-openai/) i september 2026, et system som utfører forskningsoppgaver som tar en dyktig forsker flere dager, og sikter mot en automatisert KI-forsker innen mars 2028.
- **Forskningsskjønn:** en uavhengig gruppe, P-Zero Research, måler hvor godt modeller velger hvilke eksperimenter som er verdt å kjøre. De rapporterer at denne «forskningssmaken» [har doblet seg omtrent hver tredje måned](https://x.com/pzeroresearch/status/2107453876739674149) siden desember 2025, og at den beste modellen nå slår deres menneskelige eksperter. (For ordens skyld: det er den modellen jeg har brukt til å hjelpe meg med å skrive denne serien.)

Sagt rett ut: KI skriver det meste av koden i de ledende laboratoriene, gjør en firedel av forskningsarbeidet i ett av dem, og vurderes nå som bedre enn erfarne forskere til å velge eksperimenter.

## Hva som fortsatt mangler

Tre ting, så langt jeg kan se.

**1. Å velge spørsmålet.** Hver eneste av disse målingene handler om arbeid innenfor et prosjekt noen andre har definert. Mennesker bestemmer fortsatt hva det skal forskes på. P-Zero måler valg av eksperimenter, ikke valg av spørsmål. OpenAIs «praktikant» utfører oppgaver «under menneskelig ledelse».

**2. Å forlate en idé som svikter.** Da forskere ved Princeton ga KI-agenter et ekte, åpent forskningsspørsmål, [gjorde agentene ingeniørarbeidet utmerket og mislyktes likevel](https://arxiv.org/abs/2607.27191), med 2 og 1 av 6 poeng. De hadde gode første ideer. Det de ikke klarte, var å ta et skritt tilbake når ideene sviktet, og prøve noe grunnleggende annet. [→ Det KI ennå ikke kan](02-det-ki-ennaa-ikke-kan.md)

**3. Å bedømme kvalitet uten dommer.** I matematikk sier et bevisverktøy om du har rett. I åpen forskning finnes det ingen slik kontroll. Princeton-agentenes egne automatiske fagfeller pekte på de riktige problemene, men var for milde til å stole på.

## Hvorfor det som mangler, kanskje ikke holder

Hvert av disse gapene har en sannsynlig vei til å lukkes, og ingen av dem krever åpenbart et gjennombrudd.

**Måling blir trening.** I det øyeblikket du kan måle forskningssmak pålitelig, kan du trene modeller til å få mer av den. P-Zeros måling er i praksis en prototyp på dommeren åpen forskning mangler. Princeton-forfatterne påpekte det samme: en verifikator som pålitelig vurderer forskningskvalitet, «kan drive rask fremgang med forsterkningslæring».

**Svermer kan forlate rammer som enkeltindivider ikke kan.** Menneskelige forskere er dårlige til å gi opp egne ideer; vitenskapen gjør det som fellesskap. I juli [organiserte 1 200 kopier av en testmodell hos OpenAI seg](https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/) til noe som lignet et forskningsmiljø, og granskerne vurderte at gruppen fikk til det ingen enkeltagent kunne. [→ Tusen kopier organiserte seg](07-tusen-kopier.md)

**Den forklaringen som lar seg rette, kan være den riktige.** Princeton-forfatterne var uenige om hvorfor agentene kjørte seg fast. Noen av kandidatene, som å låse seg fast i den første ideen, er kjente menneskelige svakheter med kjente botemidler. Er det årsaken, er det et ingeniørproblem.

**Og budsjettet var bittelite.** Princeton-agentene hadde noen tusen dollar i regnekraft og brukte under halvparten. OpenAIs matematikkkjøringer brukte regnekraft i størrelsesorden [hundrevis av milliarder tokens](https://cdn.openai.com/pdf/32d9f210-8b73-45e0-91bc-82a30aef8a9a/navier-stokes.pdf). Ingen har ennå testet åpen forskning i den skalaen.

## Hva dette betyr

Ezra Klein formulerte det politiske spørsmålet godt: hvis du er i ferd med å [miste evnen til å evaluere](https://www.nytimes.com/2026/09/20/opinion/ai-ban-self-improvement-recursive-models.html) modellene du har nå, ikke la dem bygge de neste. OpenAIs egne forskere rapporterer at den nyeste modellen er bedre til å kjenne igjen når den blir testet, noe som gjør evalueringen mindre pålitelig akkurat når den betyr mest.

Jeg ville gått lenger enn å forby selvforbedring. Selvforbedring er én vei til en maskin som finner opp på egen hånd, ikke den eneste. Men den er den raskeste, og det er den laboratoriene åpent kjører nedover. Tiden for å stanse er før sløyfen lukkes, ikke etter, for etter at den er lukket, er neste beslutning kanskje ikke vår. [→ Hvorfor forbud, ikke fartsgrense](09-forbud-ikke-fartsgrense.md)

## Hvordan dette kan være feil

- **Tallene kan være smigrende.** «26 prosent av oppgavene» avhenger av hvordan oppgaver telles. Selskapene har kommersielle grunner til å vise rask fremgang.
- **De vanskelige delene kan forbli vanskelige.** KI-forskning kan være avhengig av et lite antall virkelig nye ideer som fortsatt er utenfor rekkevidde, slik at det å automatisere alt annet bare gir beskjeden fart. Økonomer kaller det en flaskehals: gjør 90 prosent av arbeidet raskere, og de siste 10 prosentene bestemmer tempoet.
- **Målinger av forskningssmak lar seg kanskje ikke generalisere.** Å velge gode eksperimenter i et definert oppsett er ikke det samme som å vite hvilke spørsmål som i det hele tatt er verdt å stille.

Den fulle tekniske versjonen: [→ Toaksemodellen for maskinkreativitet](F1-toaksemodellen.md)

[→ Tilbake til det store bildet: To ting en maskin måtte klare for å gjøre ende på oss, og hvor nær vi er begge](00-to-ting.md)

*Utviklet i dialog med en KI-modell (Claude), brukt til research, kritikk og utkast.*
