
# Vitaj na GitHube!

  

Asi si sa ešte s GitHubom nestretol (nestretla), to však nevadí. V tejto príručke Ti vysvetlíme, ako funguje **Git**, zameriame sa aj na dôležité pojmy ako **Commit** alebo **Pull Request**.

  

## Navigácia

*  [Základné pojmy](#zakladne_pojmy)
*  [Založenie repozitára](#zalozenie_repozitara)
*  [Setup / Commitovanie z Visual Studia](#commit_vs)
*  [Setup / Commitovanie z GitHub Desktop](#github_desktop)
*  [Setup / Commitovanie z Jetbrains Rider](#commit_rider)
*  [Setup / Commitovanie z terminálu](#commit_cmd)
*  [Kolaborácia medzi spolužiakmi](#kolaboracia)
*  [GitHub Student Developer Pack](#student_pack)
*  [Zdroje](#zdroje)

  

## Základné pojmy <a id= zakladne_pojmy>

  

**Git** - Git je open source nástroj, ktorý Ti umožní **sledovanie zmien** v súboroch. Je základnou technológiou, ktorú GitHub využíva.

  

**Repository** (**Repozitár**, skrátene **Repo**) - Repozitár je základným prvkom GitHubu. Dá sa povedať, že to je **priečinok**, v ktorom máš umiestnený svoj projekt. Tento priečinok obsahuje všetky súbory Tvojho projektu a ukladá **históriu všetkých zmien** každého súboru. Nemusíš byť jediným, kto má k repozitáru prístup, pretože repozitár môže mať viacerých spolupracovníkov. Repozitár môže byť **verejný** alebo **súkromný**.

  

**Commit** - Commit je nejaké **zoskupenie zmien** v projekte. Keď commituješ, Git vytvára **jedinečné ID**, ktoré Ti umožní uchovávať záznamy o týchto zmenách a aj to, **kto** a **kedy** danú zmenu vykonal.

  

**Organizácia** (**Organisation**) - GitHub Organizácia je ako profil, ku ktorému majú prístup **viacerí** užívatelia. V tejto organizácií si môžeš vytvárať repozitáre.

  

**Fork** - Fork je kópia repozirára iného používateľa, ktorá sa uloží medzi Tvoje repozitáre. Forky Ti umožnia voľne vykonávať zmeny v projekte **bez ovplyvnenia pôvodného repozitára**. Môžeš však otvoriť **Pull Request** v pôvodnom repozitári.

  

**Pull Request** - Pull Requesty sú zmeny v repozitári, ktoré navrhol používateľ a ktoré môžeš ako **vlastník** (alebo **spolupracovník**) pôvodného repozirára **prijať**, prípadne **odmietnuť**.

  

**Push** - Nahranie lokálnych zmien (ešte nie sú na GitHube), ktoré sa nachádzajú v **commitoch**, na **GitHub**.

  

**Pull** - Stiahnutie **aktuálnej verzie** repozitára z GitHubu, v prípade, že si nejaké súbory upravil, tak môže nastať konflikt (**Merge Conflict**), ktorý je nutné vyriešiť.
  


**Branch** - Branch je **vetva projektu**, ktorú môžeš pridať, ak chceš opraviť chybu alebo s niečím experimentovať, ale nechceš, aby ti to ovplyvnilo Tvoj projekt. Každý repozitár má **default branch**, ale môže obsahovať aj ďaľšie.

  

**Merge** - Merge je **zlúčenie** jednej branche do druhej za vykonania **Pull Requestu**.



**Merge Conflict** - Je stav, kedy existuje viacero **novších** verzií nejakého súboru v kóde a nie je zrejmé, ktorá verzia sa má použiť.

  

**Licencia** - Licencia je dôležitý súbor, ktorý Ti **povoľuje** alebo **zakazuje** využívať kódy iných užívateľov. Licencia môže obsahovať **podmienky** a kód pod touto licenciou môžeš legálne použiť iba vtedy, ak ich spĺňaš.

  

**IDE** - *Integrated development environment* - je **vývojové prostredie** v ktorom budeš pracovať.

  

**ReadMe** - Je to textový súbor obsahujúci informácie o repozitári. Keďže sa automaticky zobrazuje **pod repozitárom**, je zvyčajne prvým súborom, ktorý návštevník Tvojho repozitára uvidí. Tvorí sa v **MarkDowne**.

  

**.gitignore** - gitignore je súbor, ktorý špecifikuje, ktoré časti by sa nemali nahrávať spolu so zmenami v commite. Používa sa na **vyfiltrovanie zbytočných súborov**, napríklad tých, ktoré vytvorí IDE, prípadne **súborov s citlivými dátami**.

  

*Pozn.: Toto sú len základné pojmy. Odporúčame, aby si si prečítal(a) slovník z oficiálnej dokumentácie GitHubu: https://docs.github.com/en/get-started/quickstart/github-glossary*

  

## Založenie Repozitára <a id = zalozenie_repozitara>

  

1. V pravom hornom rohu, rozklikni **+** a klikni na **New Repository**.

  

![img1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo1.png  "Nové repo")

  

2. Pomenuj svoj repozirár, môžeš pridať aj popis, **readme** súbor, **.gitignore**, **licenciu** alebo zmeniť repozitár na **súkromný**. Následne klikni na **Create Repository**.

  

![img2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo2.png  "Nové repo")

  

## Setup / Commitovanie z Visual Studia <a id = commit_vs>

### Setup repozitára

Po inštalacií Visual Studia si musíš synchronizovať GitHub repozitár, aby si z neho mohol vytvárať commity.

1. Po otvorení Visual Studia zvoľ možnosť **Clone a repository**, ktorá sa nachádza v pravej časti okna.

![imgvs1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/1.png  "vs")

2. Tu zvoľ možnosť **GitHub**.

![imgvs2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/2.png  "vs")

3. Vyskočí na teba okno, v ktorom sa môžeš v pravej hornej časti prihlásiť kliknutím na **Sign in...**.

![imgvs3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/3.png  "vs")

![imgvs4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/4.png  "vs")

4. Po úspešnom prihlásení Ti Visual Studio sprístupní tvoje repozitáre.

![imgvs5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/5.png  "vs")

Po vybraní jedného z repozitárov sa Ti stiahne a môžeš ho upraviť alebo inak využívať.

  

### Commitovanie

Po úprave súborov musíš commitnúť zmeny.

1. Po úprave projektu Ti Visual Studio vypíše, koľko zmien sa vykonalo. Klikneš na ceruzku v pravom dolnom rohu s číslom (číslo symbolizuje kolko súborov sa zmenilo), otvorí sa Ti **GIT panel**.

  

![imgvs6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/6.png  "vs")

2. Vypíšeš popis commitu a zmáčneš **Commit All**.

![imgvs7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/7.png  "vs")

![imgvs8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/8.png  "vs")

3. Všimni si, že Visual Studio píše, že commit bol vytvorený lokálne - to znamená, že ešte nie je v tvojom repozitári na GitHube, ale len v Tvojom počítači. Ak ho chceš dať na GitHub, klikni na **Push**, a Visual Studio to pushne na GitHub.

![imgvs9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/9.png  "vs")

![imgvs10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/10.png  "vs")

  

### Sťahovanie zmien z GitHubu / Fetch

Zmeny, ktoré boli vykonané v Repozitári niekým iným, sa Ti automaticky nestiahnú, musíš si ich najskôr **fetchnúť** a potom **pullnúť**.

  

1. V Git paneli klikni na **Fetch**.

![imgvs11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/11.png  "vs")

  

2. Visual Studio Ti potom vypíše, že koľko commitov je potrebné stiahnuť, aby si mal najaktuálnejšiu verziu repozitára:

  

![imgvs12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/12.png  "vs")

3. Klikneš na **počet zmien** a následne na **Pull**.

  

![imgvs13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/13.png  "vs")

## Setup / Commitovanie z GitHub Desktop <a id = github_desktop>

Na rozdiel od ostatných **IDE**, GitHub Desktop je stand-alone GIT client, to znamená, že nemá prvky IDE (Compiler, code editor, ...) ale je určený len na commitovanie a iné GIT operácie. 

### Setup Repozitára
Po inštalacií GitHub Desktop si musíš ešte synchronizovať GitHub repozitár, aby si z neho mohol commitovať.

1. Naľavo klikneš na **Clone a repository from the Internet**
2. Následne zvolíš **GitHub.com** a klikneš na **Sign In** Potom v okne upozornujúcom na bezpečnosť klikni na **Continue with browser**.

![img_gh1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/1.png  "ghd")

![img_gh2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/2.png  "ghd")

![img_gh3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/3.png  "ghd")


4. V prehladači sa prihlás do GitHubu (ak ešte nie si) a klikni na **Authorize desktop**.

![img_gh4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/4.png  "ghd")

6. Napravo sa Ti zobrazia Tvoje repozitáre. Zvoľ si ten správny a klikni na **Clone [meno repozitára]** Vyber si, že kde ho chceš uložiť a klikni na **Clone**.

![img_gh5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/5.png  "ghd")

![img_gh6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/6.png  "ghd")

![img_gh7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/7.png  "ghd")

8. Tvoj repozitár sa práve naklonoval a môžeš začať pracovať.

![img_gh8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/8.png  "ghd")


### Commitovanie
Po úprave súborov je potrebné vykonať **commit**. GitHub Desktop Ti automaticky sleduje zmeny v súboroch a pri každej zmene ich vypíše na panel v ľavej časti.

1. V ľavom dolnom roku vypíš názov commitu prípadne popis a klikni na **Commit to master**.

![img_gh9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/9.png  "ghd")

2. Všimni si, že Tvoj commit ešte nie je na GitHube, a GitHub Desktop píše, že je k dispozíci jeden (alebo viacero) commitov, ktoré ešte neboli **pushnuté** na Github  - to znamená, že dané commity ešte nie sú v Tvojom repozitári na GitHube, ale len v Tvojom počítači. Ak ich chceš dať na GitHub, klikni na  **Push origin**, a Github Desktop to automaticky pushne na GitHub.

![img_gh10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/10.png  "ghd")

### Sťahovanie zmien z GitHubu / Fetch
Zmeny, ktoré boli vykonané v repozitári niekým iným, sa Ti automaticky nestiahnú, musíš si ich najskôr **fetchnúť** a potom **pullnúť**.

1. Na paneli hore klikni na **Fetch Origin**. Toto overí stav, v ktorom sa nachádza repozitár a či je k dispozicií novší commit.

![img_gh11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/11.png  "ghd")

2. V prípade, že je k dispozícií novší commit, zobrazí sa Ti možnosť **pullnuť** zmeny. Pullni ich kliknutím na **Pull origin**.

![img_gh12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/12.png  "ghd")

## Setup / Commitovanie z Jetbrains Rider <a id = commit_rider>

### Setup Repozitára

Po inštalacií Jetbrains Rider si musíš synchronizovať GitHub repozitár, aby si z neho mohol commitovať.

1. Po otvorení Jetbrains Rider zvoľ možnosť **Get from VCS**.

![imgrd1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/1.png  "rider")

2. Po otvorení nového okna skontroluješ, či Rider rozoznáva Git v systéme. Pokiaľ sa Ti zobrazuje možnosť **Git is not intalled**, klikni na **Download and install** a počkaj kým sa proces skončí (môže to trvať pár minút).

![imgrd2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/2.png  "rider")

3. Naľavo v menu klikni na **GitHub** a potom na možnosť **Log in via Github...**, čo Ti otvorí internetový prehliadač. Klikni na tlačidlo **Authorise in Github**, prihlás sa a po úspešnom prihlásení sa Ti zobrazí, že si sa úspešne prihlásil do Githubu a že môžeš zavrieť kartu.

![imgrd3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/3.png  "rider")

![imgrd4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/4.png  "rider")

![imgrd5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/5.png  "rider")

![imgrd6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/6.png "rider")

4. Po úspešnom prihlásení Ti Rider ponúkne Tvoje repozitáre na stiahnutie:

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/7.png "rider")

5. Klikni na tlačidlo **Clone** - Repozitár sa Ti automaticky stiahne a môžeš ho používať.

### Commitovanie

Po úprave súborov je potrebné vykonať **commit**.

  

1. V pravom hornom rohu vidíš ikony ponuky **GIT**. Na commitovanie klikni na zelenú fajku.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/11.png "rider")

  

2. Otovrí sa Ti ponuka naľavo, ktorá ukazuje zmenené súbory. Dole napíš popis commitu a klikni na **Commit and Push**.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/12.png "rider")

  

3. Tento krok je nutný iba po **prvom commite** z nového **IDE**: Git potrebuje Tvoje údaje pre prvé spustenie. Informácie zadáš a následne klikneš na **Set and commit**.

  

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/13.png "rider")

  

4. Zobrazí sa Ti okno, ktoré Ti zhrnie, aké zmeny ideš vykonať. Klikni na tlačidlo **Push** a Rider nahrá zmeny priamo na GitHub.

  

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/14.png "rider")

  

### Sťahovanie zmien z GitHubu / Fetch

Zmeny, ktoré boli vykonané v Repozitári niekým iným, sa Ti automaticky nestiahnú, musíš si ich najskôr **fetchnúť** a potom **pullnúť**.

1. V GIT paneli klikni na modrú šípku smerujúcu nadol.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/16.png "rider")

2. Po kliknutí zvoľ možnosť **Merge incomming changes into current branch**.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/17.png "rider")



## Setup / Commitovanie z terminálu <a id = commit_cmd>

### Setup
1. Stiahni **GIT** (návod na stiahnutie je k dispozícii na [ich stránkach](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
2. Nakonfiguruj svoje **meno** a **email**.
```
$ git config --global user.name "Tvoj Github Login"
$ git config --global user.email "tvoj_email@nieco.nieco"
```
3. **Inicializuj** GitHub repozitár.
```
$ git init
```
4. **Napáruj** si repozitár na terminál.
```
$ git remote add origin "https://github.com/github_login/meno_repozitara.git"
```
4. Nastav si **vetvu**, v ktorej chceš pracovať (spravidla `main`).
```
$ git branch -M main
```
### Commitovanie
1. Vyber všetky **zmeny**, ktoré chceš **nahrať**.
```
$ git add <zmenený_súbor>
```
Ak chceš nahrať **všetky súbory**, tak treba zadať:
```
$ git add .
```
2. **Commitni** zmeny s vhodným **popisom** zmien.
```
$ git commit -m "toto je popis commitu"
```
3. **Nahraj** commitnuté zmeny na GitHub.
```
$ git push
```
### Sťahovanie zmien z GitHubu / Fetch
1. Pokiaľ chceš iba v terminále **aktualizovať povedomie** o **aktuálnej verzii** na GitHube.
```
$ git fetch
```
2. Pokiaľ chceš nie len zistiť, aké zmeny boli prevedené, ale chceš ich aj **stiahnuť**.
```
$ git pull
```

## Kolaborácia medzi spolužiakmi <a id = kolaboracia>

  

Si v tíme so spolužiakom a máte spoločne robiť na projekte, no nechceš, aby ste mali každý svoj repozitár, chcete pracovať na jednom. V takom prípade môžeš spolužiaka pridať ako spolupracovníka do svojho repozitára.

1. Pôjdeš do **nastavení repozitára**.

![img3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep1.png "settings")

2. Klikneš na **Manage Access** (Môže vyžadovať opätovné prihlásenie).

![img4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep2.png "settings")

3. Klikneš na **Invite a collaborator**.

![img5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep4.png "settings")

  

4. Vyhľadáš spolužiaka a pridáš ho.

![img6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep5.png "settings")

![img7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep6.png "settings")

![img8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep7.png "settings")

![img9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep8.png "settings")

5. Spolužiakovi potom príde na e-mailovú adresu pozvánka, ktorú príjme.

![img10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo8.png "settings")

![img11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo9.png "settings")

  

## GitHub Student Developer Pack <a id = student_pack>

  

Github poskytuje pre študentov sadu nástrojov a výhod **zadarmo**. Príkladom je **Jetbrains IDE** alebo **Github Copilot**. Naša škola je registrovaná GitHubom a preto ako študent máš možnosť dané výhody využívať.

Na balíček potrebujete:

1. **GitHub** Účet

2. Potvrdenie o návšteve školy z **EduPage** alebo **ISIC**

3. **Školskú** e-mailovú adresu (@spsknm.onmicrosoft.com)

  

Začni tým, že si pridáš v nastaveniach školskú emailovú adresu ako **sekundárnu**:

  

![img12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/email1.png "settings")

  

Následne choď na stránku https://education.github.com , kde sa prihlás a požiadaj o **discount**. Zvoľ **školskú* e-mailovú adresu a napíš, že akým spôsobom plánuješ využívať **GitHub Student Pack**:

  

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/imgGEdu.png "settings")

  

Potom klikni na **continue** a nahraj svoj naskenovaný **ISIC** / snímku obrazovky z **EduPage**:

  

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/eduimg3.png "settings")

  
  

Do **Proof type** daj:

  

* pokiaľ si poslal **ISIC** - **Dated School ID**.

  

* pokiaľ si poslal snímku obrazovky z **EduPage** - **Other (Example: Screenshot of school portal)**.

  

A žiadosť odošli. GitHub by sa mal ozvať do **30 dní**.


*Pozn.: Školsku e-mailovú adresu (@spsknm.onmicrosoft.com) si treba pýtať od svojho učiteľa programovania*

*Pozn.: Odporúčame, aby si si prečítal(a) oficiálnu dokumentáciu GitHub Education: https://docs.github.com/en/education. Takisto odporúčame aby si si prečítal(a) FAQ Github Education v prípade že nemáš ISIC: https://github.blog/2019-07-30-how-to-get-the-github-student-developer-pack-without-a-student-id/*
  
*Pozn.: Github často mení tieto požiadávky, čiže táto časť môže byť out-of-date. V prípade, že je, uvítame pull-requesty s opraveným postupom.*

## Zdroje <a id = zdroje>

  

GitHub Docs - https://github.com/github/docs/ pod licenciou <a href="https://github.com/github/docs/blob/main/LICENSE">CC-BY 4.0</a>
