# Úloha 8: Ignorovanie nepotrebných súborov pomocou `.gitignore`

## 🎯 Cieľ úlohy
Naučiť sa, prečo a ako používať súbor `.gitignore`, aby si do repozitára omylom nenahral dočasné súbory, heslá, konfigurácie IDE či vygenerované binárne priečinky (`bin/`, `obj/`, `node_modules/`).

---

## 🧰 Čo potrebuješ
* **JetBrains IDE** alebo **GitHub Desktop** s projektom `git-trening`

---

## 📝 Postup krok za krokom

1. **Vytvorenie nechcených súborov na disku:**
   * Vo svojom projekte vytvor dva nové súbory:
     * `tajne_hesla.env` (predstavuje citlivé dáta, ktoré nikdy nesmú ísť na verejný GitHub).
     * `aplikacia.log` (predstavuje veľký dočasný súbor so záznamom chýb).
   * Do oboch napíš ľubovoľný text a ulož ich.

2. **Pridanie do `.gitignore` cez JetBrains IDE:**
   * V strome projektu naľavo (`Alt + 1`) klikni pravým tlačidlom myši na súbor `tajne_hesla.env`.
   * Zvoľ **Git -> Add to .gitignore -> .gitignore**.
   * Potvrď vytvorenie súboru `.gitignore` v koreňovom priečinku projektu.
   * Následne klikni pravým tlačidlom na súbor `aplikacia.log` a urob to isté, alebo priamo otvor vytvorený `.gitignore` a dopíš doň riadok:
     ```gitignore
     # Ignorované súbory
     tajne_hesla.env
     *.log
     ```

3. **Ako to funguje v GitHub Desktop (alternatíva):**
   * V aplikácii GitHub Desktop v zozname *Changes* stačí kliknúť pravým tlačidlom myši na ľubovoľný súbor a zvoliť **Ignore file** (alebo **Ignore all .log files**). GitHub Desktop automaticky pridá pravidlo do `.gitignore`.

4. **Commit a push samotného `.gitignore`:**
   * Otvor Commit panel (`Ctrl + K`).
   * Všimni si: Súbory `tajne_hesla.env` a `aplikacia.log` v zozname zmien **vôbec nie sú**! Zosiveli a Git ich ignoruje.
   * Jediný nový súbor pripravený na commit je `.gitignore`.
   * Zaškrtni ho, zadaj správu: `chore: nastavenie .gitignore pre citlivé a log súbory` a klikni na **Commit and Push**.

---

## ✅ Ako overiť správnosť
* V strome projektu majú súbory `tajne_hesla.env` a `aplikacia.log` zvyčajne tmavšiu/sivú farbu (označenie ignored).
* Otvor `tajne_hesla.env`, zmeň v ňom text a ulož ho.
* Pozri sa do zoznamu Git zmien (`Ctrl + K`) – Git vôbec nereaguje a neponúka súbor na commit.
* Na GitHub.com v prehliadači vidíš súbor `.gitignore`, ale citlivé súbory tam chýbajú.

---

## ❓ Bonusová otázka na zamyslenie
> Čo sa stane, ak pridáš pravidlo do `.gitignore` pre súbor, ktorý si už predtým v minulosti commitol a pushol na GitHub? Začne ho Git automaticky ignorovať, alebo je potrebné urobiť niečo navyše?

---

[⬅️ Predchádzajúca úloha](07-jetbrains-fetch-pull.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Vetvy a Pull Request ➡️](09-vetvy-a-pull-request.md)

