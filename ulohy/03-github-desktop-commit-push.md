# Úloha 3: Prvý Commit a Push cez GitHub Desktop

## 🎯 Cieľ úlohy
Pochopiť základný cyklus práce v Gite: úprava súboru na disku, zobrazenie zmien (diff), vytvorenie lokálneho záznamu (**Commit**) a odoslanie zmien na server (**Push**).

---

## 🧰 Čo potrebuješ
* Aplikáciu **GitHub Desktop**
* Ľubovoľný textový editor (Poznámkový blok, VS Code, Notepad++ a pod.)
* Dokončenú [Úlohu 2](02-github-desktop-setup-klonovanie.md)

---

## 📝 Postup krok za krokom

1. **Úprava súboru na disku:**
   * Otvor lokálny priečinok svojho repozitára `git-trening`.
   * Otvor súbor `README.md` v textovom editore.
   * Na koniec súboru pridaj napríklad tieto riadky:
     ```markdown
     ## O mne
     * **Autor:** Tvoje Meno a Priezvisko
     * **Trieda:** Tvoja trieda (napr. II.AI)
     * **Dátum:** Dnešný dátum
     ```
   * Súbor ulož (`Ctrl + S`) a zatvor editor.

2. **Kontrola zmien v GitHub Desktop:**
   * Otvor **GitHub Desktop**.
   * V ľavom paneli pod záložkou **Changes** uvidíš súbor `README.md` so zaškrtnutým políčkom.
   * V pravej časti uvidíš farebné zvýraznenie: zelené riadky so znamienkom `+` označujú novo pridaný text.

3. **Vytvorenie commitu (lokálne uloženie do histórie):**
   * V ľavom dolnom rohu nájdeš pole **Summary (required)**.
   * Zadaj výstižný názov commitu, napr.:
     `docs: pridanie informácií o autorovi do README`
   * Do poľa **Description** môžeš pridať doplňujúci popis.
   * Klikni na modré tlačidlo **Commit to main**.

4. **Odoslanie na GitHub (Push):**
   * Všimni si, že GitHub Desktop teraz hlási: `Push origin (1)` – zmena je zatiaľ len v tvojom počítači!
   * V hornom paneli klikni na tlačidlo **Push origin**.

---

## ✅ Ako overiť správnosť
* V GitHub Desktop uvidíš hlásenie: `No local changes` a `Last fetched just now`.
* Prejdi na záložku **History** v GitHub Desktop – uvidíš tam svoj nový commit so zadanou správou a časom.
* Otvor svoj repozitár v internetovom prehliadači na [GitHub.com](https://github.com) – v náhľade súboru `README.md` musí byť vidieť tvoje meno a trieda.

---

## ❓ Bonusová otázka na zamyslenie
> Prečo sa zmeny po kliknutí na **Commit to main** neobjavili hneď na webe GitHub.com? Aký je rozdiel medzi operáciou **Commit** a **Push**?

---

[⬅️ Predchádzajúca úloha](02-github-desktop-setup-klonovanie.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Nastavenie JetBrains IDE ➡️](04-jetbrains-setup-klonovanie.md)

