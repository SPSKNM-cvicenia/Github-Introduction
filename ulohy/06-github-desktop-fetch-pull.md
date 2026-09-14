# Úloha 6: Simulácia vzdialenej zmeny a Fetch & Pull v GitHub Desktop

## 🎯 Cieľ úlohy
Pochopiť prácu v tíme: nasimulovať zmenu kódu vykonanú iným používateľom (cez webové rozhranie GitHubu) a naučiť sa rozdiel medzi operáciami **Fetch** (overenie zmien) a **Pull** (stiahnutie a zlúčenie do lokálneho projektu).

---

## 🧰 Čo potrebuješ
* Internetový prehliadač s otvoreným repozitárom na [GitHub.com](https://github.com)
* Aplikáciu **GitHub Desktop** s naklonovaným projektom z [Úlohy 2](02-github-desktop-setup-klonovanie.md)

---

## 📝 Postup krok za krokom

1. **Simulácia kolegu (úprava súboru cez web):**
   * V prehliadači otvor repozitár `https://github.com/<tvoje-meno>/git-trening`.
   * V zozname súborov klikni na `pozdrav.txt` (vytvorený v úlohe 5).
   * V pravom hornom rohu súboru klikni na ikonu ceruzky (**Edit this file**).
   * Pridaj nový riadok na koniec súboru:
     ```text
     Tento riadok pridal môj kolega priamo cez webové rozhranie.
     ```
   * Klikni na zelené tlačidlo **Commit changes...**.
   * Zadaj správu (napr. `docs: doplnenie pozdravu z webu`) a potvrď tlačidlom **Commit changes**.

2. **Overenie vzdialených zmien v GitHub Desktop (Fetch):**
   * Prejdi do aplikácie **GitHub Desktop** (kde máš otvorený repozitár `git-trening`).
   * Všimni si, že GitHub Desktop zatiaľ o zmene na webe nevie.
   * V hornom paneli klikni na tlačidlo **Fetch origin** (alebo stlač `Ctrl + Shift + T`).
   * Git sa spojí so serverom GitHubu a zistí, či pribudli nové commity.

3. **Stiahnutie zmien do lokálneho počítača (Pull):**
   * Po dokončení fetchu sa tlačidlo zmení na modré:
     **Pull origin** s počítadlom `Pull 1 commit from origin`.
   * Klikni na tlačidlo **Pull origin**.

---

## ✅ Ako overiť správnosť
* GitHub Desktop vypíše, že repozitár je aktuálny (`No local changes`).
* Prejdi do záložky **History** v GitHub Desktop – na vrchu vidíš commit, ktorý si vytvoril na webe.
* Otvor súbor `pozdrav.txt` v prieskumníkovi súborov na disku v priečinku pre GitHub Desktop – riadok pridaný cez web v ňom už je prítomný!

---

## ❓ Bonusová otázka na zamyslenie
> Prečo Git automaticky nestiahne nový kód hneď pri operácii **Fetch**? Prečo existujú dva samostatné kroky (**Fetch** a **Pull**)?

---

[⬅️ Predchádzajúca úloha](05-jetbrains-commit-push.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Update Project v JetBrains ➡️](07-jetbrains-fetch-pull.md)

