# Úloha 5: Vytvorenie súboru a Commit & Push v JetBrains IDE

## 🎯 Cieľ úlohy
Vytvoriť nový kódový/textový súbor priamo v IDE, naučiť sa pracovať s panelom **Commit** v JetBrains a odoslať zmeny v jednom kroku cez **Commit and Push**.

---

## 🧰 Čo potrebuješ
* Otvorené **JetBrains IDE** s projektom `git-trening` z [Úlohy 4](04-jetbrains-setup-klonovanie.md)

---

## 📝 Postup krok za krokom

1. **Vytvorenie nového súboru v projekte:**
   * V strome projektu naľavo (panel *Project* / `Alt + 1`) klikni pravým tlačidlom na koreňový priečinok projektu.
   * Zvoľ **New -> File**.
   * Pomenuj súbor `pozdrav.txt` (alebo `Program.cs`, `main.py`, `index.js` podľa tvojho zamerania).
   * Ak sa zobrazí otázka *“Do you want to add the following file to Git?”*, klikni na **Add**.

2. **Napísanie obsahu:**
   * Do súboru napíš jednoduchý text alebo kód, napr.:
     ```text
     Ahoj! Tento súbor bol vytvorený v JetBrains IDE.
     Git v tomto prostredí funguje skvele.
     ```
   * Súbor ulož (`Ctrl + S`).

3. **Otvorenie Commit panelu:**
   * Klikni na zelenú fajku v hornom paneli, **alebo** stlač skratku `Ctrl + K` (na macOS `Cmd + K`), **alebo** otvor bočnú záložku **Commit** naľavo.
   * V zozname *Changes* skontroluj, či je zaškrtnutý súbor `pozdrav.txt`.

4. **Vyplnenie údajov a prvotná konfigurácia:**
   * Do poľa pre správu napíš:
     `feat: pridanie súboru pozdrav.txt`
   * *(Poznámka: Ak commituješ z tohto IDE prvýkrát, Git ťa môže požiadať o zadanie **Mena** a **Emailu**. Zadaj svoje meno a školský/GitHub email a potvrď kliknutím na **Set and commit**)*.

5. **Commit and Push:**
   * Namiesto samotného tlačidla *Commit* klikni na šípku na tlačidle a zvoľ **Commit and Push...** (alebo stlač `Ctrl + Alt + K`).
   * Zobrazí sa rekapitulačné okno **Push Commits**, kde vidíš vetvu `main -> origin: main` a zoznam commitov.
   * Klikni na modré tlačidlo **Push**.

---

## ✅ Ako overiť správnosť
* V spodnom stavovom riadku JetBrains IDE sa zobrazí bublina: `Pushed 1 commit to origin/main`.
* Otvor repozitár na [GitHub.com](https://github.com) – v zozname súborov vidíš nový súbor `pozdrav.txt` s tvojím commit popisom.

---

## ❓ Bonusová otázka na zamyslenie
> Aký je rozdiel medzi samotným tlačidlom **Commit** a kombinovanou akciou **Commit and Push**? Kedy by si ako vývojár zvolil radšej len Commit bez Pushu?

---

[⬅️ Predchádzajúca úloha](04-jetbrains-setup-klonovanie.md) | [Späť na prehľad úloh](README.md) | [Nasledujúca úloha: Fetch a Pull v GitHub Desktop ➡️](06-github-desktop-fetch-pull.md)

