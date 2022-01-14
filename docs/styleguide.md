---
title: Guida al design
copyright:
  noCopy: true
  noSelect: true
colors:
  primary:
   hex: 0075BF
   name: Strong blue
  secondary:
   hex: 00A8E8
   name: Pure (or mostly pure) blue
  accent:
   hex:  DD0C10
   name: Vivid red
  dark:
   hex:  2B2727
   name: Very dark red
  light:
   hex:  F7F7F7
   name: Very light gray
colorsystem:
  info:
    hex:  D90CDD
    name: Information
  success:
   hex:  0CDD71
   name: Success
  warning:
   hex:  FFE40D
   name: Warning
  error:
   hex:  DD710C
   name: Danger

---

## Colori


<section class="container-lg clearfix">
<h3 class="my-2 color-fg-muted">Colori Principali</h3>
<p class="col-6 text-small text-center color-fg-subtle border-top border-x ">Brand Colors</p>
  <div class="col-2 float-left text-center mb-3 ">
  <img class="primary border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">Primario</h4>
    <p class="f6 m-auto ">{{ $frontmatter.colors.primary.name }}</p>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colors.primary.hex }}</p>
  </div>
    <div class="col-2 float-left text-center mb-3">
  <img class="secondary border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">Secondario</h4>
    <p class="f6 m-auto">{{ $frontmatter.colors.secondary.name }}</p>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colors.secondary.hex }}</p>
  </div>
      <div class="col-2 float-left text-center mb-3">
  <img class="accent border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">Accento</h4>
    <p class="f6 m-auto">{{ $frontmatter.colors.accent.name }}</p>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colors.accent.hex }}</p>
  </div>



<div class="col-2 float-left text-center mb-3 ">
  <img class="dark border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">Nero</h4>
    <p class="f6 m-auto">{{ $frontmatter.colors.dark.name }}</p>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colors.dark.hex }}</p>
  </div>

  <div class="col-2 float-left text-center mb-3">
  <img class="light border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">Bianco</h4>
    <p class="f6 m-auto">{{ $frontmatter.colors.light.name }}</p>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colors.light.hex }}</p>
  </div>
</section>

<section class="container-lg clearfix">
<h3 class="my-2 color-fg-muted">Colori di Sistema</h3>
  <div class="col-2 float-left text-center mb-3">
  <img class="info border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">{{ $frontmatter.colorsystem.info.name }}</h4>
  <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colorsystem.info.hex }}</p>
  </div>
    <div class="col-2 float-left text-center mb-3">
  <img class="success border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">{{ $frontmatter.colorsystem.success.name }}</h4>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colorsystem.success.hex }}</p>
  </div>
  <div class="col-2 float-left text-center mb-3">
<img class="warn border rounded-3 color-border-subtle"  width="100" height="100" />
    <h4 class="f5 m-auto">{{ $frontmatter.colorsystem.warning.name }}</h4>
   <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colorsystem.warning.hex }}</p>
  </div>
        <div class="col-2 float-left text-center mb-3">
  <img class="error border rounded-3 color-border-subtle"  width="100" height="100" />
  <h4 class="f5 m-auto">{{ $frontmatter.colorsystem.error.name }}</h4>
    <p class="f6 m-auto color-fg-subtle">#{{ $frontmatter.colorsystem.error.hex }}</p>
  </div>
</section>


### Primario

<li class="d-inline-block colorbox primary col-12 p-2 my-4">
<p class="f6 text-mono text-center color-fg-on-emphasis">#{{ $frontmatter.colors.primary.hex }} - {{ $frontmatter.colors.primary.name }}</p>
</li>


#### Tabella di Conversione.

| Hex triplet  | 0075bf                       | #0075bf               |
| ------------ | ---------------------------- | --------------------- |
| RGB Decimal  | 0, 117, 191                  | rgb(0,117,191)        |
| RGB Percent  | 0, 45.9, 74.9                | rgb(0%,45.9%,74.9%)   |
| CMYK         | 100, 39, 0, 25               |                       |
| HSL          | 203.2°, 100, 37.5            | hsl(203.2,100%,37.5%) |
| HSV (or HSB) | 203.2°, 100, 74.9            |                       |
| Web Safe     | 0066cc                       | #0066cc               |
| IE-LAB       | 47.601, 0.563, -46.309       |
| XYZ          | 15.763, 16.483, 51.638       |
| xyY          | 0.188, 0.196, 16.483         |
| CIE-LCH      | 47.601, 46.313, 270.697      |
| CIE-LUV      | 47.601, -29.065, -70.159     |
| Hunter-Lab   | 40.599, -1.743, -46.992      |
| Binary       | 00000000, 01110101, 10111111 |



#### Simulazione Ipovisione.
<br/>

*Acromatopsia*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #5a5a5a;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.005% odella popolazione mondiale">acromatopsia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #485f6e;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.001% della popolazione mondiale">atipica</span>
  </div>
</div>


*Dicromatismo*
<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #5876bd;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il primo colore fondamentale, ossia il rosso">protanopia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #3979c3;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il secondo colore fondamentale, ossia il verde">deuteranopia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #00848c;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il terzo colore fondamentale, ossia il blu-giallo">tritanopia</span>
  </div>
</div>

*Tricromatismo*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #3875bd;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il rosso">protanomalia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #2477c1;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il verde">deuteranomalia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #007e9e;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il blu-giallo">tritanomalia</span>
  </div>
</div>

---

### Secondario

<li class="d-inline-block colorbox secondary col-12 p-2 my-4">
<p class="f6 text-mono text-center color-fg-on-emphasis">#{{ $frontmatter.colors.secondary.hex }} - {{ $frontmatter.colors.secondary.name }}</p>
</li>

#### Tabella di Conversione.

| Hex triplet  | 00a8e8                       | #00a8e8               |
| ------------ | ---------------------------- | --------------------- |
| RGB Decimal  | 0, 168, 232                  | rgb(0, 168, 232)      |
| RGB Percent  | 0, 65.9, 91                  | rgb(0%,65.9%,91%)     |
| CMYK         | 100, 28, 0, 9                |                       |
| HSL          | 196.6°, 100, 45.5            | hsl(196.6,100%,45.5%) |
| HSV (or HSB) | 196.6°, 100, 91              |                       |
| Web Safe     | 0099ff                       | #0099ff               |
| CIE-LAB      | 64.826, -13.476, -42.134     |
| XYZ          | 28.564, 33.829, 81.364       |
| xyY          | 0.199, 0.235, 33.829         |
| CIE-LCH      | 64.826, 44.237, 252.264      |
| CIE-LUV      | 64.826, -43.293, -65.774     |
| Hunter-Lab   | 58.162, -14.12, -42.227      |
| Binary       | 00000000, 10101000, 11101000 |


#### Simulazione Ipovisione.
<br/>

*Acromatopsia*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #7d7d7d;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.005% odella popolazione mondiale">acromatopsia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #648692;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.001% della popolazione mondiale">atipica</span>
  </div>
</div>


*Dicromatismo*
<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #8ca0e0;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il primo colore fondamentale, ossia il rosso">protanopia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #7aa1ed;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il secondo colore fondamentale, ossia il verde">deuteranopia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #00b2be;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il terzo colore fondamentale, ossia il blu-giallo">tritanopia</span>
  </div>
</div>

*Tricromatismo*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #59a3e3;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il rosso">protanomalia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #4ea4eb;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il verde">deuteranomalia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #00aecd;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il blu-giallo">tritanomalia</span>
  </div>
</div>

---

### Accento

<li class="d-inline-block colorbox accent col-12 p-2 my-4">
<p class="f6 text-mono text-center color-fg-on-emphasis">#{{ $frontmatter.colors.accent.hex }} - {{ $frontmatter.colors.accent.name }}</p>
</li>

#### Tabella di Conversione.

| Hex triplet  | dd0c10                       | #dd0c10                |
| ------------ | ---------------------------- | ---------------------- |
| RGB Decimal  | 221, 12, 16                  | rgb(221,12,16)         |
| RGB Percent  | 86.7, 4.7, 6.3               | rgb(86.7%,4.7%,6.3%)   |
| CMYK         | 0, 95, 93, 13                |                        |
| HSL          | 358.9°, 89.7, 45.7           | hsl(358.9,89.7%,45.7%) |
| HSV (or HSB) | 358.9°, 94.6, 86.7           |                        |
| Web Safe     | cc0000                       | #cc0000                |
| CIE-LAB      | 46.547, 71.004, 55.656       |
| XYZ          | 30.046, 15.677, 1.934        |
| xyY          | 0.63, 0.329, 15.677          |
| CIE-LCH      | 46.547, 90.218, 38.091       |
| CIE-LUV      | 46.547, 148.642, 31.644      |
| Hunter-Lab   | 39.594, 66.165, 24.819       |
| Binary       | 11011101, 00001100, 00010000 |


#### Simulazione Ipovisione.
<br/>

*Acromatopsia*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #4b4b4b;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.005% odella popolazione mondiale">acromatopsia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #683e3f;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="0.001% della popolazione mondiale">atipica</span>
  </div>
</div>


*Dicromatismo*
<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #83762e;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il primo colore fondamentale, ossia il rosso">protanopia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #937000;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il secondo colore fondamentale, ossia il verde">deuteranopia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #de1a0f;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="cecità per il terzo colore fondamentale, ossia il blu-giallo">tritanopia</span>
  </div>
</div>

*Tricromatismo*

<div class="container-lg clearfix mb-4">
  <div class="col-4 float-left border p-4" style="background-color: #a34f23;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il rosso">protanomalia</span>
  </div>
  <div class="col-4 float-left border p-4" style="background-color: #ae4b05;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il verde">deuteranomalia</span>
  </div>
<div class="col-4 float-left border p-4" style="background-color: #de150f;">
    <span class="f6 color-fg-on-emphasis tooltipped tooltipped-n" aria-label="qualora sia deficitaria la sensibilità per il blu-giallo">tritanomalia</span>
  </div>
</div>

### Tinte

<BlankSlate>
<h2>Contenuto Non Disponibile</h2>
<p>Not Specified</p>
</BlankSlate>

### Toni

<BlankSlate>
<h2>Contenuto Non Disponibile</h2>
<p>Not Specified</p>
</BlankSlate>

### Gradienti

<BlankSlate>
<h2>Contenuto Non Disponibile</h2>
<p>Not Specified</p>
</BlankSlate>

## Tipografia

The main reason for using "system" fonts is performance. Fonts are typically one of the largest/heaviest resources loaded on a website. If we can use a font already available on the user’s machine, we can completely eliminate the need to fetch this resource, making load times noticeably faster.
The beauty of system fonts is that it matches what the current OS uses, so it can be a comfortable look.

### Font Stack

| Font  | 	Device Targeted |
| ------ | ---------------- |
| -apple-system (San Francisco) |	iOS Safari, macOS Safari, macOS Firefox |
| BlinkMacSystemFont (San Francisco) | 	macOS Chrome |
| Segoe UI  | 	Windows |
| Roboto | 	Android, Chrome OS |
| Oxygen / Oxygen-Sans | 	KDE |
| Ubuntu  | 	Ubuntu |
| Cantarell | 	GNOME |
| Helvetica Neue |	macOS versions < 10.11 |
| sans-serif | 	Any |


### Font Style
<p class="f6 color-fg-default typostyle">Roboto</p>
<div class="Box mt-4 px-4">
<p id="fs" class="color-fg-muted" style="font-size:60px;">AaBbCc</p>
<span id="fs" class="f6 color-fg-muted">
ABCDEFGHIJKLMNOPQRSTUVWXYZ<br>
abcdefghijklmnopqrstuvwxyz<br>
0123456789<br>
~%!@#$%^&*-_=+<br>
 []{}()|\/<>‘’”,.;:?</span></p>
</div>

 ### Font Weights

<ul class="Box mt-4">
<li id="fs" class="color-fg-muted Box-row"  style="font-weight:100;">Roboto Regular 100</li>
<li id="fs" class="color-fg-muted Box-row" style="font-weight:200;">Roboto Regular 200</li>
<li id="fs" class="color-fg-muted Box-row"  style="font-weight:300;">Roboto Regular 300</li>
<li id="fs" class="color-fg-muted Box-row" style="font-weight:400;">Roboto Regular 400</li>
<li id="fs" class="color-fg-muted Box-row" style="font-weight:500;">Roboto Regular 500</li>
<li id="fs" class="color-fg-muted Box-row" style="font-weight:600;">RobotoRegular 600</li>
</ul>


### Headings

<ul class="Box mt-4">
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:60px; font-weight:500;"><span class="f6 ws-normal color-fg-default typostyle mr-6 overflow-hidden flex-auto">HEADING 1</span>Roboto w500 60</p>
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:40px; font-weight:400;"><span class="f6 ws-normal color-fg-default typostyle  mr-6 overflow-hidden flex-auto">HEADING 2</span>Roboto w400 40</p>
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:32px; font-weight:300;"><span class="f6 ws-normal color-fg-default typostyle mr-6 overflow-hidden flex-auto">HEADING 3</span>Roboto w300 32</p>
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:28px; font-weight:300;"><span class="f6 ws-normal color-fg-default typostyle mr-6 overflow-hidden flex-auto">HEADING 4</span> Roboto w300 28</p>
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:26px; font-weight:300;"><span class="f6 ws-normal color-fg-default typostyle mr-6 overflow-hidden flex-auto">HEADING 5</span> Roboto w300 26</p>
<p id="fs" class="color-fg-muted Box-row d-flex flex-items-center" style="font-size:24px; font-weight:300;"><span class="f6 ws-normal color-fg-default typostyle mr-6 overflow-hidden flex-auto">HEADING 6</span> Roboto w300 24</p>
</ul>

### Corpo del Testo

<div class="Box mt-4 p-4">
<p id="fs" class="color-fg-muted" style="font-size:30px; line-height=50px;"> Lorem ipsum dolor sit amet, vel accumsan liberavisse ex, ea nec elaboraret interpretaris, sed diceret concludaturque no...</p>
<p class="Box-row text-small text-right">Paragraph Text | Roboto Regular - Weight 400 - 30px</p>
</div>

### Testo Aggiuntivo

<div class="Box mt-4 p-4">
<div class="d-flex flex-items-start">
<h4 id="fs" class="color-fg-muted mr-4 col-6" style="font-style:italic; color:#2B2727 !important;  font-size:22px; font-weight:200;">Some Title</h4>
<p id="fs" class="color-fg-muted ml-6 float-right col-12" style="font-size:24px; color:#2B2727 !important; font-weight:200;  line-height=50px;"> Lorem ipsum dolor sit amet, vel accumsan liberavisse ex, ea nec elaboraret interpretaris, sed diceret concludaturque no...</p>
</div>
<p class="Box-row text-small text-right">Additional Text | Roboto Regular Italic - Weight 200 - 24px</p>
</div>


## Accessibility Screenshots
Simulazione della visione dell'utente affetto da diverse patologie legate alla visione e alla percezione dei colori.

<!-- flex container -->
<section class="d-flex flex-justify-between flex-wrap mt-2">
<div class="p-1  my-1 tooltipped tooltipped-s tooltipped-multiline" aria-label="qualora sia deficitaria la sensibilità per il blu/giallo">
<p class="text-mono text-uppercase">tritanopia</p>
<img class="border color-border-accent-emphasis" alt="tritanopia" src="/images/accessibility_sim_tritanopia(noblue).png" width="320"  />
</div>
<div class="p-1  my-1 tooltipped tooltipped-s tooltipped-multiline" aria-label="qualora sia deficitaria la sensibilità per il rosso">
<p class="text-mono text-uppercase">protanopia</p>
<img class="border color-border-accent-emphasis" alt="protanopia" src="/images/accessibility_sim_protanopia(nored).png" width="320" />
</div>
<div class="p-1  my-1 tooltipped tooltipped-s tooltipped-multiline" aria-label="qualora sia deficitaria la sensibilità per il verde">
<p class="text-mono text-uppercase">deutoranopia</p>
<img class="border color-border-accent-emphasis" alt="deutoranopia" src="/images/accessibility_sim_deutoranopia(nogreen).png" width="320" />
</div>
<div class="p-1  my-1 tooltipped tooltipped-s tooltipped-multiline" aria-label="La bassa sensibilità al contrasto può essere sintomo di alcune patologie oculari come la cataratta, il glaucoma o la retinopatia diabetica.">
<p class="text-mono text-uppercase">contrastloss</p>
<img class="border color-border-accent-emphasis" alt="contrastloss" src="/images/accessibility_sim_contrastloss(nocontrast).png" width="320" />
</div>
<div class="p-1  my-1 tooltipped tooltipped-s tooltipped-multiline" aria-label="incapacità totale di percepire qualunque colore">
<p class="text-mono text-uppercase">achromatopsia</p>
<img class="border color-border-accent-emphasis" src="/images/accessibility_sim_achromatopsia_nocolor.png" width="300" />
</div>
</section>



<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

.primary {
background-color: #0075BF;
}

.secondary {
 background-color: #00A8E8;
}

.accent {
 background-color: #DD0C10;
}

.dark {
 background-color: #2B2727;
}

.light {
 background-color: #F7F7F7;
}

.info {
background-color: #D90CDD;
}

.success {
background-color: #0CDD71;
}

.warn {
background-color: #FFE40D;
}

.error {
background-color: #DD710C;
}

.colorblind {
width: 240px;
height: 48px;
}

#fs {
font-style: unset;
font-family:  Roboto, sans-serif;
}

.typostyle {
font-family: -apple-system,
            BlinkMacSystemFont,
            "Segoe UI",
            Roboto,
            Oxygen,
            Ubuntu,
            antarell,
            Open Sans
            "Helvetica Neue",
            sans-serif;
}


</Style>
