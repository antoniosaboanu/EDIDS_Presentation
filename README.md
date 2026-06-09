---
title: Daimyo Simulator - Presentazione Progetto
ga: ua-123456-1
mode: slide
theme: night
transition: slide
---

<style>
/* CSS per rendere le tue slide dinamiche e schematiche */
.reveal h2.ux-title {
    color: #fca311 !important;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 40px !important;
}
.ux-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 30px;
}
.ux-card {
    background: rgba(255, 255, 255, 0.05);
    border-top: 4px solid #fca311;
    padding: 20px;
    border-radius: 8px;
    text-align: center;
    transition: transform 0.2s;
}
.ux-card:hover { transform: scale(1.02); }
.ux-card i {
    font-size: 40px;
    color: #fca311;
    margin-bottom: 15px;
}
.ux-card h3 {
    font-size: 26px !important;
    color: #fff !important;
    margin-bottom: 10px;
}
.file-box {
    background: rgba(0, 0, 0, 0.3);
    border-left: 5px solid #14213d;
    padding: 15px;
    margin-bottom: 15px;
    border-radius: 4px;
    display: flex;
    align-items: center;
    gap: 15px;
}
.file-name {
    background: #fca311;
    color: #000;
    font-family: monospace;
    font-weight: bold;
    padding: 4px 10px;
    border-radius: 4px;
    font-size: 20px;
}
.file-desc {
    color: #e5e5e5;
    font-size: 22px;
    margin: 0 !important;
    text-align: left;
}
/* Colori tematici per i file */
.border-blue { border-left-color: #3a86ff !important; }
.bg-blue { background: #3a86ff !important; color: white !important; }
.border-green { border-left-color: #38b000 !important; }
.bg-green { background: #38b000 !important; color: white !important; }
.border-red { border-left-color: #d90429 !important; }
.bg-red { background: #d90429 !important; color: white !important; }
    
.reveal h1, .reveal h2, .reveal h3 {
    color: #e63946 !important;
    font-family: 'Playfair Display', serif;
}
.reveal p, .reveal li {
    font-size: 28px !important;
    text-align: justify;
}
.reveal .important-box {
    background: rgba(230, 57, 70, 0.1);
    border-left: 6px solid #e63946;
    padding: 15px;
    margin-top: 20px;
    border-radius: 4px;
}
.reveal .todo-box {
    background: rgba(241, 196, 15, 0.15);
    border-left: 6px solid #f1c40f;
    padding: 20px;
    margin-top: 20px;
    border-radius: 4px;
    text-align: left;
}
.reveal .todo-title {
    color: #f1c40f !important;
    font-weight: bold;
    font-size: 24px;
    margin-bottom: 10px;
    text-transform: uppercase;
}
</style>

# Daimyo Simulator
### Presentazione del Progetto

<br>
<p style="text-align: center !important; font-size: 24px !important; color: #aaa;">
    <b>Team di Sviluppo:</b><br>
    Antonio Saboanu, Edoardo Perissinotto, Luca Feggi, Mario Pepe
</p>

---

## Il Nostro Workflow
### Linea Temporale dello Sviluppo

## Il Nostro Workflow
### Linea Temporale dello Sviluppo

<br>

**Settimana 1** (Brainstorming & User Stories) ➔ **Settimane 2-4** (Stesura Codice & Ruoli) ➔ **Settimana 5** (Testing & Consegna)

<br>

<div class="important-box">
<p style="margin: 0 !important; font-size: 22px !important; text-align: center !important;">
    Un percorso di 5 settimane incentrato sul parallelismo tattico, disaccoppiamento architetturale e pulizia del codice.
</p>
</div>
---

## Prima Settimana
### Brainstorming & User Stories

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: center;">
<div>
<p>
    Ci siamo incontrati per buttare giù le idee fondanti del progetto. Abbiamo scelto come ambientazione una <b>città medievale nel Giappone feudale</b>.
</p>
<p>
    Una volta definite le caratteristiche fondamentali del gioco (gestione risorse, strutture operative, metriche di felicità/stabilità), abbiamo iniziato a scrivere, in maniera assistita con l'IA, le <b>User Stories</b> collegate alle nostre idee.
</p>
</div>
<div>
    <img src="https://images.unsplash.com/photo-1528164344705-4754268799af?auto=format&fit=crop&q=80&w=600" alt="Japan Temple" style="border-radius: 8px; border: 2px solid #e63946; box-shadow: 0 10px 20px rgba(0,0,0,0.5);">
</div>
</div>

---

## Seconda - Quarta Settimana
### Stesura Codice & Divisione Ruoli

<p>
    La maggior parte del tempo è stata impiegata a scrivere il codice dell'applicazione. Non avendo esperienze pregresse con strumenti grafici in Java (libGDX), la fase di setup iniziale e l'interfaccia grafica sono state assistite dall'IA per muovere rapidamente i primi passi.
</p>

<div class="important-box">
<p style="margin: 0 !important; font-weight: bold;">
    Separazione Netta delle Responsabilità:
</p>
<ul>
    <li><b>UX / UI (Grafica e Interazione):</b> Gestita da Antonio e Luca.</li>
    <li><b>Core Logic (Motore e Regole):</b> Gestita da Edoardo e Mario.</li>
</ul>
</div>


---

## Quinta Settimana
### Quality Testing & Foolproofing

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: center;">
<div>
<p>
    Abbiamo dedicato l'ultimo blocco di tempo a perfezionare e rifinire il progetto. 
</p>
<p>
    Abbiamo fatto provare il simulatore a <b>persone esterne</b> al team per individuare criticità nascoste, bug di stabilità o passaggi d'interfaccia poco chiari. L'obiettivo è stato rendere il gioco il più <b>foolproof (a prova di errore)</b> possibile prima della consegna finale.
</p>
</div>
<div>
    <img src="https://images.unsplash.com/photo-1600132806370-bf17e65e942f?auto=format&fit=crop&q=80&w=600" alt="Code Testing" style="border-radius: 8px; border: 2px solid #e63946; box-shadow: 0 10px 20px rgba(0,0,0,0.5);">
</div>
</div>

---

## User Stories & JIRA
### Gestione del Backlog e Task Allocations

<div class="todo-box">
    <div class="todo-title">SLIDE DA COMPLETARE — REQUISITO PER: MARIO PEPE</div>
    <p><b>Indicazioni per lo sviluppo della slide:</b></p>
    <ul>
        <li>Spiegare come hai strutturato JIRA e l'organizzazione delle User Stories.</li>
        <li>Dividere le User Stories in <b>macrogruppi logici</b>, ricalcando esattamente l'organizzazione degli Epic/Componenti usata sul software di gestione.</li>
        <li>Raccontare la gestione pratica dei task: come venivano descritte le storie includendo gli <b>Acceptance Criteria</b>.</li>
        <li>Spiegare il criterio di assegnazione dei ticket in base alle competenze delle coppie e al bilanciamento del carico di lavoro già assegnato.</li>
    </ul>
</div>

---

## Stesura del Codice
### La Struttura dell'Applicazione

<p style="text-align: center !important;">
    L'intera implementazione software di Daimyo Simulator è stata segmentata in tre macro-aree indipendenti e comunicanti:
</p>

<br>
<div style="display: flex; gap: 20px; justify-content: space-between;">
    <div style="background: rgba(255,255,255,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px;">
        <h3 style="color: #52b788 !important;">LOGICA</h3>
        <p style="font-size: 18px !important; text-align: center !important;">Motore matematico, tick e risorse.</p>
    </div>
    <div style="background: rgba(255,255,255,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px;">
        <h3 style="color: #4cc9f0 !important;">MOTORE GRAFICO</h3>
        <p style="font-size: 18px !important; text-align: center !important;">Rendering, Texture Atlas e Stage.</p>
    </div>
    <div style="background: rgba(255,255,255,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px;">
        <h3 style="color: #f72585 !important;">INTERAZIONE</h3>
        <p style="font-size: 18px !important; text-align: center !important;">Input router, comandi e pannelli UI.</p>
    </div>
</div>

---

## Struttura della Logica di Gioco
### Il Modulo Core del Simulatore

<div class="todo-box">
    <div class="todo-title">SLIDE DA COMPLETARE — REQUISITO PER: EDOARDO PERISSINOTTO</div>
    <p><b>Indicazioni per lo sviluppo della slide:</b></p>
    <ul>
        <li>Spiegare la struttura del backend logico (modulo daimyosimulator-core).</li>
        <li>Approfondire il funzionamento del motore a tick discreti e la gestione delle strutture dati delle risorse.</li>
        <li>Esporre le formule matematiche e le regole di bilanciamento (es. i rapporti per Sicurezza, Cultura, Craftsmanship, e i malus legati allo stock zero di Tools o Luxury).</li>
    </ul>
</div>

---

## Architettura del Motore Grafico
### Perché libGDX e Integrazione con Scene2D

<p>
    Fin dall'inizio abbiamo deciso di affidarci a un <b>framework dedicato al rendering 2D</b> piuttosto che a una libreria UI generica. libGDX lavora <b>a metà strada tra l'alto e il basso livello</b>: ci dà accesso diretto a <code>SpriteBatch</code>, texture, camera ortografica e al game loop (<code>render(delta)</code>), restando un sottile strato sopra OpenGL. Questo ci ha permesso di controllare in modo esplicito <b>cosa, dove e in che ordine</b> viene disegnato ogni frame — esattamente ciò che serve a un simulatore a griglia con sprite stratificati. Io avevo già esperienza con <b>SDL2 in C/C++</b>, di filosofia molto simile, quindi mi sono occupato io del setup del motore grafico.
</p>

<div class="important-box">
<p style="margin: 0 !important; font-size: 21px !important;"><b>Perché non JavaFX o Swing?</b> Sono toolkit pensati per <b>applicazioni desktop con widget</b>, non propriamente per giochi: niente game loop nativo, niente batching delle sprite né integrazione OpenGL pronta all'uso. Avrebbero reso scomodo il rendering continuo a 60 FPS della mappa, lo zoom pixel-perfect e il disegno per-frame degli sprite. libGDX è invece costruito attorno a questo caso d'uso.</p>
</div>

<p style="font-size: 22px !important;">
    Sopra il rendering grezzo, per tutta la <b>UI in-game</b> usiamo <b>Scene2D</b> (il modulo UI di libGDX): uno <code>Stage</code> fa da radice della scena e da router degli input, mentre pannelli come HUD, Build Menu e Market estendono <code>Table</code> per disporre <code>Actor</code> (Label, Image, TextButton) con un layout a griglia dichiarativo, senza calcolare coordinate a mano.
</p>

---

## Architettura del Motore Grafico
### Caricamento e Rendering della Mappa 2D

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 24px; align-items: center;">
<div>
<p>
    Tutti gli asset di gioco sono <b>singoli file PNG pre-tagliati</b> (un file per chiave: tile, edifici, feature naturali, icone). Al caricamento, il <code>SpriteSheetRegionRegistry</code> apre ogni file come <code>Texture</code>, vi applica <code>TextureFilter.Nearest</code> per mantenere il <b>pixel art nitido</b> in fase di zoom, e lo espone come <code>TextureRegion</code> tramite il <code>GameAssetManager</code>.
</p>
<p style="font-size: 22px !important;">
    Una chiave mancante non fa crashare il gioco: il manager logga l'errore e restituisce un <code>missing_asset</code> di fallback.
</p>
</div>
<div>
<div class="important-box">
<p style="margin: 0 !important; font-size: 20px !important;"><b>Pipeline di rendering per frame</b></p>
<p style="font-size: 18px !important; margin: 8px 0 0 0 !important;">
    Il <code>WorldRenderer</code> apre un solo <code>SpriteBatch</code> (allineato alla <code>OrthographicCamera</code>) e disegna a strati:
</p>
<ol style="font-size: 18px !important;">
    <li>Tiles del terreno</li>
    <li>Bordi di foresta</li>
    <li>Feature naturali</li>
    <li>Edifici (+ anteprima di costruzione)</li>
    <li>Animazioni</li>
</ol>
<p style="font-size: 17px !important; margin: 0 !important;">La griglia di selezione è sovrapposta come overlay finale.</p>
</div>
</div>
</div>

---

## Architettura del Motore Grafico
### Disaccoppiamento tra Logica e Rendering

<p>
    La scelta architetturale più importante del motore grafico è che <b>il rendering non conosce il dominio</b>. La logica di gioco non espone i suoi oggetti interni: a ogni tick produce un <code>VillageSnapshot</code> <b>immutabile</b>, una fotografia di sola lettura dello stato. Il <code>WorldRenderer</code> riceve quello snapshot e disegna, senza mai toccare né modificare il modello.
</p>

<div class="important-box">
<p style="margin: 0 !important; font-size: 21px !important;"><b>Vantaggi della separazione:</b> la coppia Logica (Edoardo, Mario) e la coppia Grafica (io, Antonio) hanno potuto lavorare <b>in parallelo</b> contro un contratto stabile — lo snapshot. Il motore grafico è sostituibile e testabile in isolamento, e non esiste accoppiamento bidirezionale tra le due metà del progetto.</p>
</div>

<p style="font-size: 22px !important;">
    Il ponte tra i due mondi è l'<b>Adapter</b> (<code>SnapshotToRenderModelAdapter</code>), che traduce ogni cella dello snapshot in un <code>CellRenderModel</code> pronto per il disegno. La risoluzione degli sprite passa invece per dei <b>Registry</b> dedicati (<code>BuildingSpriteRegistry</code>, <code>TileSpriteRegistry</code>, …): ognuno mappa un <b>enum di dominio</b> (es. <code>BuildingType</code>) sulla chiave testuale dell'asset, isolando in un solo punto la corrispondenza «entità ➔ immagine» e restituendo un <code>missing_asset</code> di fallback quando una chiave non esiste.
</p>

---

# Interazione Utente & UI Layout


<h2 class="ux-title">Cos'è la UX nel nostro simulatore?</h2>

<div class="ux-grid">
    <div class="ux-card" style="border-top-color: #3a86ff;">
        <i class="fa-solid fa-eye" style="color: #3a86ff;"></i>
        <h3 style="color: #000000 !important;">Interazione Fluida</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Select & Drag, navigazione mappa (Pan/Zoom) e interazione coerente coi bottoni senza conflitti.</p>
    </div>
    <div class="ux-card" style="border-top-color: #38b000;">
        <i class="fa-solid fa-eye" style="color: #38b000;"></i>
        <h3 style="color: #000000 !important;">Visibilità Contestuale</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">HUD organizzato a cornice. I menù e i dettagli (es. Market) appaiono solo quando selezioni una struttura.</p>
    </div>
    <div class="ux-card" style="border-top-color: #d90429;">
        <i class="fa-solid fa-bell" style="color: #d90429;"></i>
        <h3 style="color: #000000 !important;">Alert Significativi</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Pop-up cromatici (verde/rosso) e First-Time Warnings per educare il giocatore senza fare spam.</p>
    </div>
    <div class="ux-card" style="border-top-color: #9d4edd;">
        <i class="fa-solid fa-sliders" style="color: #9d4edd;"></i>
        <h3 style="color: #000000 !important;">Controllo Utente</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Menù Impostazioni facilmente accessibile, controllo velocità logica e opzioni di salvataggio veloci.</p>
    </div>
</div>

---

<h2 class="ux-title">I File dell'Interazione</h2>

<div class="file-box border-blue">
    <div class="file-name bg-blue">GameInputProcessor</div>
    <p class="file-desc" style="color: #ffffff !important;">Ascolta i click "grezzi". Ignora le azioni fuori dalla griglia e impedisce conflitti se l'utente sta cliccando sull'HUD.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">CameraController</div>
    <p class="file-desc" style="color: #ffffff !important;">Gestisce l'esplorazione: permette il "Select and Drag", il pan (WASD) e blocca lo zoom per non rompere la prospettiva.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">BuildModeState</div>
    <p class="file-desc" style="color: #ffffff !important;">La memoria a breve termine della UX: ricorda se stai solo esplorando, se hai in mano un edificio o il martello da demolizione.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">InputCommandRouter</div>
    <p class="file-desc" style="color: #ffffff !important;">Lo "smistatore". Prende il click convertito e decide: ispeziono la cella? Piazzo l'edificio? O cancello tutto?</p>
</div>

---

<h2 class="ux-title">I File dell'Interfaccia</h2>

<div class="file-box border-green">
    <div class="file-name bg-green">DashboardHud</div>
    <p class="file-desc" style="color: #ffffff !important;">La cornice madre. Racchiude BuildMenu, Risorse e parametri ai bordi, lasciando il centro dello schermo libero per giocare.</p>
</div>

<div class="file-box border-red">
    <div class="file-name bg-red">WarningPanel & EventModal</div>
    <p class="file-desc" style="color: #ffffff !important;">Gestiscono i First-Time Warnings (es. quando finisce il cibo) e mostrano gli eventi casuali sfruttando la psicologia dei colori.</p>
</div>

<div class="file-box border-green">
    <div class="file-name bg-green">SelectedBuildingPanel</div>
    <p class="file-desc" style="color: #ffffff !important;">UX contestuale: appare in basso solo quando ispezioni un edificio. Nasconde la complessità finché non la richiedi (es. tasto Trade).</p>
</div>

<div class="file-box border-green">
    <div class="file-name bg-green">SettingsModal / Dialogs</div>
    <p class="file-desc" style="color: #ffffff !important;">Modali in sovraimpressione per mettere in pausa e dare controllo su Salvataggi, Tutorial e regolazione Audio asincrona.</p>
</div>

---

<h2 class="ux-title">Persistenza: JSON & Memento Pattern</h2>
<div class="ux-grid">
    <div class="ux-card" style="border-top-color: #fca311;">
        <i class="fa fa-floppy-o" style="color: #fca311;"></i>
        <h3 style="color: #000000 !important;">Memento Pattern</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Catturiamo uno "snapshot" istantaneo di tutte le variabili (risorse, edifici, cittadini) senza violare l'incapsulamento.</p>
    </div>
    <div class="ux-card" style="border-top-color: #fca311;">
        <i class="fa fa-file-code-o" style="color: #fca311;"></i>
        <h3 style="color: #000000 !important;">Formato JSON</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Semplice, leggero e leggibile. Permette di debuggare i salvataggi aprendoli come semplici file di testo.</p>
    </div>
</div>

<div class="file-box" style="border-left-color: #fca311 !important; margin-top: 30px;">
    <div class="file-name" style="background: #fca311 !important; color: #000 !important;">VillagePersistenceService</div>
    <p class="file-desc" style="color: #ffffff !important;">L'orchestratore: gestisce i 5 slot di salvataggio nella cartella utente e coordina l'apertura/chiusura dei file su disco.</p>
</div>

<div class="file-box" style="border-left-color: #fca311 !important;">
    <div class="file-name" style="background: #fca311 !important; color: #000 !important;">VillageMapper</div>
    <p class="file-desc" style="color: #ffffff !important;">Il traduttore: trasforma l'oggetto Java <code>Village</code> in una stringa JSON e viceversa, gestendo anche le versioni del salvataggio.</p>
</div>

<div class="file-box" style="border-left-color: #fca311 !important;">
    <div class="file-name" style="background: #fca311 !important; color: #000 !important;">GamePersistenceManager</div>
    <p class="file-desc" style="color: #ffffff !important;">Il ponte con la UI: permette ai pulsanti "Save" e "Load" del menù di dialogare con il sistema di scrittura senza bloccare il rendering.</p>
</div>