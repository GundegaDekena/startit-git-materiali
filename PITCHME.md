## Versiju kontroles sistēmas

---?color=linear-gradient(90deg, white 50%, black 50%)

@snap[west span-30 text-center]

## git

### GitHub

@fa[github fa-3x]
@snapend

@snap[north-east span-60 text-12]
@box[bg-green text-white box-padding](**Kas** tas ir?)
@snapend

@snap[east span-60 text-12]
@box[bg-blue text-white box-padding](**Kāpēc** to vajag?)
@snapend

@snap[south-east span-60 text-12]
@box[bg-gold text-white box-padding](**Kā** to lieto?)
@snapend

---

## Kas tas ir?

+++

## Versiju kontrole

@ul

- Specializēts rīks, ko lieto programmatūras izstrādei
- Līdzīgi save/load un undo/redo
- Vienkārša dažādu versiju apvienošana vienai vai daudzām datnēm
- **Daudz** jaudīgākas iespējas
- Rezerves kopijas mākonī un pie citiem izstrādātājiem

@ulend

+++

@snap[north-west span-50]
Pazīstamas darbības
@snapend

@snap[north-east span-40]
Līdzīgas **git** darbības
@snapend

@snap[west span-40]
save

load / open
@snapend

@snap[east span-40]
commit / push

pull / checkout
@snapend

@snap[south-west span-40 text-06]
saglabāt izmaiņas datnē

atvērt esošu datni
@snapend

@snap[south-east span-40 text-06]
saglabāt jaunu versiju vienai vai vairākām datnēm

atjaunot jaunāko vai iepriekšējo versiju vienai vai vairākām datnēm
@snapend

---

## Kāpēc to vajag?

+++

### Kāpēc to vajag vispār?

@ul

- Izstrādes procesa pārskats un attīstība @note[Var redzēt kad kas mainījies]
- Atvieglo sadarbību @note[Grupu darbs ir svarīgs, tā tiek veidoti reāli projekti]
- Industrijas standarts
- Koda rezerves kopijas @note[Ja lieto kādu centralizētu repozitoriju]

@ulend

+++

### Kāpēc to vajag skolā?

@ul

- Viegli dalīties ar programmēšanas piemēriem un uzdevumiem
- Viegla mājasdarbu vai projektu darbu nodošana
- Var vai nu klonēt ar git vai lejupielādēt kā *.zip
- Grūti taisnoties, ka darbu "suns apēda" vai "dators pazaudēja"
- Redzams izmaiņu laiks - redzams kad un ko skolēns ir darījis
- Statiska mājas lapa GitHub par brīvu

@ulend

+++

### Kāpēc to vajadzēs pēc skolas?

@ul

- Versiju kontroles sistēmas lieto visur
- Citām VCS ir līdzīgi pamatprincipi kā git
- git ir pašlaik visizplatītākā VCS
- GitHub ir populārākā tiešsaistes git platforma
- Daudzi darba devēji ņem vērā potenciālo darbinieku GitHub profilus un aktivitāti

@ulend

---

## Kā to lieto?

+++

### Termini

@ul

- Repozitorijs (repository), repo - koda organizācijas vienība, mape
- Versija (version) - paralēli saglabātas un pieejamas datnes/-ņu satura izmaiņas
- Kommits (commit) - izmaiņu versijas saglabāšana (process), pati versija
- Zars (branch) - paralēla izmaiņu versija repozitorijā

@ulend

+++

Esoša repozitorija pievienošana (fork) savam GitHub kontam

@img[](assets/img/github-fork.png)

+++

Repozitorija klonēšana ar GitHub Desktop

@img[](assets/img/gh-desktop-clone.png)

+++

Repo mapes atvēršana VSCode

@img[](assets/img/gh-desktop-open-vsc.png)

+++

### Ja VSCode rāda git error 

@img[](assets/img/vscode-git-error.png)

+++

- iekš VSCode - atver Command Palette (Ctrl+Shift+P)
- atrod un atver "settings.json" datni
- izveido ierakstu, kur iestatīt "git.exe" atrašanās vietu

+++

- atrod un atver mapi, kur tika ieinstalēts "Git for Windows" vai GitHubDesktop
- atrod "git.exe" atrašanās vietu
- saglabā "settings.json" datni

Ierakstam jāizskatās tā:

```
{
    "git.path": "C:/ "
}
```

+++

### Aizver un atkal atver VSCode

@img[](assets/img/vscode-git-view.png)

@img[](assets/img/vscode-git-view-light.png)

+++

### VSCode integrācija

@img[](assets/img/vscode-side-icons.png)

+++

### Darba plūsma

@img[](assets/img/git-workflow-simple.png)

+++

### Lejupielādē (klonē) repozitoriju lokāli

 @img[](assets/img/github-repo-menu.png)
 
 @img[](assets/img/gh-desktop-clone.png)
 
 ```
 git clone https://github.com/vards/repo-nosaukums.git
 ```

+++

### Izveido jaunu zaru

Darbojas kā virtuāla kopija visai repozitorijas struktūrai un datiem.

@img[](assets/img/gh-desktop-branching.png)

```
git branch -b gd--b123-labojums
```

+++

### Reģistrē mainītu datni saglabāšanai

- Izmaiņu pievienošana repo nenotiek automātiski.
- Mainīta datne būs iezīmēta (**M**). 
- Izmainīto datni vai datnes jāpievieno "staging" sarakstam.
- Kad pievienotas visas datnes, veic "commit"

+++

### Saglabā reģistrētās datnes jaunā versijā

@img[](assets/img/vscode-git-commit.png)

```
git add .
git commit -m "Izmaiņas aprakstošs komentārs"
```

+++

### Publicē visas versijas (kommitus) tiešsaistes repo

@img[](assets/img/gh-desktop-push.png)

```
git push
```

+++

### Publicē visas versijas (kommitus) tiešsaistes repo

@img[](assets/img/gh-desktop-pull-changes.png)

```
git pull
```

---

## GitHub

### git repozitoriju tiešsaistes krātuve

+++

### Jauna repozitorija izveidošana

+++

### Repozitorija dublēšana sev - "fork"

+++

### Lietotāju pievienošana un tiesības

- Lietotāja pievienošana
- Lietotāja tiesības

+++

### Izmaiņu pievienošanas pieprasījums

- Issuing a pull request
- Accepting a pull request
