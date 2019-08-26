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

@snap[north-west span-20]
@fa[code-branch]
@snapend

@snap[north span-40]
Pazīstamas darbības
@snapend

@snap[north-east span-40]
Līdzīgas **git** darbības
@snapend

@snap[west span-20]
**Darbības**
@snapend

@snap[midpoint span-40]
save

load / open
@snapend

@snap[east span-40]
commit / push

pull / checkout
@snapend

@snap[south-west span-20]
**Jēga**
@snapend

@snap[south span-40 text-06]
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
- Statiska mājas lapa GitHub par brīvu

@ulend

+++

### Kāpēc to vajag skolā?

@ul

- Viegli dalīties ar programmēšanas piemēriem un uzdevumiem
- Viegla mājasdarbu vai projektu darbu nodošana
- Var vai nu klonēt ar git vai lejupielādēt kā *.zip
- Grūti taisnoties, ka darbu "suns apēda" vai "dators pazaudēja"
- Redzams izmaiņu laiks - redzams kad un ko skolēns ir darījis

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

# Kā to lieto?

+++

Shematisks workflow

+++

@snap[west span-40]
@img[](assets/img/vscode-side-icons.png)
@snapend

@snap[north span-50]
@css[text-green fragment](Datņu saraksta skats)
@snapend

@snap[midpoint span-50]
@css[text-pink fragment](Versiju kontroles skats)
@snapend

+++

## Lejupielādē (klonē) repozitoriju lokāli

 ```
 git clone https://github.com/vards/repo-nosaukums.git
 ```

 piemēram

 ```
 git clone https://github.com/startitfonds/startit-git-materiali.git
 ```

+++

## Repozitorija statuss

```
git status
```

+++

## Lejupielādē izmaiņas

```
git pull
```

+++

## Izveido jaunu zaru

Darbojas kā virtuāla kopija visai repozitorijas struktūrai un datiem.

Zarus nosaukumus parasti veido pēc kāda iepriekš norunāta principa

```
git branch -b zara-nosaukums
```

Piemēram:

```
git branch -b gd--b123-labojums
```

+++

## Reģistrē mainītu datni saglabāšanai

- Izmaiņu pievienošana nenotiek automātiski.
- Saglabāta datne ar git status komandu parādīsies kā mainīta (salīdzinot ar to, kas bija repozitorijā). 
- Izmainīto datni vai datnes jāpievieno ar **+** vai git add komandu

```
git add . // Pievieno visas izmainītās datnes
git add important.h // Pievieno tikai konkrētu datni
```

+++

## Saglabā reģistrētās datnes jaunā versijā

```
git commit -m "Izmaiņas aprakstošs komentārs"
```

+++

## Publicē visas versijas (kommitus) tiešsaistes repo

```
git push
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
