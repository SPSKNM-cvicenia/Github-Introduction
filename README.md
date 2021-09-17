# Vitaj na GitHube!

Asi si sa ešte s GitHubom nestretol(nestretla), to však nevadí. V tejto príručke Ti vysvetlíme, ako funguje **Git**, zameriame sa aj na dôležité pojmy ako **Commit** alebo **Pull Request**.

## Navigácia
* [Základné pojmy](#zakladne_pojmy)
* [Založenie repozitára](#zalozenie_repozitara)
* [Setup / Commitovanie z Visual Studia](#commit_vs)
* [Setup / Commitovanie z Jetbrains Rider](#commit_rider)
* [Kolaborácia medzi spolužiakmi](#kolaboracia)
* [GitHub Student Developer Pack](#student_pack)
* [Zdroje](#zdroje)

## Základné pojmy <a id= zakladne_pojmy>

**Git** - Git je open source nástroj, ktorý Ti umožní **sledovanie zmien** v súboroch. Je základnou technológiou, ktorú GitHub využíva.

**Repository** (**Repozitár**, skrátene **Repo**) - Repozitár je základným prvkom GitHubu. Dá sa povedať, že to je **priečinok**, v ktorom máš umiestnený svoj projekt. Tento priečinok obsahuje všetky súbory Tvojho projektu a ukladá **históriu všetkých zmien** každého súboru. Nemusíš byť jediným, kto má k repozitáru prístup, pretože repozitár môže mať viacerých spolupracovníkov. Repozitár môže byť **verejný** alebo **súkromný**.

**Commit** - Commit je **konkrétna zmena** v projekte. Keď commituješ, Git vytvára **jedinečné ID**, ktoré Ti umožní uchovávať záznamy o týchto zmenách a aj to, **kto** a **kedy** danú zmenu vykonal.

**Organizácia** (**Organisation**) - GitHub Organizácia je ako profil, ku ktorému majú prístup **viacerí** užívatelia. V tejto organizácií si môžeš vytvárať repozitáre.

**Fork** - Fork je kópia repozirára iného používateľa, ktorá sa uloží medzi Tvoje repozitáre. Forky Ti umožnia voľne vykonávať zmeny v projekte **bez ovplyvnenia pôvodného repozitára**. Môžeš však otvoriť **Pull Request** v pôvodnom repozitári.

**Pull Request** - Pull Requesty sú zmeny v repozitári, ktoré navrhol používateľ a ktoré môžeš ako **vlastník** (alebo **spolupracovník**) pôvodného repozirára **prijať**, prípadne **odmietnuť**. 

**Push** - Pushnúť znamená, že zmeny, ktoré sa nachádzajú v **commitoch** a ešte neboli pushnuté, sa objavia v **repozitári**.

**Pull** - Pullnuť znamená, že ak nemáš aktuálnu verziu svojho repozitára, tak sa ti z GitHubu stiahne **aktuálna verzia**, v prípade, že si nejaké súbory upravil, tak môže nastať **konflikt**, ktorý je nutné vyriešiť.

**Branch** - Branch je **vetva projektu**, ktorú môžeš pridať, ak chceš opraviť chybu alebo s niečím experimentovať, ale nechceš, aby ti to ovplyvnilo Tvoj projekt. Každý repozitár má **default branch**, ale môže obsahovať aj ďaľšie.

**Merge** - Merge je **zlúčenie** jednej branche do druhej za vykonania **Pull Requestu**.

**Licencia** - Licencia je dôležitý súbor, ktorý Ti **povoľuje** alebo **zakazuje** využívať kódy iných užívateľov. Licencia môže obsahovať **podmienky** a kód pod touto licenciou môžeš legálne použiť iba vtedy, ak ich spĺňaš.

**IDE** - *Integrated development environment* - je **vývojové prostredie** v ktorom budeš pracovať.

**readme** - Je to textový súbor obsahujúci informácie o repozitári. Keďže sa automaticky zobrazuje **pod repozitárom**, je zvyčajne prvým súborom, ktorý návštevník Tvojho repozitára uvidí. Tvorí sa v **markdowne**.

**.gitignore** - gitignore je súbor, ktorý špecifikuje, ktoré časti by sa nemali nahrávať spolu so zmenami v commite. Používa sa na **vyfiltrovanie zbytočných súborov**, napríklad tých, ktoré vytvorí IDE.

*Pozn.: Toto sú len základné pojmy. Odporúčame, aby si si prečítal(a) slovník z oficiálnej dokumentácie GitHubu: https://docs.github.com/en/get-started/quickstart/github-glossary*

## Založenie Repozitára <a id = zalozenie_repozitara>

1. V pravom hornom rohu, rozklikni **+** a klikni na **New Repository**.

![img1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo1.png "Nové repo")

2. Pomenuj svoj repozirár, môžeš pridať aj popis, **readme** súbor, **.gitignore**, **licenciu** alebo zmeniť repozitár na **súkromný**. Následne klikni na **Create Repository**.

![img2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo2.png "Nové repo")

## Setup / Commitovanie z Visual Studia <a id = commit_vs>
### Setup repozitára
Po inštalacií Visual Studia si musíš synchronizovať GitHub repozitár, aby si z neho mohol vytvárať commity.
  
1. Po otvorení Visual Studia zvoľ možnosť **Clone a repository**, ktorá sa nachádza v pravej časti okna.
  
![imgvs1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/1.png "vs")
  
2. Tu zvoľ možnosť **Github**.
  
![imgvs2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/2.png "vs")
  
3. Vyskočí na teba okno, v ktorom sa môžeš v pravej hornej časti prihlásiť kliknutím na **Sign in...**.
  
![imgvs3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/3.png "vs")
![imgvs4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/4.png "vs")
  
4. Po úspešnom prihlásení Ti Visual Studio sprístupní tvoje repozitáre.
  
![imgvs5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/5.png "vs")
  
Po vybraní jedného z repozitárov sa Ti stiahne a môžeš ho upraviť alebo inak využívať.

### Commitovanie 
Po úprave súborov musíš commitnúť zmeny.
1. Po úprave projektu Ti Visual Studio vypíše, koľko zmien sa vykonalo. Klikneš na ceruzku v pravom dolnom rohu s číslom (číslo symbolizuje kolko súborov sa zmenilo), otvorí sa Ti **GIT panel**.

  ![imgvs6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/6.png "vs")
 
2. Vypíšeš popis commitu a zmáčneš **Commit All**.
  
  ![imgvs7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/7.png "vs")
  
  ![imgvs8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/8.png "vs")
  
3. Všimni si, že Visual Studio píše, že commit bol vytvorený lokálne - to znamená, že ešte nie je v tvojom repozitári na GitHube, ale len v Tvojom počítači. Ak ho chceš dať na GitHub, klikni na **Push**, a Visual Studio to pushne na GitHub.
  
  ![imgvs9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/9.png "vs")
  
  ![imgvs10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/10.png "vs")

### Sťahovanie zmien z Githubu / Fetchovanie
Zmeny, ktoré boli vykonané v Repozitári niekým iným, sa Ti automaticky nestiahnú, musíš si ich najskôr **fetchnúť** a potom **pullnúť**.

1. V Git paneli klikni na **Fetch**
 
  ![imgvs11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/11.png "vs")

2. Visual Studio Ti potom vypíše, že koľko commitov je potrebné stiahnuť, aby si mal najaktuálnejšiu verziu repozitára:

  ![imgvs12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/12.png "vs")
  
3. Klikneš na **počet zmien** a následne na **Pull**.

  ![imgvs13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/13.png "vs")
  
## Setup / Commitovanie z Jetbrains Rider <a id = commit_rider>
### Setup Repozitára
Po inštalacií Jetbrains Rider si musíš synchronizovať GitHub repozitár, aby si z neho mohol commitovať.
  
1. Po otvorení Jetbrains Rider zvoľ možnosť **Get from VCS**.
![imgrd1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/1.png "rider")
2. Po otvorení nového okna skontroluješ, či Rider rozoznáva Git v systéme. Pokiaľ sa Ti zobrazuje možnosť **Git is not intalled**, klikni na **Download and install** a počkaj kým sa proces skončí (môže to trvať pár minút).
![imgrd2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/2.png "rider")
3. Naľavo v menu klikni na **Github** a potom na možnosť **Log in via Github...**, čo Ti otvorí internetový prehliadač. Klikni na tlačidlo **Authorise in Github**, prihlás sa a po úspešnom prihlásení sa Ti zobrazí, že si sa úspešne prihlásil do Githubu a že môžeš zavrieť kartu.
![imgrd3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/3.png "rider")
![imgrd4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/4.png "rider")
![imgrd5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/5.png "rider")
![imgrd6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/6.png "rider")
4. Po úspešnom prihlásení Ti Rider ponúkne Tvoje repozitáre na stiahnutie:
![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/7.png "rider")
5. Klikni na tlačidlo **Clone** - Repozitár sa Ti automaticky stiahne a môžeš ho používať.
### Commitovanie 
Po úprave súborov je potrebné vykonať **commit**.

1. V pravom hornom rohu vidíš ikony ponuky **GIT**. Na commitovanie klikni na zelenú fajku.
   
![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/11.png "rider")

2. Otovrí sa Ti ponuka naľavo, ktorá ukazuje zmenené súbory. Dole napíš popis commitu a klikni na **Commit and Push**
 
![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/12.png "rider")

3. Tento krok je nutný iba po **prvom commite** z nového **IDE**: Git potrebuje Tvoje údaje pre prvé spustenie. Informácie zadáš a následne klikneš na **Set and commit**. 

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/13.png "rider")

4. Zobrazí sa Ti okno, ktoré Ti zhrnie, aké zmeny ideš vykonať. Klikni na tlačidlo **Push** a Rider nahrá zmeny priamo na GitHub.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/14.png "rider")

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/14.png "rider")
 
### Sťahovanie zmien z Githubu / Fetchovanie
Zmeny, ktoré boli vykonané v Repozitári niekým iným, sa Ti automaticky nestiahnú, musíš si ich najskôr **fetchnúť** a potom **pullnúť**.
  
1. V GIT paneli klikni na modrú šípku smerujúcu nadol
  
![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/16.png "rider")
  
2. Po kliknutí zvoľ možnosť **Merge incomming changes into current branch**.
  
![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/17.png "rider")

  
## Kolaborácia medzi spolužiakmi <a id = kolaboracia>

Si v tíme so spolužiakom a máte spoločne robiť na projekte, no nechceš, aby ste mali každý svoj repozitár, chcete pracovať na jednom. V takom prípade môžeš spolužiaka pridať ako spolupracovníka do svojho repozitára.
1. Pôjdeš do **nastavení repozitára**.
![img3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep1.png "settings")
2. Klikneš na **Manage Access** (Môže vyžadovať opätovné prihlásenie).
![img4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep2.png "settings")
3. Klikneš na **Invite a collaborator**.
![img5](
https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep4.png "settings")

4. Vyhľadáš spolužiaka a pridáš ho.
![img6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep5.png "settings")
![img7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep6.png "settings")
![img8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep7.png "settings")
![img9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep8.png "settings")
5. Spolužiakovi potom príde na e-mailovú adresu pozvánka, ktorú príjme.
![img10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo8.png "settings")
![img11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo9.png "settings")

## GitHub Student Developer Pack <a id = student_pack>

Github poskytuje pre študentov sadu nástrojov a výhod **zadarmo**. Príkladom je **Jetbrains IDE** alebo **Github Pro**. Naša škola je registrovaná GitHubom a preto je možné dané výhody využívať.
Na balíček potrebujete: 
1. **GitHub** Účet
2. Potvrdenie o návšteve školy z **EduPage** alebo **ISIC**
3. **Školskú** e-mailovú adresu

Začni tým, že si pridáš v nastaveniach školskú emailovú adresu ako **sekundárnu**:

![img12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/email1.png "settings")

Následne choď na stránku https://education.github.com , kde sa prihlás a požiadaj o **discount**. Zvoľ **školskú* e-mailovú adresu a napíš, že akým spôsobom plánuješ využívať **GitHub Student Pack**:

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/imgGEdu.png "settings")

Potom klikni na **continue** a nahraj svoj naskenovaný **ISIC** / snímku obrazovky z **EduPage**:

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/eduimg3.png "settings")


Do **Proof type** daj:

Pokiaľ si poslal **ISIC** - **Dated School ID**

Pokiaľ si poslal snímku obrazovky z **EduPage** - **Other (Example: Screenshot of school portal)**

A žiadosť odošli. GitHub by sa mal ozvať do **30 dní**

*Pozn.: Odporúčame, aby si si prečítal(a) oficiálnu dokumentáciu GitHub Education: https://docs.github.com/en/education. Takisto odporúčame aby si si prečítal(a) FAQ Github Education v prípade že nemáš ISIC: https://github.blog/2019-07-30-how-to-get-the-github-student-developer-pack-without-a-student-id/*
  
## Zdroje <a id = zdroje>

GitHub Docs - https://github.com/github/docs/ pod licenciou <a href="https://github.com/github/docs/blob/main/LICENSE">CC-BY 4.0</a>


