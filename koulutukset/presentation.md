layout: true
name: sininen-palkki
class: sininen-palkki
![logo](suomifi_logo.svg)

---
layout: true
name: header
class: center, middle, sininen
![logo](suomifi_logo.svg)

---
layout: true
name: valkoinen
class: valkoinen
![logo](suomifi_logo.svg)

<!--DON'T TOUCH ABOVE THIS !!!!!! -->

---
template: header
# Tämä on aloitus dia, sen sisältö on keskitetty

---
class: sininen-palkki
# Dian vaihto Remarkjs:ssä

Kirjoittamalla markdown tiedostoon '---' aloitetaan uusi dia.

Kirjoittamalla tiedostoon '???' aloitetaan dian komentti osia. Komentti osia ei ole pakollinen

Tässä diass on käytetty `class: kanerva`, joka muuttaa tekstin värin mustaksi ja taustan palveluväylän väriseksi. Kaikkien diojen pitää alkaa luokalla. Vaihtoehdot on: sininen, valkoinen tai kanerva

---
template: sininen-palkki

# Dian attribuutit

* Dialle voi antaa nimen, kirjoittamalla dian alkuun 'name:' ja dian nimi
* Dialle voi antaa luokkia kirjoittamalla dian alkuun 'class:' ja luokan nimi.
* Dialle voi antaa tausta kuvan kirjoittamalla dian alkuun 'background-image'
* Layout ja templateista: [Remarkjs:n documentaatiossa](https://github.com/gnab/remark/wiki/Markdown#template)

---
template: sininen-palkki

# Rivin vaihto markdown:ssa

Markdown syntaxin kirjoittaminen on helppoa. Jos haluat jakaa tekstin useamalle riville, lisää rivin loppuun
```html
  <br>
```
Jolloin rivin vaihto tapahtuu ilman tyhjää tilaa. Mutta yleensä tälle ei ole juuri käyttöä koska Remark osaa jäsennellä rivit dian levyiseksi automaattisesti.

Myös rivin vaihto tapahtuu jättämällä Markdown tiedostoon yhden ylimääräisen tyhjän välin.

---
template: sininen-palkki

# Otsikot

Otsikko Markdown:ssa tehdään käytttämällä merkkiä #.

Merkkien lukumäärä kertoo otsikon tason, mitä enemmän sitä pienempi (syvemmällä).

## 2. Tason otsikko ##

### 3. Tason otsikko ###

#### 4. Tason otsikko ####

##### 5. Tason otsikko #####

##### 6. Tason otsikko #######

---
template: sininen-palkki

# Listat

Listoja tehdään aloittamalla rivi joko * tai - :
* Listaelementti
  * Sisennetty listaelementti

tai
- Listaelementti
  - Sisennetty listaelementti

Listojen sisennys tapahtuu 2 välilyönnillä.

---
template: sininen-palkki

# Koko tekstin asettelu diassa

On mahdollista asetalla dian sisältöä hyödyntäen luokkia. Muutama valmis luokka:
Vertikaalinen asettelu:
```markdown
top (default)
middle
bottom
```

Horisontaalinen asettelu:
```markdown
left (default)
center
right
```

Myös on mahdollista asetella vain teksti palaa:
```markdown
.left[Left-aligned text]
.center[Centered text]
.right[Right-aligned text]
```

---
template: sininen-palkki

# Kuvan tai linkin lisääminen

Remarkissa on mahdollista asettaa linkki tai kuva diaan:
```markdown
![Kuvan-alias](/path/to/image tai url.to.image)

<img alt="nimi" src="osoite" height="korkeus" width="leveys" />

[Linkin nimi](url.to.link)

<a href="osoite">Nimi</a>
```
Mikäli haluaa kuvalle tai linkille omia CSS sääntöjä:
```markdown
.right[![Right-aligned image](imageUrl)]
```
Koodi blockin lisääminen markdownissa tapahtuu kirjoittamalla koodi

&#96;&#96;&#96;javascript <br/>
function sum(a, b) { <br/>
  return a + b; <br />
} <br/>
&#96;&#96;&#96;
