---
title: Daimyo Simulator - Presentazione Progetto
ga: ua-123456-1
mode: slide
theme: white
transition: slide
---

<style>
    
/* FORZATURA SFONDO BIANCO */
.reveal {
    background-color: #ffffff !important;
}
.reveal .slides section {
    background-color: #ffffff !important;
}
/* CSS per rendere le tue slide dinamiche e schematiche su sfondo bianco */
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
    background: rgba(0, 0, 0, 0.05); /* Grigio leggero su bianco */
    border-top: 4px solid #fca311;
    border-bottom: 1px solid #ddd;
    border-left: 1px solid #ddd;
    border-right: 1px solid #ddd;
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
    color: #000 !important; /* Testo nero */
    margin-bottom: 10px;
}
.file-box {
    background: rgba(0, 0, 0, 0.05); /* Sfondo chiaro per i file */
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
    color: #000 !important; /* Testo nero per visibilità */
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
    

/* Stile sezione Architettura & Motore Grafico */
.reveal h2.gfx-title {
    color: #14213d !important;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 40px !important;
    margin-bottom: 6px !important;
}
.gfx-subtitle {
    text-align: center !important;
    color: #555 !important;
    font-size: 22px !important;
    margin: 0 0 24px 0 !important;
}
.gfx-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    margin-top: 18px;
}
.gfx-card {
    background: linear-gradient(180deg, rgba(20,33,61,0.08), rgba(0,0,0,0.03));
    border-top: 4px solid #14213d;
    border-bottom: 1px solid #ddd;
    border-left: 1px solid #ddd;
    border-right: 1px solid #ddd;
    padding: 18px;
    border-radius: 10px;
    text-align: center;
    box-shadow: 0 8px 18px rgba(0,0,0,0.06);
}
.gfx-card i {
    font-size: 38px;
    color: #14213d;
    margin-bottom: 10px;
}
.gfx-card h3 {
    font-size: 24px !important;
    color: #000 !important;
    margin: 6px 0 8px 0 !important;
}
.gfx-card p {
    font-size: 19px !important;
    text-align: center !important;
    color: #000 !important;
    margin: 0 !important;
}
.gfx-code {
    background: #14213d;
    color: #ffffff !important;
    font-family: monospace;
    padding: 3px 8px;
    border-radius: 4px;
    font-size: 18px;
    white-space: nowrap;
}
.gfx-flow {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    margin: 22px 0;
}
.gfx-step {
    background: rgba(0,0,0,0.05);
    border-top: 4px solid #fca311;
    border-radius: 10px;
    padding: 16px 12px;
    width: 170px;
    min-height: 90px;
    text-align: center;
    box-shadow: 0 6px 14px rgba(0,0,0,0.06);
}
.gfx-step i {
    color: #fca311;
    font-size: 30px;
    margin-bottom: 8px;
}
.gfx-step h3 {
    color: #000 !important;
    font-size: 20px !important;
    margin: 0 0 4px 0 !important;
}
.gfx-step p {
    color: #000 !important;
    font-size: 15px !important;
    text-align: center !important;
    margin: 0 !important;
}
.gfx-arrow {
    color: #8c1c13;
    font-size: 28px;
    font-weight: bold;
}
.gfx-file-box {
    background: rgba(0,0,0,0.05);
    border-left: 5px solid #14213d;
    padding: 12px 14px;
    margin-bottom: 12px;
    border-radius: 6px;
    display: flex;
    align-items: center;
    gap: 14px;
}
.gfx-file-name {
    background: #14213d;
    color: white;
    font-family: monospace;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 4px;
    font-size: 18px;
    min-width: 260px;
    text-align: center;
}
.gfx-file-desc {
    color: #000 !important;
    font-size: 19px !important;
    margin: 0 !important;
    text-align: left !important;
}
.gfx-highlight {
    background: rgba(252,163,17,0.13);
    border-left: 6px solid #fca311;
    padding: 14px;
    margin-top: 18px;
    border-radius: 6px;
}
.gfx-highlight p {
    margin: 0 !important;
    font-size: 20px !important;
    text-align: center !important;
    color: #000 !important;
}
.gfx-layer-stack {
    display: grid;
    grid-template-columns: 1fr;
    gap: 8px;
    margin-top: 8px;
}
.gfx-layer {
    background: rgba(20,33,61,0.08);
    border-left: 5px solid #3a86ff;
    padding: 9px 12px;
    border-radius: 5px;
    font-size: 18px;
    color: #000;
    text-align: left;
}

.gfx-mini-note {
    background: rgba(140,28,19,0.06);
    border-left: 6px solid #8c1c13;
    padding: 13px 16px;
    margin-top: 14px;
    border-radius: 6px;
    display: grid;
    grid-template-columns: 230px 1fr;
    gap: 12px;
    align-items: center;
}
.gfx-mini-note .gfx-mini-title {
    color: #8c1c13 !important;
    font-size: 18px !important;
    font-weight: bold;
    text-align: center !important;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin: 0 !important;
}
.gfx-mini-note p {
    margin: 0 !important;
    font-size: 18px !important;
    text-align: left !important;
    color: #000 !important;
}

.reveal h1, .reveal h2, .reveal h3 {
    color: #8c1c13 !important; /* Rosso lacca scuro, più elegante su bianco */
    font-family: 'Playfair Display', serif;
}
.reveal p, .reveal li {
    font-size: 28px !important;
    text-align: justify;
    color: #000 !important; /* Testo corpo nero */
}
.reveal .important-box {
    background: rgba(140, 28, 19, 0.05);
    border-left: 6px solid #8c1c13;
    padding: 15px;
    margin-top: 20px;
    border-radius: 4px;
}
.reveal .todo-box {
    background: rgba(241, 196, 15, 0.1);
    border-left: 6px solid #f1c40f;
    padding: 20px;
    margin-top: 20px;
    border-radius: 4px;
    text-align: left;
}
.reveal .todo-title {
    color: #b8860b !important; /* Oro scuro leggibile su bianco */
    font-weight: bold;
    font-size: 24px;
    margin-bottom: 10px;
    text-transform: uppercase;
}
</style>

# Daimyo Simulator
### Presentazione del Progetto

<br>
<p style="text-align: center !important; font-size: 24px !important; color: #555;">
    <b>Team di Sviluppo:</b><br>
    Antonio Saboanu, Edoardo Perissinotto, Luca Feggi, Mario Pepe
</p>

---

## Il Nostro Workflow
### Linea Temporale dello Sviluppo

<br>

**Settimana 1** (Brainstorming & User Stories) ➔ **Settimane 2-4** (Stesura Codice & Ruoli) ➔ **Settimana 5** (Testing & Consegna)

<br>

<div class="important-box">
<p style="margin: 0 !important; font-size: 22px !important; text-align: center !important; color: #000;">
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
    <img src="https://images.unsplash.com/photo-1528164344705-4754268799af?auto=format&fit=crop&q=80&w=600" alt="Japan Temple" style="border-radius: 8px; border: 2px solid #8c1c13; box-shadow: 0 10px 20px rgba(0,0,0,0.1);">
</div>
</div>

---

## Seconda - Quarta Settimana
### Stesura Codice & Divisione Ruoli

<p>
    La maggior parte del tempo è stata impiegata a scrivere il codice dell'applicazione. Non avendo esperienze pregresse con strumenti grafici in Java (libGDX), la fase di setup iniziale e l'interfaccia grafica sono state assistite dall'IA per muovere rapidamente i primi passi.
</p>

<div class="important-box">
<p style="margin: 0 !important; font-weight: bold; color: #000;">
    Separazione Netta delle Responsabilità:
</p>
<ul style="color: #000;">
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
    <img src="https://images.unsplash.com/photo-1600132806370-bf17e65e942f?auto=format&fit=crop&q=80&w=600" alt="Code Testing" style="border-radius: 8px; border: 2px solid #8c1c13; box-shadow: 0 10px 20px rgba(0,0,0,0.1);">
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

<p style="text-align: center !important; color: #000;">
    L'intera implementazione software di Daimyo Simulator è stata segmentata in tre macro-aree indipendenti e comunicanti:
</p>

<br>
<div style="display: flex; gap: 20px; justify-content: space-between;">
    <div style="background: rgba(0,0,0,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px; border: 1px solid #ddd;">
        <h3 style="color: #388e3c !important;">LOGICA</h3>
        <p style="font-size: 18px !important; text-align: center !important; color: #000;">Motore matematico, tick e risorse.</p>
    </div>
    <div style="background: rgba(0,0,0,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px; border: 1px solid #ddd;">
        <h3 style="color: #1976d2 !important;">MOTORE GRAFICO</h3>
        <p style="font-size: 18px !important; text-align: center !important; color: #000;">Rendering, Texture Atlas e Stage.</p>
    </div>
    <div style="background: rgba(0,0,0,0.05); padding: 20px; flex: 1; text-align: center; border-radius: 4px; border: 1px solid #ddd;">
        <h3 style="color: #c2185b !important;">INTERAZIONE</h3>
        <p style="font-size: 18px !important; text-align: center !important; color: #000;">Input router, comandi e pannelli UI.</p>
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

## Architettura & Motore Grafico
### Dal modello di gioco ai pixel su schermo

<h2 class="gfx-title">Perché libGDX?</h2>
<p class="gfx-subtitle">Non una UI desktop: un simulatore 2D con rendering continuo, asset stratificati e controllo frame-by-frame.</p>

<div class="gfx-grid">
    <div class="gfx-card" style="border-top-color: #3a86ff;">
        <i class="fa fa-refresh" style="color: #3a86ff;"></i>
        <h3>Game Loop Reattivo</h3>
        <p><span class="gfx-code">render(delta)</span> aggiorna la scena a ogni frame, mantenendo fluida la simulazione.</p>
    </div>
    <div class="gfx-card" style="border-top-color: #38b000;">
        <i class="fa fa-picture-o" style="color: #38b000;"></i>
        <h3>SpriteBatch</h3>
        <p>Disegno efficiente di tile, edifici e overlay senza appesantire il motore grafico.</p>
    </div>
    <div class="gfx-card" style="border-top-color: #d90429;">
        <i class="fa fa-video-camera" style="color: #d90429;"></i>
        <h3>Camera Ortografica</h3>
        <p>Pan, zoom controllato e griglia pixel-perfect per una mappa leggibile e stabile.</p>
    </div>
    <div class="gfx-card" style="border-top-color: #9d4edd;">
        <i class="fa fa-object-group" style="color: #9d4edd;"></i>
        <h3>Scene2D per la UI</h3>
        <p><span class="gfx-code">Stage</span> e <span class="gfx-code">Table</span> gestiscono HUD, Build Menu e pannelli senza coordinate manuali.</p>
    </div>
</div>

<div class="gfx-highlight">
    <p><b>Idea chiave:</b> libGDX ci dà controllo da videogioco; Scene2D ci evita di reinventare il layout dell'interfaccia.</p>
</div>

<div class="gfx-mini-note">
    <p class="gfx-mini-title">Perché non JavaFX o Swing?</p>
    <p>Sono ottimi per applicazioni a widget, ma meno adatti a un gioco 2D: non offrono nativamente game loop, batching sprite e pipeline OpenGL pensata per rendering continuo a 60 FPS.</p>
</div>

---

## Architettura & Motore Grafico
### Pipeline asset e rendering della mappa

<h2 class="gfx-title">Dall'asset PNG alla scena 2D</h2>
<p class="gfx-subtitle">Una pipeline semplice da spiegare: carichiamo, traduciamo, ordiniamo e disegniamo.</p>

<div class="gfx-flow">
    <div class="gfx-step">
        <i class="fa fa-file-image-o"></i>
        <h3>PNG</h3>
        <p>Tile, edifici, icone e feature.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step">
        <i class="fa fa-database"></i>
        <h3>Registry</h3>
        <p>Chiavi asset e fallback.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step">
        <i class="fa fa-th-large"></i>
        <h3>Render Model</h3>
        <p>Ogni cella diventa disegnabile.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step">
        <i class="fa fa-magic"></i>
        <h3>WorldRenderer</h3>
        <p>Disegno stratificato.</p>
    </div>
</div>

<div class="gfx-grid">
    <div>
        <div class="gfx-file-box" style="border-left-color: #3a86ff;">
            <div class="gfx-file-name" style="background: #3a86ff;">SpriteSheetRegionRegistry</div>
            <p class="gfx-file-desc">Carica i PNG come <span class="gfx-code">TextureRegion</span> e applica <span class="gfx-code">Nearest</span> per mantenere la pixel art nitida.</p>
        </div>
        <div class="gfx-file-box" style="border-left-color: #38b000;">
            <div class="gfx-file-name" style="background: #38b000;">GameAssetManager</div>
            <p class="gfx-file-desc">Espone gli asset al resto del gioco e gestisce il <span class="gfx-code">missing_asset</span> senza bloccare la partita.</p>
        </div>
    </div>
    <div class="gfx-card" style="border-top-color: #fca311; text-align: left;">
        <h3 style="text-align: center;">Ordine di rendering</h3>
        <div class="gfx-layer-stack">
            <div class="gfx-layer">1. Terreno base</div>
            <div class="gfx-layer" style="border-left-color:#38b000;">2. Bordi di foresta</div>
            <div class="gfx-layer" style="border-left-color:#fca311;">3. Feature naturali</div>
            <div class="gfx-layer" style="border-left-color:#d90429;">4. Edifici e anteprima costruzione</div>
            <div class="gfx-layer" style="border-left-color:#9d4edd;">5. Animazioni e griglia di selezione</div>
        </div>
    </div>
</div>

---

## Architettura & Motore Grafico
### Disaccoppiamento tra logica e rendering

<h2 class="gfx-title">Contratto stabile: Snapshot ➔ Adapter ➔ Renderer</h2>
<p class="gfx-subtitle">La logica calcola il villaggio; la grafica riceve solo ciò che deve disegnare.</p>

<div class="gfx-flow">
    <div class="gfx-step" style="border-top-color:#8c1c13;">
        <i class="fa fa-cogs" style="color:#8c1c13;"></i>
        <h3>Core Logic</h3>
        <p>Regole, risorse e tick.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step" style="border-top-color:#fca311;">
        <i class="fa fa-camera-retro" style="color:#fca311;"></i>
        <h3>VillageSnapshot</h3>
        <p>Fotografia immutabile.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step" style="border-top-color:#3a86ff;">
        <i class="fa fa-exchange" style="color:#3a86ff;"></i>
        <h3>Adapter</h3>
        <p>Traduce dominio in grafica.</p>
    </div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step" style="border-top-color:#38b000;">
        <i class="fa fa-desktop" style="color:#38b000;"></i>
        <h3>WorldRenderer</h3>
        <p>Disegna senza modificare il modello.</p>
    </div>
</div>

<div class="gfx-grid">
    <div class="gfx-card" style="border-top-color: #14213d;">
        <i class="fa fa-code-fork"></i>
        <h3>Team in parallelo</h3>
        <p>Core logic e grafica comunicano tramite snapshot: meno dipendenze, meno conflitti, sviluppo più ordinato.</p>
    </div>
    <div class="gfx-card" style="border-top-color: #fca311;">
        <i class="fa fa-shield" style="color: #fca311;"></i>
        <h3>Renderer sicuro</h3>
        <p>Il renderer non conosce le regole di gioco: legge dati pronti e li trasforma in immagini.</p>
    </div>
</div>

<div class="gfx-file-box" style="border-left-color: #9d4edd; margin-top: 22px;">
    <div class="gfx-file-name" style="background: #9d4edd;">BuildingSpriteRegistry / TileSpriteRegistry</div>
    <p class="gfx-file-desc">Centralizzano la mappa <b>entità ➔ immagine</b>, così cambiare un asset non richiede modifiche alla logica.</p>
</div>
---

# Interazione Utente & UI Layout


<h2 class="ux-title">Cos'è la UX nel nostro simulatore?</h2>

<div class="ux-grid">
    <div class="ux-card" style="border-top-color: #3a86ff;">
        <i class="fa fa-mouse-pointer" style="color: #3a86ff;"></i>
        <h3 style="color: #000000 !important;">Interazione Fluida</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Select & Drag, navigazione mappa (Pan/Zoom) e interazione coerente coi bottoni senza conflitti.</p>
    </div>
    <div class="ux-card" style="border-top-color: #38b000;">
        <i class="fa fa-eye" style="color: #38b000;"></i>
        <h3 style="color: #000000 !important;">Visibilità Contestuale</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">HUD organizzato a cornice. I menù e i dettagli (es. Market) appaiono solo quando selezioni una struttura.</p>
    </div>
    <div class="ux-card" style="border-top-color: #d90429;">
        <i class="fa fa-bell" style="color: #d90429;"></i>
        <h3 style="color: #000000 !important;">Alert Significativi</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Pop-up cromatici (verde/rosso) e First-Time Warnings per educare il giocatore senza fare spam.</p>
    </div>
    <div class="ux-card" style="border-top-color: #9d4edd;">
        <i class="fa fa-sliders" style="color: #9d4edd;"></i>
        <h3 style="color: #000000 !important;">Controllo Utente</h3>
        <p style="text-align: center; font-size: 20px !important; color: #000000 !important;">Menù Impostazioni facilmente accessibile, controllo velocità logica e opzioni di salvataggio veloci.</p>
    </div>
</div>

---

<h2 class="ux-title">I File dell'Interazione</h2>

<div class="file-box border-blue">
    <div class="file-name bg-blue">GameInputProcessor</div>
    <p class="file-desc" style="color: #000000 !important;">Ascolta i click "grezzi". Ignora le azioni fuori dalla griglia e impedisce conflitti se l'utente sta cliccando sull'HUD.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">CameraController</div>
    <p class="file-desc" style="color: #000000 !important;">Gestisce l'esplorazione: permette il "Select and Drag", il pan (WASD) e blocca lo zoom per non rompere la prospettiva.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">BuildModeState</div>
    <p class="file-desc" style="color: #000000 !important;">La memoria a breve termine della UX: ricorda se stai solo esplorando, se hai in mano un edificio o il martello da demolizione.</p>
</div>

<div class="file-box border-blue">
    <div class="file-name bg-blue">InputCommandRouter</div>
    <p class="file-desc" style="color: #000000 !important;">Lo "smistatore". Prende il click convertito e decide: ispeziono la cella? Piazzo l'edificio? O cancello tutto?</p>
</div>

---

<h2 class="ux-title">I File dell'Interfaccia</h2>

<div class="file-box border-green">
    <div class="file-name bg-green">DashboardHud</div>
    <p class="file-desc" style="color: #000000 !important;">La cornice madre. Racchiude BuildMenu, Risorse e parametri ai bordi, lasciando il centro dello schermo libero per giocare.</p>
</div>

<div class="file-box border-red">
    <div class="file-name bg-red">WarningPanel & EventModal</div>
    <p class="file-desc" style="color: #000000 !important;">Gestiscono i First-Time Warnings (es. quando finisce il cibo) e mostrano gli eventi casuali sfruttando la psicologia dei colori.</p>
</div>

<div class="file-box border-green">
    <div class="file-name bg-green">SelectedBuildingPanel</div>
    <p class="file-desc" style="color: #000000 !important;">UX contestuale: appare in basso solo quando ispezioni un edificio. Nasconde la complessità finché non la richiedi (es. tasto Trade).</p>
</div>

<div class="file-box border-green">
    <div class="file-name bg-green">SettingsModal / Dialogs</div>
    <p class="file-desc" style="color: #000000 !important;">Modali in sovraimpressione per mettere in pausa e dare controllo su Salvataggi, Tutorial e regolazione Audio asincrona.</p>
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
    <p class="file-desc" style="color: #000000 !important;">L'orchestratore: gestisce i 5 slot di salvataggio nella cartella utente e coordina l'apertura/chiusura dei file su disco.</p>
</div>

<div class="file-box" style="border-left-color: #fca311 !important;">
    <div class="file-name" style="background: #fca311 !important; color: #000 !important;">VillageMapper</div>
    <p class="file-desc" style="color: #000000 !important;">Il traduttore: trasforma l'oggetto Java <code>Village</code> in una stringa JSON e viceversa, gestendo anche le versioni del salvataggio.</p>
</div>

<div class="file-box" style="border-left-color: #fca311 !important;">
    <div class="file-name" style="background: #fca311 !important; color: #000 !important;">GamePersistenceManager</div>
    <p class="file-desc" style="color: #000000 !important;">Il ponte con la UI: permette ai pulsanti "Save" e "Load" del menù di dialogare con il sistema di scrittura senza bloccare il rendering.</p>
</div>