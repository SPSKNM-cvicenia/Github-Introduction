# Úloha 7: Synchronizácia a Update Project v JetBrains IDE

## 🎯 Cieľ úlohy
Naučiť sa stiahnuť novinky zo vzdialeného repozitára priamo v prostredí JetBrains IDE pomocou funkcie **Update Project (Pull)** a preskúmať históriu commitov v Git okne.

---

## 🧰 Čo potrebuješ
* **JetBrains IDE** s projektom `git-trening` z [Úlohy 5](05-jetbrains-commit-push.md)
* Internetový prehliadač s repozitárom na GitHub.com

---

## 📝 Postup krok za krokom

1. **Vytvorenie novej vzdialenej zmeny:**
   * Otvor svoj repozitár na [GitHub.com](https://github.com) v prehliadači.
   * Rozklikni súbor `README.md`, klikni na ikonu ceruzky (**Edit this file**).
   * Doplň nový riadok, napríklad:
     ```markdown
     > Aktuálny stav: Prebieha testovanie Git procesov.
     ```
   * Klikni na **Commit changes...** a potvrď zmenu.

2. **Vyvolanie aktualizácie v JetBrains IDE:**
   * Prejdi do svojho JetBrains IDE.
   * Všimni si, že v editore v `README.md` nový riadok zatiaľ nemáš.
   * V pravom hornom rohu IDE klikni na **modrú šípku smerujúcu nadol** (**Update Project**), alebo použi klávesovú skratku `Ctrl + T` (na macOS `Cmd + T`).
   * Zobrazí sa dialógové okno *Update Project*:
     * Zvoľ **Merge incoming changes into the current branch**.
     * Klikni na **OK**.

3. **Preskúmanie histórie (Git Log):**
   * V spodnom paneli klikni na kartu **Git** (alebo stlač klávesovú skratku `Alt + 9`).
   * V záložke **Log** uvidíš grafickú časovú os všetkých commitov:
     * Vidíš commity z GitHub Desktopu, commity z webu aj commity z IDE.
     * Kliknutím na ľubovoľný commit v zozname uvidíš vpravo presný zoznam zmenených súborov a konkrétne rozdiely (diff).

---

## ✅ Ako overiť správnosť
* V pravom dolnom rohu IDE sa zobrazí oznámenie: `Updated 1 file` (alebo `1 commit fetched and merged`).
* V otvorenom editore `README.md` sa okamžite objavil nový riadok, ktorý si zapísal cez web.

---

## ❓ Bonusová otázka na zamyslenie
> Čo robí voľba **Rebase** namiesto **Merge** v dialógu *Update Project*? V čom sa líši výsledná história commitov?

---

[⬅️ Predchádzajúca úloha](06-github-desktop-fetch-pull.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Ignorovanie súborov (.gitignore) ➡️](08-gitignore.md)

