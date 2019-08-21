## Versiju kontroles sistēmas
### Git

---

@snap[west span-30]
@box[bg-gold text-white rounded box-padding](Kas tas ir?)
@snapend

@snap[midpoint span-30]
@box[bg-gold text-white rounded box-padding](Kāpēc to vajag?)
@snapend

@snap[east span-30]
@box[bg-gold text-white rounded box-padding](Kā to lieto?)
@snapend

---

# Kas tas ir?

+++

## Versiju kontrole

@ul

- Līdzīgi save/load - saglabāt un atvērt datnes
- Līdzīgi undo/redo - atgūt iepriekšējo versiju
- Daudz jaudīgākas iespējas
- Vienkārša dažādu versiju apvienošana
- Rezerves kopijas mākonī un pie citiem izstrādātājiem

@ulend

---

# Kāpēc to vajag?

+++

## Izstrādes procesa kontrole

+++

## Koda rezerves kopijas

+++

## Efektīva sadarbība

+++

## Industrijas standarts

+++

## Vienkārša mājas lapa GitHub

- https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages

+++

## Lietošana skolā

+++

### Mājasdarbu vai projektu darbu nodošana

- Var vai nu klonēt repozitoriju vai lejupielādēt kā *.zip
- Grūti taisnoties, ka darbu "suns apēda" vai "dators pazaudēja"
- Redzams izmaiņu laiks

+++

### Var viegli sekot skolēnu darba procesam

Redzams kad un ko skolēns ir darījis

+++

### Darbs grupās

- Viegli darboties pie viena uzdevuma/projekta
- Redzams cik daudz un bieži katrs ir darbojies

+++

### Sagatavo reālai darba videi

- Versiju kontroles sistēmas lieto visur, tām ir līdzīgi pamatprincipi
- Git ir pašlaik visizplatītākā VCS
- GitHub ir populārākā tiešsaistes platforma, citām ir līdzīga funkcionalitāte (GitLab, BitBucket)

---

# Kā to lieto?

+++

TODO shematisks workflow

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

## git clone

Lejupielādē (klonē) repozitoriju lokāli

 ```
 git clone https://github.com/<vards>/<repo-nosaukums>.git
 ```

 piemēram

 ```
 git clone https://github.com/GundegaDekena/startit-git-materiali.git
 ```

+++

## git pull

Esot git repozitorija datnē, pārbauda izmaiņu esamību un lejupielādē izmaiņas

```
git pull
```

+++

## git status

Esot git repozitorija datnē, parāda repozitorija statusu

```
git status
```

+++

## git branch

Izveido jaunu zaru ar definētu nosaukumu. Darbojas kā virtuāla kopija visai repozitorijas struktūrai un datiem. Zarus nosaukumus parasti veido pēc kāda iepriekš norunāta principa

```
git branch -b <zara-nosaukums>
```

Piemēram:

```
git branch -b gd--b123-labojums
```

+++

## git add

Izmaiņu pievienošana nenotiek automātiski. Saglabāts fails ar git status komandu parādīsies kā mainīts (salīdzinot ar to, kas bija repozitorijā). Izmainīto failu vai failus jāpievieno ar git add:

Pievieno visus izmainītos failus:

```
git add .
```

Pievieno tikai konkrētu datni:

```
git add important.h
```

+++

## git commit


+++

## git push

+++

## git merge

---

## GitHub

### Git repozitoriju tiešsaistes krātuve

---
