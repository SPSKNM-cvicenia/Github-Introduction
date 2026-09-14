# Úloha 4: Nastavenie a klonovanie v JetBrains IDE

## 🎯 Cieľ úlohy
Pripojiť svoj GitHub účet do integrovaného vývojového prostredia **JetBrains IDE** (Rider, IntelliJ IDEA, WebStorm, PyCharm a pod.) a stiahnuť repozitár priamo z prostredia IDE.

---

## 🧰 Čo potrebuješ
* Ľubovoľné **JetBrains IDE** (napr. JetBrains Rider, IntelliJ IDEA Ultimate/Community, PyCharm, WebStorm...)
* Dokončenú [Úlohu 3](03-github-desktop-commit-push.md)

---

## 📝 Postup krok za krokom

1. **Spustenie JetBrains IDE a otvorenie VCS okna:**
   * Spusti svoje JetBrains IDE.
   * Na úvodnej obrazovke (Welcome Screen) klikni na tlačidlo **Get from VCS** v pravom hornom rohu.
   * *(Ak už máš otvorený iný projekt, choď do horného menu: `Git -> Clone...` alebo `VCS -> Get from Version Control...`)*.

2. **Kontrola inštalácie Gitu v systéme:**
   * V okne skontroluj, či IDE nehlási: `Git is not installed`.
   * Pokiaľ takéto hlásenie vidíš, klikni priamo na modrý odkaz **Download and install** a počkaj, kým IDE Git automaticky stiahne a nakonfiguruje.

3. **Prihlásenie cez GitHub účet:**
   * V ľavom bočnom paneli okna klikni na záložku **GitHub**.
   * Klikni na možnosť **Log In via GitHub...** (alebo **Use Token...**).
   * Otvorí sa internetový prehliadač s prihlasovacou stránkou GitHubu.
   * Klikni na zelené tlačidlo **Authorize in GitHub**.
   * Po schválení uvidíš potvrdenie `You have been successfully authenticated`. Záložku v prehliadači môžeš zavrieť.

4. **Klonovanie projektu do nového priečinka:**
   * Po návrate do IDE uvidíš zoznam všetkých svojich repozitárov z GitHubu.
   * Nájdi a klikni na `git-trening`.
   * V poli **Directory** nastav cestu.
     > ⚠️ **POZOR:** Neklonuj do rovnakého priečinka, ktorý už používa GitHub Desktop! Nastav novú zložku, napr.:
     > `C:\Users\tvoje_meno\Documents\JetBrainsProjects\git-trening`
   * Klikni na tlačidlo **Clone**.

---

## ✅ Ako overiť správnosť
* JetBrains IDE otvorí pracovnú plochu projektu.
* V pravej dolnej lište vidíš vetvu `main` (alebo v hornom paneli vedľa ikony vetvy).
* V hornom paneli pribudli ikony pre Git:
  * ⬇️ Modrá šípka (Update Project / Pull)
  * ⬆️ Zelená fajka (Commit, prípadne modrá fajka podľa verzie IDE)
  * 📜 História / Push

---

## ❓ Bonusová otázka na zamyslenie
> Aké výhody má mať Git integrovaný priamo v prostredí IDE oproti používaniu externého klienta? Kedy je naopak vhodnejší samostatný klient ako GitHub Desktop?

---

[⬅️ Predchádzajúca úloha](03-github-desktop-commit-push.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Commit a Push v JetBrains IDE ➡️](05-jetbrains-commit-push.md)

