# Úloha 10: Tímová kolaborácia a riešenie Merge Konfliktu v JetBrains IDE

## 🎯 Cieľ úlohy
Naučiť sa, ako do repozitára pozvať spolužiaka (**Collaborator**) a osvojiť si najdôležitejšiu pokročilú zručnosť: vyriešenie **Merge Konfliktu** (situácia, keď dvaja vývojári naraz upravia ten istý riadok kódu) pomocou vizuálneho 3-stĺpcového nástroja v **JetBrains IDE**.

---

## 🧰 Čo potrebuješ
* **JetBrains IDE** s projektom `git-trening`
* Internetový prehliadač s repozitárom na GitHub.com
* *(Voliteľne)* Spolužiaka s GitHub účtom

---

## 📝 Postup krok za krokom

### Časť A: Pridanie spolužiaka do repozitára (Spolupráca)
1. Na GitHub.com otvor svoj repozitár `git-trening`.
2. Klikni na hornú záložku **Settings**.
3. V ľavom menu klikni na **Collaborators** (môže si vyžiadať potvrdenie hesla).
4. Klikni na zelené tlačidlo **Add people**.
5. Vyhľadaj spolužiaka podľa mena alebo emailu a klikni na **Add <meno> to this repository**.
6. Spolužiakovi príde email / GitHub notifikácia, ktorú musí prijať (**Accept invitation**).

---

### Časť B: Nasimulovanie konfliktu
*(Tento krok môžeš vykonať buď so spolužiakom, alebo sám pomocou webu).*

1. **Zmena na GitHube (vzdialená zmena):**
   * V prehliadači na GitHub.com otvor súbor `pozdrav.txt`.
   * Klikni na ceruzku (**Edit this file**).
   * Zmeň **prvý riadok** súboru na tento presný text:
     ```text
     TOTO JE VERZIA OD MOJHO SPOLUZIAKA Z WEBU.
     ```
   * Ulož zmenu kliknutím na **Commit changes...**.

2. **Zmena v JetBrains IDE (lokálna zmena):**
   * Otvor **JetBrains IDE** s tým istým projektom.
   * **DÔLEŽITÉ:** Nerob Update/Pull!
   * Otvor lokálny súbor `pozdrav.txt`.
   * Uprav ten istý **prvý riadok** na úplne iný text:
     ```text
     TOTO JE MOJA VLASTNA LOKALNA VERZIA Z IDE.
     ```
   * Súbor ulož.
   * Otvor Commit panel (`Ctrl + K`), zaškrtni `pozdrav.txt`, napíš správu `test: moja lokálna úprava prvého riadku` a klikni na **Commit** (iba Commit, nie Commit and Push!).

---

### Časť C: Vyriešenie Merge Konfliktu v JetBrains IDE

1. **Vyvolanie konfliktu:**
   * Teraz, keď máš lokálny commit a na webe je iný commit meniaci ten istý riadok, klikni na modrú šípku **Update Project** (`Ctrl + T`).
   * Zvoľ *Merge incoming changes...* a potvrď.
   * IDE okamžite zahlási: **Conflicts detected during merge**.

2. **Použitie 3-stĺpcového Merge nástroja:**
   * V zozname konfliktných súborov klikni na modré tlačidlo **Merge...**.
   * Otvorí sa špecializované trojstĺpcové okno:
     * **Vľavo (Your version):** Tvoj lokálny kód z počítača.
     * **Vpravo (Incoming changes):** Kód zo servera (od spolužiaka / z webu).
     * **V strede (Result):** Výsledná verzia súboru, ktorá sa uloží.
   * Medzi stĺpcami uvidíš farebné šípky (`»` a `«`):
     * Kliknutím na šípku prenesieš daný riadok do stredu.
     * Môžeš do stredového stĺpca kliknúť a kód aj manuálne prepísať a skombinovať obe zmeny.
   * Keď je stredový stĺpec upravený k tvojej spokojnosti a neobsahuje žiadne červené konflikty, klikni dole na zelené tlačidlo **Apply**.

3. **Odoslanie vyriešeného stavu:**
   * Git vytvoril automatický tzv. **Merge Commit**.
   * V pravom hornom rohu klikni na zelenú fajku / Push šípku (alebo `Ctrl + Shift + K`) a odošli zmeny kliknutím na **Push**.

---

## ✅ Ako overiť správnosť
* V JetBrains IDE otvor okno **Git Log** (`Alt + 9`) – uvidíš, ako sa dve vetvy histórie spojili v jednom bode (Merge commit).
* Na [GitHub.com](https://github.com) v súbore `pozdrav.txt` je zobrazený vyriešený text bez akýchkoľvek chybových značiek ako `<<<<<<< HEAD`.

---

## ❓ Bonusová otázka na zamyslenie
> Čo sú to konštrukcie `<<<<<<< HEAD`, `=======` a `>>>>>>>` v súbore, ak niekto rieši merge konflikt bez grafického nástroja v obyčajnom textovom editore?

---

[⬅️ Predchádzajúca úloha](09-vetvy-a-pull-request.md) | [Späť na prehľad úloh](README.md)

