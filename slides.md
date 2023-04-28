---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss
---

# Amplificatori

Presentazione sugli amplificatori Hi-Fi

---
transition: fade-out
---

# Che cos'è un AMPLIFICATORE

Si parla di amplificatori quanto il guadagno di tensione o corrente  è **MAGGIORE** di **UNO**.

Gli amplificatori, in elettronica, sono dispositivi che sono in grado amplificare ovvero aumentare il segnale in ingresso. Il guadagno che crea può essere misurato con diverse unità di misura o addirittura **adimensionale**.<br><br>L'unità di misura più utilizzata e il decibel ***dB*** che è un sottomultiplo delle ***unità logaritmiche*** utilizzate per rappresentare scale estese in poco spazio. 

<center>
<img src="https://www.electroyou.it/fidocad/cache/9335c7a0cb14aa6fd0106ea89b586b61b6fe7ce1_3.png" alt="amplificatore">
</center>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: default
---

# Come si calcola l'amplificazione
Le formule per il calcolo dell'amplificazione sono uguali a quelle dell'attenuazione infatti derivano entrambi dal calcola delle guadagno. 

Amplificazione [*adimensionale*]:&emsp; $A = Uscita / Entrata$
<br><br><br>
Amplificazione [*dB*]:&emsp; $A[dB] = 10 * log10(A[adimensionale])$
<br><br>

Inoltre per i valori relativi alle fraquenze radio ***RF*** vengono usati i ***dBm*** o i ***dBW***.
<br><br>
Amplificazione [*dBm*]:&emsp; $A[dBm] = 10 * log10(P / 1mW)$
<br><br><br>
Amplificazione [*dBW*]:&emsp; $A[dBW] = 10 * log10(P / 1W)$
<br><br>
Dove 1mW e 1W sono i valori di riferimento.

---

# Tipi di amplificatori
Vari tipi di amplificatori.

Gli amplificatori si distinguono in più macro-settori:
- Digitale
- Analogico
- In continua
- In alternata

<div class="grid grid-cols-2 flex justify-center space-around space-x-10">
  <img src="https://www.cariatielettronica.eu/9489-large_default/amplificatore-audio-digitale-tpa3118-mono-1x60w-8-24v-dc.jpg" alt="ampli-digitale" style="width: 25%;">
  <img src="https://s.alicdn.com/@sc04/kf/H6326c56854094c189b411d0015137590O.jpg_280x280.jpg" alt="ampli-analogico" style="width: 25%;">
</div>


---
transition: slide-up

level: 2
---

# Amplificatore Digitale 
Un amplificatore digitale è un amplificatore che utilizza un **processore** per amplificare i segnali audio, nei circuiti digitali non ha importanza il valore preciso del segnale purché sia compreso entro certe soglie.

Il processore usato da questi tipi di amplificatori è chiamato DSP (**D**igital **S**ignal **P**rocessor) che permette di amplificare e di modificare il segnale inserendo degli effetti, per esempio cambiando la modulazione.

### Vantaggi
Il più ovvio è il fatto che non sono suscettibili alle interferenze di altre apparecchiature elettriche. Questo li rende ideali per l’uso con sistemi HiFi di fascia alta dove la chiarezza del suono è fondamentale.
### Svantaggi
Un amplificatore digitale è un’apparecchiatura molto complessa e come tale può essere più costosa da acquistare rispetto ad un amplificatore analogico ed hanno anche un consumo maggiore. 

<center>
  <img src="https://www.reviewbox.it/wp-content/uploads/2022/03/digital-amp-1024x683.jpg" alt="ampli-digitale" style="width: 20 %;">
</center>

---
layout: two-cols
---

# Amplificatore Analogico
Gli amplificatori analogici sono costituiti per la maggiorparte da componenti elettrici ma non da circuiti integrati. 

Nei circuiti analogici il segnale di uscita deve poter variare in modo continuo. La maggiorparte degli amplificatori analogici usano ***transistor*** o ***valvole***. 

Il transistor difatti sono un componente largamente usato in tutti campi, basti pensare che le CPU sono fatte di milioni di transistor.

Le valvole invece, sono usate molto poco e hanno campi di applicazione molto limitati per via delle dimensioni e del consumo di corrente elevato. Tuttavia nel caso degli amplificatori audio forniscono un suono generalmente più pulito amplificando in maniera costante tutte le frequenze, per questo si dice che "scaldano" il suono.

::right::

  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxjcFw0nixw9sqyhN9FchOnXMUhWUZbdep2AgjaCDXrNgFShnVC_iLT14pHBqC4pOhSLg&usqp=CAU" alt="ampli-transistor">

  <img src="https://images.squarespace-cdn.com/content/v1/5912db7ee6f2e1435dbab4fd/1514370957294-RHD01PBD5GQ6TVN7S52N/VALVECASTER+PCB+LESS+LAYOUT" alt="ampli-valvole" style="width: 90%">
---
layout: two-cols
---

# Amplificatore in corrente continua

<p></p>

Gli amplificatori in corrente continua hanno il compito di elevare il livello di piccole tensioni continue per poterle utilizzare in molte applicazioni, ad esempio, vengano molto usati per amplificare il valore di un sensore come sensori sismici, sensori elettromedicali...

Questi tipi di amplificatori riescono a "raddrizzare" la corrente alternata dei sensori perchè hanno una frequenza molto bassa e la trasformano in corrente continua.

  <img src="https://upload.wikimedia.org/wikipedia/commons/b/bc/Goper1dtcx.jpg" width="150" />
  Esempio di amplificatore 
  
::right::

  <img src="https://estore.st.com/media/catalog/product/m/i/miniso-8_1.jpg?quality=80&bg-color=255,255,255&fit=bounds&height=&width=" width="300"/>
  Un arduino per amplificare i segnali GPIO usa un amplificatore in corrente continua detto Analog Comparator(modello LMV358LIST-A.9)

---

# Amplificatore in corrente alternata
<p></p>

Gli amplificatori generalmente funzionano sia in corrente continua che in alternata, tuttavia, se noi amplifichiamo una corrente alternata in uscita risulterà sempre una piccola tensione in corrente continua(detta offset input) che dobbiamo stabilizzare aggiungendo un condensatore in uscita

<img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Amp2dtcx.jpg" />

---

# Costruiamo un amplificatore a transistor

Per costruire un amplificatore a transistor MOSFET, abbiamo bisogno di un transistor di tipo N, una resistenza da 20KOhm, un condensatore elettrolitico da 100 uF, uno speaker e un jack di ingresso.

<center>
  <img src="/images/ampli_normale.png" width="400"/>
</center>
---

# Osservazioni 
Se noi attacchiamo al circuito un generatore di funzioni che possiamo identificarlo nel nostro circuito come generatore di un suono e all'uscita attacchiamo un oscilloscopio per vedere l'amplificazione dell'onda possiamo osservare diverse caratteristiche:

- L'onda viene raddrizzata qualunque essa sia per effetto del condensatore
- L'onda viene amplificata da 1.5V a 1.84V circa in caso di tensione in ingresso di 1.5V

<div class="grid grid-cols-2 gap-2">
<div>
  <img src="/images/salita_istantanea.jpeg" />
  Crescita istantanea quando accendiamo il generatore di tensione
</div>
<div>
    <img src="/images/salita.jpeg" />
    Cambiando la scala del tempo riusciamo a vedere che l'accensione a 1.5V e poi l'amplificazione fino a 1.84V
    </div>
</div>

---

# Aggingiamo il volume e il tasto di accensione

Il nostro amplificatore adesso è molto basilare, non supporta il volume e non si può spegnere senza staccare l'alimentazione. Per fare queste modifiche prendiamo un potenziometro da 20Kohm e sostituiamolo alla resistenza

<center>
  <img src="/images/ampli_switch.png" width="400"/>
</center>