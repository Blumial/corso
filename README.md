<div align="center">

  <!-- HEADER GITHUB READ-ME -->
  <svg width="100%" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
    <rect width="800" height="200" rx="16" fill="#1e1e28" />
    <circle cx="100" cy="100" r="60" fill="#e53935" />
    <path d="M82,90 C82,85 86,81 91,81 L109,81 C114,81 118,85 118,90 L118,110 C118,115 114,119 109,119 L91,119 C86,119 82,115 82,110 Z" fill="none" stroke="#ffffff" stroke-width="3"/>
    <path d="M100,85 L100,115 M85,100 L115,100" stroke="#ffffff" stroke-width="4" stroke-linecap="round"/>
    <circle cx="125" cy="95" r="4" fill="#ffffff"/>
    <circle cx="133" cy="103" r="4" fill="#ffffff"/>
    <text x="180" y="80" fill="#ffffff" font-family="'Segoe UI', Roboto, sans-serif" font-weight="800" font-size="28">JAPAN MATSURI WORKSHOP</text>
    <text x="180" y="115" fill="#e53935" font-family="'Segoe UI', Roboto, sans-serif" font-weight="700" font-size="22">Dal Game Center al Platform 2D</text>
    <text x="180" y="145" fill="#a0a0b0" font-family="'Segoe UI', Roboto, sans-serif" font-size="14">15 min Storia dei Videogiochi + 45 min Sviluppo Pratico con Construct 3</text>
  </svg>

  # 🎮 Japan Matsuri: Costruiamo un Platform 2D

  [![Construct 3](https://img.shields.io/badge/Engine-Construct_3-blue.svg)](https://editor.construct.net/)
  [![Duration](https://img.shields.io/badge/Durata-1_Ora-orange.svg)](#)
  [![Level](https://img.shields.io/badge/Livello-Principiante-brightgreen.svg)](#)

</div>

---

## 📌 Indice del Workshop

1. [Parte 1: Storia del Videogioco Giapponese (15 min)](#-parte-1-storia-del-videogioco-giapponese-15-min)
2. [Parte 2: Sviluppo Pratico con Construct 3 (45 min)](#-parte-2-sviluppo-pratico-con-construct-3-45-min)
3. [Requisiti e Risorse](#-requisiti-e-risorse)

---

## 📜 Parte 1: Storia del Videogioco Giapponese (15 min)[cite: 1]

Un breve viaggio storico attraverso le tappe fondamentali che hanno definito la grammatica del genere platform[cite: 1]:

### 🕹️ 1978 — Il Boom dei Game Center[cite: 1]
* **Space Invaders (Taito):** Accende l'industria arcade in Giappone[cite: 1]. Il successo fu così travolgente da causare (secondo la leggenda) una temporanea carenza di monete da 100 yen[cite: 1].
* **Nascita dei Game Center:** Le sale giochi diventano luoghi fondamentali di aggregazione giovanile e socialità[cite: 1].
* **I grandi Publisher:** Nascono e si strutturano le aziende che domineranno il mercato: *Nintendo*, *Sega*, *Namco*, *Capcom*, *Konami*[cite: 1].

### 🦍 1981 — Nasce il Platform: Donkey Kong[cite: 1]
* **Shigeru Miyamoto:** Introduce per la prima volta una narrazione visiva strutturata su più livelli verticali[cite: 1].
* **Jumpman:** Debutta il personaggio che pochi anni dopo diventerà *Mario*[cite: 1].
* **La Grammatica Base:** Piattaforme da scalare, ostacoli in movimento da schivare e un obiettivo in cima alla schermata[cite: 1].

### 🍄 1985 — Super Mario Bros. e lo Scrolling[cite: 1]
* **Scrolling Orizzontale:** Il mondo di gioco non è più vincolato a una singola schermata fissa[cite: 1].
* **Level Design Didattico:** Il livello 1-1 insegna le regole del gioco in modo intuitivo senza bisogno di istruzioni scritte[cite: 1].
* **Rinascita dell'Industria:** Salva e rilancia il mercato globale dei videogiochi dopo la crisi del 1983[cite: 1].

### 🦔 1991 — Sonic & La Console War[cite: 1]
* **Sega Mega Drive:** Sfida il dominio Nintendo puntando sulla velocità pura[cite: 1].
* Il genere platform diventa il principale terreno di scontro d'immagine tra le due grandi compagnie negli anni '90[cite: 1].

### 🏃 Step 2: Assegnazione dei Comportamenti (Behaviors)
Seleziona ciascun oggetto e nel pannello **Properties -> Behaviors** aggiungi:

* **Player:**
  * Aggiungi il comportamento **`Platform`** (gestisce la gravità, la corsa e il salto con le frecce direzionali).
  * Aggiungi il comportamento **`Bound to layout`** (impedisce al giocatore di uscire dallo schermo).
* **SolidGround:**
  * Aggiungi il comportamento **`Solid`** (rende il blocco un ostacolo solido su cui ci si può appoggiare).

---

### 🧠 Step 3: Logica ed Event Sheet (Variabili e Collezionabili)

Passa alla scheda **Event Sheet** per programmare la logica del gioco:

#### 1. Creare la Variabile Globale del Punteggio
* Fai clic con il tasto destro nell'Event Sheet e seleziona **Add global variable**.
* Nome: `Score`
* Tipo: `Number`
* Valore iniziale: `0`

#### 2. Raccogliere la Moneta ed Incrementare lo Score
Aggiungi il seguente evento:

* **Condition:** `Player` ➡️ *On collision with another object* ➡️ seleziona `Coin`
* **Actions:**
  1. `System` ➡️ *Add to* ➡️ Variable: `Score`, Value: `1`
  2. `Coin` ➡️ *Destroy* (la moneta scompare dal livello)

---

## 📦 Requisiti e Risorse

* **Browser Web:** Google Chrome, Edge o Firefox (nessun software da installare).
* **Game Engine:** [Construct 3 Editor](https://editor.construct.net/)
* **Asset Grafici:** Sprite semplici o pixel art creati con l'editor integrato di Construct.

---
<div align="center">
  <sub>Workshop creato per Japan Matsuri • Realizzato con Construct 3</sub>
</div>
