# Úloha 2: Prihlásenie a klonovanie cez GitHub Desktop

## 🎯 Cieľ úlohy
Prihlásiť sa do samostatného grafického klienta **GitHub Desktop** a stiahnuť si vzdialený repozitár (`git-trening`) z GitHubu do svojho počítača (tzv. **klonovanie**).

---

## 🧰 Čo potrebuješ
* Aplikáciu **GitHub Desktop**
* Internetové pripojenie
* Hotovú [Úlohu 1](01-vytvorenie-repozitara.md)

---

## 📝 Postup krok za krokom

1. **Prihlásenie do GitHub Desktop:**
   * Spusti aplikáciu **GitHub Desktop**.
   * Ak ju spúšťaš prvýkrát, aplikácia ti priamo ponúkne prihlásenie.
   * Ak už je spustená, prejdi do horného menu:
     `File -> Options... -> Accounts`.
   * Pri položke **GitHub.com** klikni na tlačidlo **Sign in**.
   * Vyber možnosť **Continue with browser**.
   * V otvorenom okne prehliadača klikni na zelené tlačidlo **Authorize desktop** (ak nie si prihlásený, najprv zadaj svoje prihlasovacie údaje do GitHubu).

2. **Klonovanie repozitára:**
   * Po úspešnom prihlásení klikni na úvodnej obrazovke na **Clone a repository from the Internet...** (alebo v menu `File -> Clone repository...`).
   * Zvoľ záložku **GitHub.com**.
   * Do vyhľadávacieho poľa napíš názov svojho repozitára: `git-trening`.
   * V spodnej časti skontroluj položku **Local path** (cesta na tvojom disku, kam sa priečinok stiahne, napr. `C:\Users\tvoje_meno\Documents\GitHub\git-trening`).
   * Klikni na tlačidlo **Clone**.

---

## ✅ Ako overiť správnosť
* V ľavom hornom rohu aplikácie GitHub Desktop svieti:
  * **Current repository:** `git-trening`
  * **Current branch:** `main`
* Klikni v hornom menu na `Repository -> Show in Explorer` (alebo stlač `Ctrl + Shift + F`). Otvorí sa priečinok, v ktorom nájdeš súbor `README.md` a skrytý priečinok `.git`.

---

## ❓ Bonusová otázka na zamyslenie
> Aký je rozdiel medzi **naklonovaním** repozitára cez Git a obyčajným stiahnutím projektu vo formáte `.zip`? Prečo je priečinok `.git` kľúčový?

---

[⬅️ Predchádzajúca úloha](01-vytvorenie-repozitara.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Prvý Commit a Push ➡️](03-github-desktop-commit-push.md)

