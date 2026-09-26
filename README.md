# kodakondsuse-eksam

Free offline-friendly drill trainer for the Estonian citizenship (kodakondsuse) constitution & citizenship-act exam.

**Live demo:** https://upyrj.github.io/eesti-kodakondsuse-eksam/

> **Disclaimer (EN / ET / RU below):** The question bank is a community/study artefact and is **not** kept up to date with official exam changes. Anyone may fork, modify, or republish as they wish. This is **not** an official [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid)/state product. For the real exam, rely on official law texts ([PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008)) and official materials.

---

## English

### What it is
A static, mobile-first practice site for the **Eesti Vabariigi põhiseaduse ja kodakondsuse seaduse tundmise eksam** (citizenship exam on the Constitution and Citizenship Act). Estonian questions first; Russian debrief after you answer. Progress stays in your browser (`localStorage`).

### Try it
- **Live:** https://upyrj.github.io/eesti-kodakondsuse-eksam/
- **This repository:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Run locally
No build step required for day-to-day use:

```bash
# option A — open the file
open index.html   # or double-click / xdg-open

# option B — any static server
python3 -m http.server 8080
# then http://127.0.0.1:8080
```

Works on [Cloudflare Pages](https://pages.cloudflare.com/), [Netlify](https://www.netlify.com/), [GitHub Pages](https://pages.github.com/), or any static host: publish the repo root (`index.html` + `data/`).

### Question bank
- Inlined in `index.html` as `QUESTIONS` (what the live site runs).
- Same bank as a file: `data/drill-bank-quality-v3.json` (525 items).

### Rebuild (brief)
There is no separate public build pipeline in this package. To change questions:

1. Edit `data/drill-bank-quality-v3.json` (keep the existing item schema).
2. Re-embed into `index.html` (replace the `QUESTIONS = [ ... ]` array with the updated JSON), **or** keep using the inlined copy and treat `data/` as the editable source of truth before embed.
3. Refresh in the browser.

### Contribute / fork
Fork freely. Improvements to wording, distractors, accessibility, or packaging are welcome. Please keep the disclaimer visible.

### Provenance / results
Built with practice items and a consultation presentation used in citizenship-exam prep. Three people who trained with this material scored **23–24 out of 24** on the official exam on **26 September 2026**.

### Credits / sources
- [Denis Ivanov](https://ivanov.in) — publisher of this site and bank
- [Grok Bot Tõnu](https://x.ai/bot) — Cursor/Grok Bot assistant that coached and built the drill with [Denis](https://ivanov.in)
- Law references: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); exam context: [Harno materials](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) and [Integratsiooni Sihtasutus exam-prep materials](https://integratsioon.ee/kodakondsuseksam) (not affiliated)

### Disclaimer
The question bank is a **community/study artefact** and is **not** kept up to date with official exam changes. Anyone may fork, modify, or republish. This is **not** an official [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) or Estonian state product. For the real exam, rely on official law texts ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) and official materials.

### License
MIT License — see [`LICENSE`](LICENSE).

---

## Eesti

### Mis see on
Tasuta, võrguühenduseta sobiv treeningleht **Eesti Vabariigi põhiseaduse ja kodakondsuse seaduse tundmise eksami** (kodakondsuseksam) harjutamiseks. Küsimus eesti keeles; pärast vastust vene keeles selgitus. Progress salvestub brauserisse (`localStorage`).

### Proovi
- **Live:** https://upyrj.github.io/eesti-kodakondsuse-eksam/
- **See repositoorium:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Kohalik käivitamine
Ehitust pole vaja:

```bash
open index.html
# või
python3 -m http.server 8080
```

Sobib [Cloudflare Pages](https://pages.cloudflare.com/) / [Netlify](https://www.netlify.com/) / [GitHub Pages](https://pages.github.com/) / mis tahes staatiline host (juur: `index.html` + `data/`).

### Küsimustepank
- Sisseehitatud `index.html`-is (`QUESTIONS`).
- Failina: `data/drill-bank-quality-v3.json` (525 küsimust).

### Ümbertegemine (lühidalt)
Avalikku eraldi build-skripti selles paketis pole. Muuda panka `data/` all, seejärel asenda `QUESTIONS = [ ... ]` massiiv `index.html`-is või hoia `data/` allikatõena enne sisseehitamist.

### Panusta / fork
Forki vabalt. Parandused (sõnastus, distraktorid, ligipääsetavus, pakendamine) on oodatud. Palun jäta disclaimer nähtavaks.

### Päritolu / tulemused
Kasutasime treeningülesandeid ja konsultatsiooni esitlust kodakondsuseksami ettevalmistusest. Kolm inimest, kes materjaliga treenisid, said ametlikul eksamil **26. septembril 2026** **23–24 punkti 24-st**.

### Tunnustus / allikad
- [Denis Ivanov](https://ivanov.in) — saidi ja panga väljaandja
- [Grok Bot Tõnu](https://x.ai/bot) — Cursor/Grok Bot abiline, kes treenis ja ehitas driilli koos [Denisega](https://ivanov.in)
- Õigusviited: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); eksami kontekst: [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) materjalid ja [Integratsiooni Sihtasutuse eksamiks ettevalmistavad materjalid](https://integratsioon.ee/kodakondsuseksam) (seotud asutusega ei ole)

### Hoiatus (disclaimer)
Küsimustepank on **kogukonna/õppematerjal** ja seda **ei hoita** ametlike eksamimuudatustega sünkroonis. Igaüks võib forki teha, muuta või uuesti avaldada. See **ei ole** ametlik [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) ega riigi toode. Päriseksami jaoks tugine ametlikele seadustekstidele ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) ja ametlikele materjalidele.

### Litsents
MIT litsents — vaata faili [`LICENSE`](LICENSE).

---

## Русский

### Что это
Бесплатный офлайн-дружественный тренажёр к экзамену на знание **Конституции Эстонской Республики и Закона о гражданстве** (kodakondsuse eksam). Сначала вопрос по-эстонски; после ответа — разбор по-русски. Прогресс хранится в браузере (`localStorage`).

### Попробовать
- **Live:** https://upyrj.github.io/eesti-kodakondsuse-eksam/
- **Этот репозиторий:** https://github.com/upyrj/eesti-kodakondsuse-eksam

### Локальный запуск
Сборка не нужна:

```bash
open index.html
# или
python3 -m http.server 8080
```

Подойдёт [Cloudflare Pages](https://pages.cloudflare.com/) / [Netlify](https://www.netlify.com/) / [GitHub Pages](https://pages.github.com/) / любой статический хостинг (корень: `index.html` + `data/`).

### Банк вопросов
- Встроен в `index.html` (`QUESTIONS`).
- Отдельным файлом: `data/drill-bank-quality-v3.json` (525 вопросов).

### Пересборка (кратко)
Отдельного публичного build-скрипта в пакете нет. Правите банк в `data/`, затем заменяете массив `QUESTIONS = [ ... ]` в `index.html` (или держите `data/` источником истины до встраивания).

### Вклад / форк
Форкайте свободно. Правки формулировок, дистракторов, доступности и упаковки приветствуются. Пожалуйста, оставляйте дисклеймер на виду.

### Откуда взялось / результаты
Использовали тренировочные задания и презентацию с консультаций к экзамену. Трое, кто готовился по этому материалу, сдали официальный экзамен **26 сентября 2026** на **23–24 из 24**.

### Участники / источники
- [Denis Ivanov](https://ivanov.in) — издатель сайта и банка
- [Grok Bot Tõnu](https://x.ai/bot) — ассистент Cursor/Grok Bot, который вместе с [Денисом](https://ivanov.in) готовил и собрал тренажёр
- Ссылки на закон: [PS](https://www.riigiteataja.ee/akt/PS), [KodS](https://www.riigiteataja.ee/akt/126062025008); контекст экзамена: материалы [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) и [материалы Integratsiooni Sihtasutus для подготовки к экзамену](https://integratsioon.ee/kodakondsuseksam) (официальной аффилиации нет)

### Отказ от ответственности (disclaimer)
Банк вопросов — **учебный/сообщественный материал** и **не синхронизируется** с официальными изменениями экзамена. Любой может форкнуть, менять или перепубликовать. Это **не** официальный продукт [Harno](https://www.harno.ee/eksamid-testid-ja-uuringud/eksamid-testid-ja-lopudokumendid/kodakondsuseksamid) или государства. Для настоящего экзамена опирайтесь на официальные тексты законов ([**PS**](https://www.riigiteataja.ee/akt/PS), [**KodS**](https://www.riigiteataja.ee/akt/126062025008)) и официальные материалы.

### Лицензия
Лицензия MIT — см. файл [`LICENSE`](LICENSE).

---

## Layout

```
kodakondsuse-eksam-oss/
  index.html                      # static app (bank inlined)
  data/drill-bank-quality-v3.json # same bank as file
  README.md                       # EN + ET + RU
  LICENSE                        # MIT License
  .gitignore
```
