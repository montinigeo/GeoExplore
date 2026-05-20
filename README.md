# Simulazioni Interattive

Raccolta di simulazioni didattiche interattive realizzate in HTML/JavaScript, senza dipendenze esterne. Ogni file è autonomo e funziona direttamente nel browser.

### 🚀 Lancia le simulazioni

| Simulazione | Link diretto |
|-------------|-------------|
| [🌀 Moto Armonico Periodico](#moto-armonico) | [Apri](https://montinigeo.github.io/Simulazioni/moto_armonico.html) |
| [⚛️ Diffrattometro XRD](#xrd) | [Apri](https://montinigeo.github.io/Simulazioni/diffrattometro_xrd_v5.html) |
| [📡 DInSAR — Interferometria Radar Differenziale](#dinsar) | [Apri](https://montinigeo.github.io/Simulazioni/dinsar.html) |
| [🛰️ Visibilità SAR Frane](#sar-frane) | [Apri](https://montinigeo.github.io/Simulazioni/visibilita_sar_frane.html) |
| [🔥 Diagrammi di Fase — Fusi Silicatici](#diagrammi-fase) | [Apri](https://montinigeo.github.io/Simulazioni/diagrammi_fase.html) |
| [🔬 Microscopio Polarizzato](#microscopio) | [Apri](https://montinigeo.github.io/Simulazioni/microscopio_polarizzato.html) |
| [🌋 Serie di Bowen](#serie-bowen) | [Apri](https://montinigeo.github.io/Simulazioni/serie_bowen.html) |
| [🌍 Onde Sismiche](#onde-sismiche) | [Apri](https://montinigeo.github.io/Simulazioni/onde_sismiche.html) |
| [🪨 Metamorfismo](#metamorfismo) | [Apri](https://montinigeo.github.io/Simulazioni/metamorfismo.html) |

---

<a name="moto-armonico"></a>
## 🌀 Moto Armonico Periodico

**File:** `moto_armonico.html`

Simulazione interattiva del moto armonico periodico, con rappresentazione simultanea del piano fasoriale e dell'andamento temporale.

### Contenuto

Il moto armonico è descritto dall'equazione:

```
x(t) = A · cos(ωt + φ₀)
```

La simulazione mostra la connessione tra il **moto circolare uniforme** (piano fasoriale) e il **moto armonico** (proiezione sull'asse reale), permettendo di visualizzare le tre grandezze cinematiche normalizzate:

- **Spostamento** x(t) = cos(ωt + φ₀)
- **Velocità** v(t) = −sin(ωt + φ₀)
- **Accelerazione** a(t) = −cos(ωt + φ₀)

### Funzionalità

- Regolazione interattiva di **frequenza** (0.2–4 Hz), **ampiezza** e **fase iniziale** tramite slider
- Selezione del parametro da visualizzare nel grafico temporale (spostamento, velocità, accelerazione) con radio button
- Fasore rotante che cambia direzione in base al parametro selezionato:
  - Posizione → radiale
  - Velocità → tangenziale (+90°)
  - Accelerazione → centripeta (verso il centro)
- Visualizzazione opzionale dei vettori sull'asse x del piano fasoriale
- Marcatori verticali nel grafico temporale al cambio di parametri
- Forma trigonometrica e fasoriale aggiornate in tempo reale
- Layout responsive (PC e mobile)

---

<a name="xrd"></a>
## ⚛️ Diffrattometro XRD

**File:** `diffrattometro_xrd_v5.html`

Simulazione interattiva di un diffrattometro a raggi X per polveri, basata sulla **legge di Bragg**:

```
nλ = 2d · sin(θ)
```

### Contenuto

La diffrazione a raggi X è una tecnica fondamentale per la determinazione della struttura cristallina dei minerali e dei materiali. Quando un fascio di raggi X colpisce un campione policristallino, i piani reticolari con spaziatura *d* soddisfano la condizione di Bragg per un angolo θ specifico, generando un picco di diffrazione a 2θ nel diffrattogramma.

### Materiali inclusi

| Materiale | Sistema cristallino | Gruppo |
|-----------|-------------------|--------|
| NaCl (alite) | Cubico — Fm3̄m | — |
| Si (silicio) | Cubico — Fd3̄m | — |
| Al (alluminio) | Cubico — Fm3̄m | — |
| Quarzo (SiO₂) | Trigonale — P3₁21 | Tettosilicato |
| TiO₂ (rutilo) | Tetragonale — P4₂/mnm | — |
| FeO (wüstite) | Cubico — Fm3̄m | — |
| Olivina Fo | Ortorombico — Pbnm | Nesosilicato |
| Epidoto | Monoclino — P2₁/m | Sorosilicato |
| Berillo | Esagonale — P6/mcc | Ciclosilicato |
| Diopside | Monoclino — C2/c | Inosilicato (pirosseno) |
| Muscovite | Monoclino — C2/c | Fillosilicato |
| Anortite | Triclino — P1̄ | Tettosilicato (feldspato) |

### Funzionalità

- **Schema ottico** con sorgente, campione e rivelatore in geometria reale
- Due geometrie selezionabili:
  - **Bragg-Brentano** (θ/2θ): campione rotante, sorgente fissa
  - **θ-θ**: campione fisso, sorgente e rivelatore si muovono simmetricamente
- Quattro sorgenti disponibili: Cu Kα, Mo Kα, Co Kα, Cr Kα (lunghezze d'onda reali)
- **Diffrattogramma** costruito in tempo reale durante la scansione automatica o manuale
- Tabella dei picchi attesi con indici di Miller (hkl), spaziatura d e intensità relativa I/I₀
- Identificazione automatica dei picchi con etichette hkl
- Campione rappresentato come rettangolo rotante (BB) o fisso (θ-θ) con piani reticolari visibili
- Angoli θ e 2θ visualizzati come archi crescenti sul goniometro
- Layout responsive (PC: schema e diffrattogramma affiancati; mobile: verticale)

---

<a name="dinsar"></a>
## 📡 DInSAR — Interferometria Radar Differenziale da Satellite

**File:** `dinsar.html`

Simulazione animata del principio fisico dell'**Interferometria Radar Differenziale da Satellite (DInSAR)**, tecnica utilizzata per misurare spostamenti del suolo millimetrici da piattaforme orbitali (es. Sentinel-1, ALOS-2, COSMO-SkyMed).

### Contenuto

Il DInSAR si basa sul confronto della fase delle onde radar ricevute in due acquisizioni successive (T1 e T2) dello stesso bersaglio. La differenza di fase è legata allo spostamento del bersaglio lungo la linea di vista (LOS):

```
Δφ = 4π · Δd / λ   →   Δd = λ · Δφ / (4π)
```

L'ambiguità intrinseca è ±n·λ/2 (spostamenti multipli di λ/2 producono la stessa differenza di fase).

### Struttura della simulazione

L'animazione si articola in sei fasi sequenziali:

1. **T1 — emissione**: il satellite illumina il bersaglio; l'onda parte da y=0 al satellite e percorre la LOS accumulando fase
2. **T1 — ritorno**: l'onda riflessa riparte da y=0 al bersaglio e torna al satellite con la fase accumulata φ₁ = (4πR₁/λ) mod 2π
3. **Transizione**: dissolvenza di T1
4. **T2 — emissione**: seconda acquisizione; il bersaglio si è spostato di Δd lungo la LOS
5. **T2 — ritorno**: l'onda di ritorno porta la fase φ₂ = (4πR₂/λ) mod 2π, diversa da φ₁
6. **Confronto**: le due onde di ritorno vengono sovrapposte; Δφ è evidenziato graficamente con la distanza tra le creste e la formula di conversione in spostamento

### Layout

- **Pannello sinistro**: geometria di acquisizione con satellite, bersaglio, LOS e punto mobile animato
- **Pannello centrale**: segnale radar T1 (andata + ritorno)
- **Pannello destro**: segnale radar T2 (andata + ritorno)
- **Pannello inferiore**: confronto tra le onde di ritorno T1 e T2, con Δφ evidenziato e formula finale

### Parametri fisici

- Banda C (Sentinel-1): λ = 5.6 cm
- Angolo di incidenza LOS: 35°
- Baseline orbitale: 0 m (per semplicità didattica)
- Spostamento del bersaglio Δd: regolabile con slider (−λ/4 ÷ +λ/4 = −1.4 ÷ +1.4 cm)

Il range è limitato a **±λ/4** perché questo è il massimo spostamento misurabile senza ambiguità di fase. Il segnale radar percorre il tragitto andata+ritorno, quindi la fase accumulata è Δφ = 4π·Δd/λ: uno spostamento di λ/4 produce esattamente Δφ = 180°, il massimo distinguibile. Superato questo valore la fase si "avvolge" (phase wrapping) e il satellite non è in grado di distinguere lo spostamento reale da quello apparente. Per questo motivo lo sfasamento misurato è sempre espresso come Δd_mis ± n·λ/2, dove n è un intero incognito che rappresenta l'ambiguità di fase intera.

---

<a name="sar-frane"></a>
## 🛰️ Visibilità SAR Frane

**File:** `visibilita_sar_frane.html`

Dashboard interattivo per l'analisi della **visibilità geometrica SAR** di aree in frana, basato sui principi della geometria di acquisizione dei satelliti radar ad apertura sintetica (SAR/InSAR).

### Contenuto

La visibilità di una frana da satellite dipende dall'orientamento della direzione principale di movimento della frana rispetto alla geometria di acquisizione del satellite (azimut e angolo off-nadir). Lo strumento, ipotizzando che il dissesto gravitativo si muova lungo la direzione di massima pendenza del versante, calcola, per ogni combinazione di aspect/slope configurabile dall'utente, quale è la percentuale di movimento effettivamente rilevabile dal satellite nelle orbite ascendente e discendente. Inoltre, viene proposto un diagramma conbinato di visibilità confrontando le due orbite.

### Funzionalità

- **Diagrammi polari** (aspect 0°–360° × slope 0°–90°) per orbita ascendente, discendente e visibilità combinata
- Scala di colore continua 0–100% per i diagrammi singoli
- Mappa a quattro classi per il diagramma combinato:
  - 🟢 ASC ≥50% e DESC ≥50% — ottima copertura
  - 🔴 ASC <50% e DESC <50% — scarsa copertura
  - 🔵 Solo ASC ≥50% — visibile solo in ascendente
  - 🟠 Solo DESC ≥50% — visibile solo in discendente
- **Calcolo puntuale** interattivo: inserendo aspect e slope si ottengono percentuali di visibilità e classe per il satellite selezionato
- Tooltip con valori precisi al passaggio del mouse sui diagrammi
- Preset per i principali satelliti SAR: Sentinel-1, ALOS-2, COSMO-SkyMed, ICEYE e altri
- Parametri personalizzabili (azimut e off-nadir per orbite ASC e DESC)
- Tre livelli di risoluzione del diagramma (1°, 2°, 5°)
- Layout responsive (PC: tre pannelli affiancati; tablet/mobile: ridisposizione automatica)

---

<a name="diagrammi-fase"></a>
## 🔥 Diagrammi di Fase — Fusi Silicatici Binari

**File:** `diagrammi_fase.html`

Simulazioni interattive dei quattro principali diagrammi di fase binari della petrologia ignea. Ogni diagramma anima il percorso di raffreddamento di un fuso silicatico, mostrando in tempo reale la composizione del liquido (punto ciano), la composizione del solido (punto arancio) e la temperatura corrente (punto verde).

### I. Albite — Anortite (Ab-An): soluzione solida completa

Ab (NaAlSi₃O₈) e An (CaAl₂Si₂O₈) sono completamente miscibili allo stato solido e liquido. Il liquidus è fortemente curvo, il solidus quasi lineare. Durante il raffreddamento il solido che cristallizza è sempre più ricco in An rispetto al liquido coesistente (principio della leva). La composizione finale del solido coincide con la composizione iniziale del fuso per conservazione della massa.

**Dati:** tabelle termodinamiche sperimentali (Bowen 1913).

### II. Diopside — Anortite (Di-An): eutettico semplice

Di (CaMgSi₂O₆) e An non sono miscibili allo stato solido. Il sistema presenta un eutettico E a 42% An, 1274°C. A sinistra di E cristallizza Di puro, a destra An puro; all'eutettico la temperatura rimane costante fino alla completa solidificazione. La pausa all'eutettico è animata esplicitamente (2 secondi).

**Dati:** Bowen (1915).

### III. Leucite — SiO₂ (Lc-SiO₂): peritettico + eutettico

Il sistema più complesso dei quattro. Il K-feldspato/Sanidino (Sa) è un composto intermedio che si forma per reazione peritettica Lc+L→Sa a 1557°C. Sono simulate tre situazioni distinte in base alla composizione iniziale:

- **cx ≤ 17.8%** — il liquido si esaurisce al peritettico: solido finale **Lc + Sa**
- **17.8% < cx < 40%** — tutta la Lc si converte, il liquido residuo raggiunge l'eutettico: solido finale **Sa + SiO₂**
- **cx ≥ 40%** — nessuna Lc, percorso diretto verso l'eutettico a 1080°C: solido finale **Sa + SiO₂**

La composizione percentuale del solido finale è calcolata dalla regola della leva e visualizzata al termine dell'animazione.

**Dati:** Bowen (1914), Schairer & Bowen (1947).

### IV. Albite — Ortoclasio (Ab-Or): due soluzioni solide + solvus

Ab (NaAlSi₃O₈) e Or/Sanidino (KAlSi₃O₈) mostrano due campi di soluzione solida completa che convergono a un minimo di fusione a 37% Or, 1063°C (punto termodinamico, non un minerale specifico). Sotto il solidus si forma una soluzione solida omogenea (alkali feldspar). Sotto il solvus (picco a ~660°C) la diversa dimensione di Na⁺ e K⁺ provoca l'essoluzione pertitica: i due feldspati si separano per diffusione allo stato solido in lamelle alternate di Ab-ricca e Or-ricca (pertite). La velocità di raffreddamento determina la grossolanità della pertite. Il diagramma usa un **asse spezzato** per mostrare simultaneamente i due lobi L+S (1000–1170°C) e la campana del solvus (400–800°C).

**Dati:** Bowen & Tuttle (1950), Morse (1970), Thompson & Waldbaum (1969).

### Funzionalità comuni

- Slider composizione iniziale (% componente B)
- Animazione con controllo velocità (0.5×–3×) e pausa/riavvio
- Punto **ciano** sulla composizione del liquido (liquidus), punto **arancio** sulla composizione del solido (solidus), punto **verde** sulla temperatura corrente
- Pause di 2 secondi agli invarianti (eutettico, peritettico)
- Composizione finale del solido calcolata dalla regola della leva e visualizzata nel pannello laterale
- Velocità di raffreddamento uniforme in tutte le zone del diagramma
- Interfaccia dark theme coerente con le altre simulazioni della raccolta

---

<a name="microscopio"></a>
## 🔬 Microscopio Polarizzato — Ottica Cristallografica

**File:** `microscopio_polarizzato.html`

Simulazione interattiva del microscopio ottico a luce polarizzata per lo studio delle proprietà ottiche dei minerali in sezione sottile. Include 12 minerali preimpostati (quarzo, calcite, olivina, pirosseni, feldspati, miche, silicati alluminosi) con i rispettivi parametri ottici, e permette di impostare birifrangenza e spessore personalizzati.

### Funzionalità

- **Modalità ortocopica**: visualizzazione del colore di interferenza in funzione di birifrangenza (Δn), spessore (µm) e orientazione del cristallo rispetto all'asse ottico (uniassici) o alla bisettrice acuta Bxa (biassici); intensità modulata secondo la formula I = sin²(2θ)·sin²(πΓ/λ)
- **Modalità conoscopica**: figura di interferenza calcolata pixel per pixel — croce nera e isocromi circolari per uniassici (Biot-Fouquet), isogiure iperboliche e due melatopi per biassici; angolo di inclinazione della sezione regolabile con deformazione realistica della figura
- **Rotazione piatto**: manuale tramite slider o automatica continua
- **Nicol incrociati / paralleli**: toggle istantaneo
- **Lamina compensatrice λ (550 nm)**: inseribile in modalità conoscopica per la determinazione del segno ottico; asse lento a 45° NE-SW con visualizzazione dell'effetto di addizione/sottrazione sulle isocromi
- **Tavola di Michel-Lévy**: visualizzata in tempo reale nel pannello destro con indicatore mobile della posizione corrente e linee diagonali degli spessori (10–60 µm)
- Pannello informativo con Δn apparente, ritardo Γ (nm) e ordine di interferenza aggiornati in tempo reale
---

<a name="serie-bowen"></a>
## 🌋 Serie di Bowen — Cristallizzazione Magmatica

**File:** `serie_bowen.html`

Simulazione interattiva della cristallizzazione frazionata dei magmi secondo la serie di Bowen. Il diagramma mostra le due serie su scala termica (1950°C → 580°C): la **serie discontinua** a sinistra (olivina → pirosseno → anfibolo → biotite → K-feldspato) e la **serie continua** a destra (plagioclasi da An₁₀₀ ad An₀), con il quarzo come termine finale di convergenza.

### Funzionalità

- Quattro tipi di magma selezionabili: **Basaltico**, **Andesitico**, **Riolitico** e **Ideale** (sequenza completa teorica di Bowen)
- Animazione del raffreddamento con linea di temperatura mobile e riempimento progressivo delle barre dei minerali
- Evidenziazione lampeggiante dei minerali in cristallizzazione; quando più fasi cristallizzano simultaneamente vengono mostrate tutte nel pannello laterale
- Scheda informativa per ogni minerale: formula, sistema cristallino, clivaggio, note petrologiche e rocce tipiche
- Al termine della cristallizzazione: composizione percentuale approssimativa della roccia risultante (normalizzata a 100%)
- La serie continua dei plagioclasi è rappresentata come unica barra a gradiente con indicatore mobile della composizione An corrente


---

<a name="onde-sismiche"></a>
## 🌍 Onde Sismiche — Struttura Interna della Terra

**File:** `onde_sismiche.html`

Simulazione interattiva della propagazione delle onde sismiche attraverso la Terra e della struttura interna del pianeta. Le traiettorie dei raggi sono calcolate con integrazione numerica della legge di Snell in forma sferica, tenendo conto del gradiente di velocità che produce le caratteristiche traiettorie curve.

### Struttura

La simulazione è organizzata in tre schede:

- **Onde P** — selezione del singolo raggio con slider dell'angolo di partenza (0° = verticale/profondo, 90° = orizzontale/superficiale). Mostra sia le P nel mantello (ciano) che le PKP che attraversano il nucleo (giallo), con spiegazione della rifrazione al confine di Gutenberg e della zona d'ombra (103°–143°)
- **Onde S** — stessa struttura. I raggi con angolo piccolo si fermano al confine di Gutenberg perché il nucleo esterno è liquido e non trasmette onde di taglio; i raggi più ripidi rimangono nel mantello
- **Struttura** — tutti i raggi P, PKP e S animati simultaneamente dall'epicentro, con i fronti d'onda in movimento; permette di apprezzare il pattern globale di propagazione e le zone d'ombra

### Elementi visualizzati

- Cinque strati interni colorati: crosta, mantello superiore, mantello inferiore, nucleo esterno (liquido), nucleo interno (solido)
- Discontinuità etichettate: Moho, 660 km, Gutenberg (CMB), Lehmann (ICB)
- Per ogni raggio: angolo di partenza, profondità massima raggiunta, distanza epicentrale di arrivo
- Pannello informativo con spiegazione fisica del percorso


---

<a name="metamorfismo"></a>
## 🪨 Metamorfismo — Facies e Percorsi P-T

**File:** `metamorfismo.html`

Simulazione interattiva del metamorfismo in un diagramma pressione-temperatura (P-T). Mostra le principali facies metamorfiche come campi colorati, i percorsi P-T dei diversi contesti geodinamici e le trasformazioni mineralogiche in funzione del protolite selezionato.

### Funzionalità

- **Diagramma P-T interattivo** (150–900°C, 0–30 kbar) con nove facies colorate: Zeoliti, Prehnite-Pumpellyite, Scisti Verdi, Anfibolitica, Granuliti, Scisti Blu, Eclogiti, UHP, Hornfels
- **Cinque protoliti selezionabili** (Granito/Gneiss, Basalto/Gabbro, Arenaria, Pelite, Calcare/Marna) con mineralizzazione e roccia risultante per ogni facies, mostrati in un pannello sovrapposto in alto a destra del diagramma
- **Quattro percorsi P-T** animati con punto mobile: Subduzione oceanica, Collisione continentale, Metamorfismo di contatto, Ultra-Alta Pressione (UHP)
- **Sequenza di Barrow** (solo pelite): due bottoni permettono di accendere/spegnere indipendentemente i campi delle facies e le ellissi dei minerali indice (clorite, biotite, granato, staurolite, cianite, sillimanite, cordierite)


---

## Autore

Simulazioni sviluppate da Giovanni Montini con l'assistenza di Claude (Anthropic).

## Licenza

Libero uso per scopi didattici e divulgativi.
