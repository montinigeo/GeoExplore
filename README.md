# Simulazioni Interattive di Geologia

Raccolta di simulazioni didattiche interattive realizzate in HTML/JavaScript, senza dipendenze esterne. Ogni file è autonomo e funziona direttamente nel browser.

---

## 🚀 Lancia le simulazioni

### 🌋 Magmatismo e Metamorfismo

| Simulazione | Descrizione | Link |
|-------------|-------------|------|
| 🪨 Rocce Magmatiche | Streckeisen QAPF, piroclastiche, rocce speciali | [Apri](https://montinigeo.github.io/Simulazioni/rocce_magmatiche.html) |
| ⛰️ Rocce Mafiche e Ultramafiche | Ol-Opx-Cpx, Ol-Px-Plag, geodinamica, facies mantello | [Apri](https://montinigeo.github.io/Simulazioni/rocce_mafiche.html) |
| 📊 Serie Magmatiche | TAS, AFM, K₂O-SiO₂, Na₂O-K₂O, percorsi geodinamici | [Apri](https://montinigeo.github.io/Simulazioni/serie_magmatiche.html) |
| 🔥 Serie di Bowen | Cristallizzazione frazionata, quattro tipi di magma | [Apri](https://montinigeo.github.io/Simulazioni/serie_bowen.html) |
| 🌿 Metamorfismo | Facies P-T, percorsi geodinamici, Barrow, protoliti | [Apri](https://montinigeo.github.io/Simulazioni/metamorfismo.html) |

### 🔬 Petrografia

| Simulazione | Descrizione | Link |
|-------------|-------------|------|
| 💎 Diagrammi di Fase | Ab-An, Di-An, Lc-SiO₂, Ab-Or (fusi silicatici) | [Apri](https://montinigeo.github.io/Simulazioni/diagrammi_fase.html) |
| 🔬 Microscopio Polarizzato | Ortoscopica, conoscopica, lamina λ, Michel-Lévy | [Apri](https://montinigeo.github.io/Simulazioni/microscopio_polarizzato.html) |
| ⚛️ Diffrattometro XRD | Diffrazione a raggi X, legge di Bragg | [Apri](https://montinigeo.github.io/Simulazioni/diffrattometro_xrd_v5.html) |

### 📡 Geofisica

| Simulazione | Descrizione | Link |
|-------------|-------------|------|
| 🌀 Moto Armonico | Fasore, spostamento, velocità, accelerazione | [Apri](https://montinigeo.github.io/Simulazioni/moto_armonico.html) |
| 🌍 Onde Sismiche | Onde P, S, PKP con raggi curvilinei e struttura interna | [Apri](https://montinigeo.github.io/Simulazioni/onde_sismiche.html) |
| 📡 DInSAR | Interferometria SAR differenziale, deformazione del suolo | [Apri](https://montinigeo.github.io/Simulazioni/dinsar.html) |
| 🛰️ Visibilità SAR Frane | Geometria di acquisizione SAR e ombre topografiche | [Apri](https://montinigeo.github.io/Simulazioni/visibilita_sar_frane.html) |

---

## 📖 Descrizione delle simulazioni

---

<a name="rocce-magmatiche"></a>
## 🪨 Rocce Magmatiche — Classificazione IUGS

**File:** `rocce_magmatiche.html`

Classificazione completa delle rocce magmatiche secondo lo standard IUGS (Le Maitre 2002), organizzata in quattro schede tematiche.

### Schede

**Streckeisen (QAPF)**
- Doppio triangolo QAP (rocce sature e sovrasaturate) e FAP (rocce sottosaturate) con 20 + 10 campi classificativi
- Toggle plutoniche/vulcaniche: le sigle e i nomi si aggiornano in tutti i settori e nel pannello laterale
- Hover interattivo: composizione mineralogica, SiO₂, struttura e giacitura per ogni settore
- Zona F=0–10% evidenziata come transizione verso il QAP (rocce "a feldspatoidi" accessori)

**Rocce Mafiche** (triangolo Ol-Opx-Cpx)
- Sette campi ultramafia con confini IUGS corretti: Cpx/(Cpx+Opx) = 10% e 90% come discriminanti
- Dunite, Harzburgite, Lherzolite, Wehrlite, Ortopirossenite, Websterite, Clinopirossenite

**Piroclastiche**
- Schema a matrice: granulometria dei clasti (blocchi → cenere fine) × composizione (basaltica → riolitica)
- Sette tipi di rocce consolidate: agglomerato, breccia piroclastica, tufo lapillistico, tufo, ignimbrite, surge, lahar
- Origine eruttiva, forma del deposito, esempi e note per ciascun tipo

**Rocce Speciali**
- Posizionate in un diagramma K₂O vs SiO₂ nelle loro zone geochimiche reali
- Kimberlite, Lamproite, Carbonatite, Komatiite, Fonolite, Leucitite
- Scheda dettagliata con minerali, profondità sorgente, esempi mondiali e nota petrografica

---

<a name="rocce-mafiche"></a>
## ⛰️ Rocce Mafiche e Ultramafiche

**File:** `rocce_mafiche.html`

Approfondimento delle rocce basiche e ultramafiche con quattro diagrammi complementari.

### Schede

**Ol-Opx-Cpx (IUGS)**
- Triangolo ternario con confini corretti secondo Le Maitre (2002)
- Peridotiti (Ol>40%): Dunite, Harzburgite, Lherzolite, Wehrlite
- Pirosseniti (Ol<40%): Ortopirossenite, Websterite, Clinopirossenite
- Hover interattivo con mineralizzazione, SiO₂, densità e giacitura

**Ol-Px-Plag (IUGS)**
- Triangolo per la classificazione dei gabbri e rocce basiche con plagioclasio
- Otto campi: Dunite, Wehrlite, Olivin-Pirossenite, Pirossenite, Troctolite, Gabbro Olivinico, Gabbro/Norite, Anortosite

**Geodinamica**
- Sezione litostratigrafica verticale per quattro contesti tettonici
- Sequenza ofiolitica completa (tipo Penrose 1972): sedimenti → basalti a pillow → sheeted dykes → gabbri → zona di transizione → peridotite mantellica
- Mantello d'arco: cuneo del mantello, metasomatismo da fluidi della lastra
- Mantello cratonico: radice litosferia spessa, zona diamante, kimberliti
- Rift/Hotspot: zona di fusione parziale, plume mantellico

**Facies del Mantello**
- Diagramma P-T (400–1800°C, 0–10 GPa) con campi di stabilità di plagioclasio, spinello, granato e diamante nel peridotite
- Confini empirici da Green & Ringwood (1970) e O'Neill (1981)
- Solidus secco del peridotite (McKenzie & Bickle 1988)
- Tre percorsi geodinamici animati: subduzione oceanica, risalita astenosferica, radice cratonico

---

<a name="serie-magmatiche"></a>
## 📊 Serie Magmatiche — Classificazione Geochimica

**File:** `serie_magmatiche.html`

Quattro diagrammi geochimici complementari per la classificazione delle serie magmatiche, con campioni non ambigui selezionati per coerenza tra i diagrammi.

### Schede

**TAS (Total Alkali vs Silica)**
- Campi delle rocce secondo Le Bas et al. (1986): 15 campi nominati
- Linea MacDonald-Katsura (formula lineare corretta: Na₂O+K₂O = 13.5 − 0.19·SiO₂) per separare alcalino da subalcalino
- Aree degli inviluppi per cinque serie: tholeiitica, calcalcalina, alcalina, shoshonitica, alcalina K-ricca
- Nota: la shoshonitica appare sopra la linea M-K nel TAS ma è geochimicamente subalcalina (distinzione su K₂O/Na₂O e Nb/Ta)

**AFM (triangolo ternario)**
- A = Na₂O+K₂O, F = FeOtot, M = MgO
- Trend animati per serie tholeiitica (arricchimento in Fe) e calcalcalina (trend verso M)
- Confine di Irvine & Baragar (1971) come toggle opzionale
- Campioni posizionati: MORB, Andesite, Dacite, Basalto alcalino, Shoshonite

**K₂O vs SiO₂**
- Bande di Peccerillo & Taylor (1976) come rette con pendenza corretta (0.067, calibrata sui dati originali)
- Quattro bande: Bassa-K (tholeiitica), Media-K (calcalcalina), Alta-K (shoshonitica), Molto alta-K (alcalina K-ricca)
- Quattro percorsi geodinamici animati (inizialmente spenti): Arco di subduzione, Hotspot/Isola, Rift continentale, Dorsale oceanica
- Campioni: MORB, Andesite, Dacite, Riolite, Shoshonite, Leucitite, Tefrite Vesuvio

**Na₂O vs K₂O**
- Linea Na₂O = K₂O come discriminante tra alcaline sodiche (Na>K: rift, hotspot) e potassiche (K>Na: post-collisione, shoshonitica)
- Campi indicativi per le cinque serie
- Campioni: MORB, Basalto alcalino, Fonolite, Shoshonite, Trachite, Leucitite, Tefrite Vesuvio

---

<a name="serie-bowen"></a>
## 🔥 Serie di Bowen — Cristallizzazione Frazionata

**File:** `serie_bowen.html`

Simulazione animata della cristallizzazione frazionata nei magmi secondo la serie di Bowen, con quattro tipologie di magma.

### Funzionalità

- **Quattro magmi**: Basaltico, Andesitico, Riolitico, Ideale (tutti i minerali presenti)
- **Serie continua**: barra a gradiente con indicatore An% (anortite nel plagioclasio) mobile durante la cristallizzazione
- **Serie discontinua**: Olivina → Pirosseno → Anfibolo → Biotite con intervalli di temperatura
- **Composizione finale normalizzata** al 100% per ciascun magma
- Barre pre-cristallizzazione con bordo colorato che si riempiono progressivamente

---

<a name="metamorfismo"></a>
## 🌿 Metamorfismo — Facies e Percorsi P-T

**File:** `metamorfismo.html`

Simulazione interattiva del metamorfismo in un diagramma pressione-temperatura (P-T).

### Funzionalità

- **Diagramma P-T** (150–900°C, 0–30 kbar) con nove facies colorate secondo IUGS: Zeoliti, Prehnite-Pumpellyite, Scisti Verdi, Anfibolitica, Granuliti, Scisti Blu, Eclogiti, UHP, Hornfels (con tre sottofacies termiche)
- **Cinque protoliti**: Granito/Gneiss, Basalto/Gabbro, Arenaria, Pelite, Calcare/Marna — con mineralizzazione e roccia risultante per ogni facies
- **Quattro percorsi P-T animati**: Subduzione oceanica (blu), Collisione continentale (rosso), Metamorfismo di contatto (arancio), Ultra-Alta Pressione UHP (viola)
- **Sequenza di Barrow** (solo pelite): toggle indipendente per facies e minerali indice (clorite, biotite, granato, staurolite, cianite, sillimanite, cordierite)

---

<a name="diagrammi-fase"></a>
## 💎 Diagrammi di Fase — Fusi Silicatici

**File:** `diagrammi_fase.html`

Quattro diagrammi di fase binari per sistemi silicatici fondamentali in petrologia magmatica.

### Sistemi inclusi

- **Ab-An** (Albite-Anortite): soluzione solida completa con liquidus e solidus continui. Base per la comprensione del plagioclasio
- **Di-An** (Diopside-Anortite): sistema con eutettico semplice a ~1274°C, An=42%. Modello per gabbri e basalti
- **Lc-SiO₂** (Leucite-Silice): sistema con punto peritettico — cristallizzazione incongruente della leucite verso feldspato K. Fondamentale per i magmi potassici
- **Ab-Or** (Albite-Ortoclasio): solvus e miscibilità parziale. Illustra l'evoluzione dei graniti e la pertitizzazione

---

<a name="microscopio"></a>
## 🔬 Microscopio Polarizzato

**File:** `microscopio_polarizzato.html`

Simulazione interattiva di un microscopio petrografico a luce polarizzata.

### Funzionalità

- **Modalità ortoscopica** e **conoscopica** con toggle
- Selezione di minerali uniassici (quarzo, calcite, turmalina) e biassici (muscovite, biotite, olivina, orneblenda)
- **Tavola Michel-Lévy**: indicatori di addizione (blu) e sottrazione (arancio) per la lamina λ=550 nm
- Rotazione della platina con aggiornamento in tempo reale delle figure di interferenza

---

<a name="xrd"></a>
## ⚛️ Diffrattometro XRD

**File:** `diffrattometro_xrd_v5.html`

Simulazione di diffrazione a raggi X su polveri cristalline.

### Funzionalità

- Visualizzazione geometrica della legge di Bragg: nλ = 2d·sinθ
- Selezione di minerali comuni con spaziature reticolare d caratteristiche
- Diffractogramma interattivo con picchi di diffrazione

---

<a name="moto-armonico"></a>
## 🌀 Moto Armonico Periodico

**File:** `moto_armonico.html`

Simulazione del moto armonico con rappresentazione fasoriale.

### Funzionalità

- Piano fasoriale con fasore rotante e proiezione sull'asse reale
- Grafico temporale di spostamento, velocità e accelerazione
- Slider per frequenza (0.2–4 Hz), ampiezza e fase iniziale

---

<a name="onde-sismiche"></a>
## 🌍 Onde Sismiche — Struttura Interna della Terra

**File:** `onde_sismiche.html`

Propagazione delle onde sismiche attraverso la struttura interna della Terra.

### Funzionalità

- **Tre schede**: Onde P (con PKP verde lime), Onde S, Struttura interna
- **Raggi curvilinei** calcolati con integrazione numerica della legge di Snell sferica
- Raggi simmetrici rispetto all'asse verticale, slider per l'angolo di partenza
- Zona d'ombra delle onde P (103°–143°) con spiegazione fisica

---

<a name="dinsar"></a>
## 📡 DInSAR — Interferometria SAR Differenziale

**File:** `dinsar.html`

Simulazione della tecnica DInSAR per la misura della deformazione del suolo.

### Funzionalità

- Geometria di acquisizione SAR con orbite ascendente e discendente
- Calcolo della deformazione in linea di vista (LOS) da due acquisizioni
- Interferogramma con frange di deformazione e unwrapping della fase

---

<a name="sar-frane"></a>
## 🛰️ Visibilità SAR e Frane

**File:** `visibilita_sar_frane.html`

Analisi della geometria di acquisizione SAR in relazione alla topografia e alle frane.

### Funzionalità

- Simulazione dell'angolo di incidenza locale in funzione della pendenza del versante
- Zone di foreshortening, layover e ombra radar
- Applicazione alla mappatura delle frane con SAR

---

## Autore

Simulazioni sviluppate da Giovanni Montini con l'assistenza di Claude (Anthropic).

## Licenza

Libero uso per scopi didattici e divulgativi.
