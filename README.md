# kodakondsuse-eksam

Drill trainer for the Estonian citizenship exam (Constitution + Citizenship Act).

**Live demo:** https://upyrj.github.io/eesti-kodakondsuse-eksam/

> **Disclaimer (EN / ET / RU below):** Study bank, not kept in sync with official exam changes. Fork and change freely. Not Harno / not the state. For the real exam use [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008), and official materials.

---

## English

### What it is
A static practice site for the **Eesti Vabariigi põhiseaduse ja kodakondsuse seaduse tundmise eksam**. Question in Estonian; Russian debrief after you answer. Progress stays in the browser (`localStorage`). No server.

### Links
- **Live:** https://upyrj.github.io/eesti-kodakondsuse-eksam/  
  On a phone: “Add to Home Screen” / “Install” (PWA).
- **Repository:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Run locally
No build step:

```bash
open index.html   # or double-click / xdg-open

python3 -m http.server 8080
# then http://127.0.0.1:8080
```

Works on [Cloudflare Pages](https://pages.cloudflare.com/), [Netlify](https://www.netlify.com/), [GitHub Pages](https://pages.github.com/), or any static host. Publish the repo root (`index.html`, `data/`; plus icons + manifest for PWA).

### Question bank
- What the live site runs: inlined in `index.html` as `QUESTIONS`.
- Same bank as a file: `data/drill-bank-quality-v3.json` (525 items).

### Editing the bank
No public build script here. Edit `data/drill-bank-quality-v3.json`, then replace the `QUESTIONS = [ ... ]` array in `index.html` (or treat `data/` as the source and embed when you ship).

### Fork
Fork freely. Wording, distractors, accessibility — welcome. Please keep the disclaimer visible.

### Where it came from
Built from practice items and a consultation presentation for exam prep. Three people who trained with this material scored **23–24 / 24** on the official exam on **26 September 2026**.

### Credits / sources
- [Denis Ivanov](https://ivanov.in) — site and bank
- [Grok Bot Tõnu](https://x.ai/bot) — Cursor/Grok Bot that built the drill with [Denis](https://ivanov.in)
- Law: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); exam context: [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) and [Integratsiooni Sihtasutus](https://integratsioon.ee/kodakondsuseksam) (not affiliated)

### Disclaimer
This is a **study** bank. It is **not** kept up to date with official exam changes and **not** a [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) or state product. Fork and change as you like. For the real exam, use the official law texts ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) and official materials.

### License
MIT — see [`LICENSE`](LICENSE).

---

## Eesti

### Mis see on
Staatiline treeningleht **Eesti Vabariigi põhiseaduse ja kodakondsuse seaduse tundmise eksami** (kodakondsuseksam) jaoks. Küsimus eesti keeles; pärast vastust vene keeles selgitus. Progress jääb brauserisse (`localStorage`). Serverit pole.

### Lingid
- **Live:** https://upyrj.github.io/eesti-kodakondsuse-eksam/  
  Telefonis: “Lisa avakuvale” / “Installi” (PWA).
- **Repositoorium:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Kohalik käivitamine
Ehitust pole vaja:

```bash
open index.html

python3 -m http.server 8080
# siis http://127.0.0.1:8080
```

Sobib [Cloudflare Pages](https://pages.cloudflare.com/), [Netlify](https://www.netlify.com/), [GitHub Pages](https://pages.github.com/) või mis tahes staatiline host. Avalda repo juur (`index.html`, `data/`; PWA jaoks ka ikoonid + manifest).

### Küsimustepank
- Live sait kasutab panka, mis on `index.html`-is (`QUESTIONS`).
- Sama pank failina: `data/drill-bank-quality-v3.json` (525 küsimust).

### Panga muutmine
Avalikku build-skripti pole. Muuda `data/drill-bank-quality-v3.json`, siis asenda `QUESTIONS = [ ... ]` massiiv `index.html`-is (või hoia `data/` allikana ja sisseehita enne avaldamist).

### Fork
Forki vabalt. Sõnastus, distraktorid, ligipääsetavus — oodatud. Jäta disclaimer nähtavaks.

### Päritolu
Tehtud treeningülesannete ja konsultatsiooni esitluse põhjal. Kolm inimest, kes selle materjaliga treenisid, said ametlikul eksamil **26. septembril 2026** **23–24 / 24**.

### Tunnustus / allikad
- [Denis Ivanov](https://ivanov.in) — sait ja pank
- [Grok Bot Tõnu](https://x.ai/bot) — Cursor/Grok Bot, kellega [Denis](https://ivanov.in) driilli kokku pani
- Seadused: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); eksami kontekst: [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) ja [Integratsiooni Sihtasutus](https://integratsioon.ee/kodakondsuseksam) (seotud ei ole)

### Hoiatus
See on **õppe**pank. Seda **ei hoita** ametlike eksamimuudatustega sünkroonis ja see **ei ole** [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) ega riigi toode. Forki ja muuda. Päriseksami jaoks kasuta ametlikke seadustekste ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) ja ametlikke materjale.

### Litsents
MIT — fail [`LICENSE`](LICENSE).

---

## Русский

### Что это
Тренажёр к экзамену на знание **Конституции ЭР и Закона о гражданстве** (kodakondsuse eksam). Вопрос по-эстонски, после ответа — разбор по-русски. Прогресс в браузере (`localStorage`), без сервера.

### Ссылки
- **Сайт:** https://upyrj.github.io/eesti-kodakondsuse-eksam/  
  На телефоне: «Добавить на экран» / Install — это PWA.
- **Репозиторий:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Как открыть у себя
Сборка не нужна:

```bash
open index.html

python3 -m http.server 8080
# затем http://127.0.0.1:8080
```

Подойдёт [Cloudflare Pages](https://pages.cloudflare.com/), [Netlify](https://www.netlify.com/), [GitHub Pages](https://pages.github.com/) или любой static host. Выкладывай корень репо (`index.html`, `data/`; для PWA ещё иконки и manifest).

### Банк вопросов
- Живой сайт крутит банк из `index.html` (`QUESTIONS`).
- Тот же банк файлом: `data/drill-bank-quality-v3.json` (525 штук).

### Как править банк
Отдельного build-скрипта нет. Правишь `data/drill-bank-quality-v3.json`, потом подставляешь массив `QUESTIONS = [ ... ]` в `index.html` (или считаешь `data/` источником и вшиваешь перед выкладкой).

### Форк
Форкайте как хотите. Правки формулировок, вариантов ответа, доступности — ок. Дисклеймер лучше оставить на виду.

### Откуда это
Собрано из тренировочных заданий и консультационной презентации к экзамену. Трое, кто готовился по этому материалу, **26 сентября 2026** сдали официальный экзамен на **23–24 из 24**.

### Кто и откуда
- [Denis Ivanov](https://ivanov.in) — сайт и банк
- [Grok Bot Tõnu](https://x.ai/bot) — ассистент, с которым вместе собирали тренажёр ([Denis](https://ivanov.in))
- Законы: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); контекст экзамена: [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) и [Integratsiooni Sihtasutus](https://integratsioon.ee/kodakondsuseksam) (мы с ними не связаны)

### Дисклеймер
Это **учебный** банк. Его **не** держат в актуальном виде под официальный экзамен, и это **не** продукт [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) / государства. Форкайте и меняйте. На настоящем экзамене опирайтесь на тексты законов ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) и официальные материалы.

### Лицензия
MIT — файл [`LICENSE`](LICENSE).
