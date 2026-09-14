# Úloha 9: Práca s vetvami (Branches) a Pull Request

## 🎯 Cieľ úlohy
Pochopiť koncept vetvenia (**Branching**): ako vyvíjať novú funkciu izolovane od hlavného kódu (`main`), ako publikovať vetvu na GitHub a ako vytvoriť **Pull Request (PR)**.

---

## 🧰 Čo potrebuješ
* Aplikáciu **GitHub Desktop** alebo **JetBrains IDE**
* Webový prehliadač s repozitárom na GitHub.com

---

## 📝 Postup krok za krokom

1. **Vytvorenie novej vetvy cez GitHub Desktop:**
   * Otvor **GitHub Desktop**.
   * Hore v stredovom paneli klikni na **Current branch: main**.
   * Klikni na tlačidlo **New branch**.
   * Zadaj názov novej vetvy: `feature-kalkulacka` (používaj formát bez diakritiky s pomlčkami).
   * Uisti sa, že je vybrané *Based on: main* a klikni na **Create branch**.

   > *(Tip pre JetBrains IDE: Vetvu vytvoríš kliknutím na názov vetvy `main` v pravom dolnom rohu stavového riadku -> **New Branch...**).*

2. **Vykonanie zmeny v novej vetve:**
   * Otvor projekt v editore alebo IDE.
   * Vytvor nový súbor `kalkulacka.txt` a napíš doň jednoduchý text:
     ```text
     Funkcia jednoduchej kalkulačky:
     1 + 1 = 2
     2 * 2 = 4
     ```
   * V GitHub Desktop uvidíš zmenu na novej vetve.
   * Do commit správy napíš: `feat: pridanie prototypu kalkulačky`.
   * Klikni na **Commit to feature-kalkulacka**.

3. **Publikovanie vetvy na GitHub (Publish):**
   * V hornom paneli GitHub Desktop sa objaví tlačidlo **Publish branch**.
   * Klikni naň – Git odošle novú vetvu aj s commitom na server GitHubu.

4. **Vytvorenie a schválenie Pull Requestu:**
   * Po odoslaní ti GitHub Desktop priamo v okne ponúkne modré tlačidlo **Preview Pull Request** alebo **Create Pull Request**.
   * Klikni naň – v prehliadači sa otvorí stránka GitHubu s predvyplneným Pull Requestom.
   * Skontroluj, že zdrojová vetva je `feature-kalkulacka` a cieľová vetva je `main` (`base: main <- compare: feature-kalkulacka`).
   * Klikni na zelené tlačidlo **Create pull request**.
   * Keďže si vlastník repozitára, rovno môžeš zmeny schváliť:
     Klikni na **Merge pull request** a následne na **Confirm merge**.

---

## ✅ Ako overiť správnosť
* Na GitHube sa pri Pull Requeste objaví fialový štítok **Merged**.
* Prejdi na hlavnú stránku repozitára do vetvy `main` – súbor `kalkulacka.txt` sa stal súčasťou hlavnej vetvy!
* V GitHub Desktop sa prepni späť na vetvu `main` a klikni na **Pull origin** – súbor `kalkulacka.txt` sa stiahne aj do tvojej lokálnej vetvy `main`.

---

## ❓ Bonusová otázka na zamyslenie
> Prečo sa v profesionálnych softvérových firmách zásadne zakazuje commitovať priamo do vetvy `main` a každý kód musí prejsť cez vetvu a Pull Request (Code Review)?

---

[⬅️ Predchádzajúca úloha](08-gitignore.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Kolaborácia a Merge Conflict ➡️](10-kolaboracia-a-merge-conflict.md)

