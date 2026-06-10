---
title: Daimyo Simulator - Presentazione Progetto
ga: ua-123456-1
mode: slide
theme: white
transition: slide
---

<style>
/* --- DESIGN SYSTEM: JAPAN LACQUER & GOLD --- */

.reveal { background-color: #ffffff !important; }
.reveal .slides section { background-color: #ffffff !important; }

/* Tipografia */
.reveal h1, .reveal h2, .reveal h3 {
    color: #8C1C13 !important; /* Rosso Lacca */
    font-family: 'Playfair Display', serif;
    text-transform: none !important;
}

/* Titoli di sezione con sottolineatura */
.reveal h2.ux-title, .reveal h2.gfx-title {
    font-size: 36px !important;
    border-bottom: 2px solid #D4AF37 !important; /* Oro */
    display: inline-block;
    padding-bottom: 5px;
    margin-bottom: 20px !important;
}

/* Card e Griglie */
.ux-grid, .gfx-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
}

.ux-card, .gfx-card, .gfx-step {
    background: #fdfcf0 !important; /* Pergamena */
    border: 1px solid #d4af37 !important;
    border-top: 4px solid #8C1C13 !important;
    padding: 15px !important;
    border-radius: 4px !important;
    text-align: center;
}

.ux-card i, .gfx-card i, .gfx-step i {
    font-size: 30px !important;
    color: #8C1C13 !important;
    margin-bottom: 10px;
}

.ux-card h3, .gfx-card h3 {
    font-size: 20px !important;
    color: #000 !important;
    margin: 5px 0 !important;
}

.ux-card p, .gfx-card p {
    font-size: 16px !important;
    line-height: 1.3 !important;
    color: #2d2d2d !important;
}

/* File Box (Liste schematiche) */
.file-box, .gfx-file-box {
    background: rgba(140, 28, 19, 0.03) !important;
    border-left: 5px solid #8C1C13 !important;
    padding: 8px 15px !important;
    margin-bottom: 8px !important;
    display: flex;
    align-items: center;
    gap: 15px;
}

.file-name, .gfx-file-name {
    background: #8C1C13 !important;
    color: #ffffff !important;
    font-family: monospace;
    font-weight: bold;
    padding: 4px 10px;
    border-radius: 2px;
    font-size: 16px;
    min-width: 250px;
    text-align: center;
}

.file-desc, .gfx-file-desc {
    color: #000 !important;
    font-size: 17px !important;
    margin: 0 !important;
    text-align: left;
}

/* Box Importanti e Todo */
.important-box, .gfx-highlight, .reveal .todo-box {
    background: #fdfcf0 !important;
    border-left: 6px solid #D4AF37 !important;
    padding: 15px !important;
    margin-top: 15px;
    text-align: left;
}

/* Flow e Frecce */
.gfx-flow { display: flex; align-items: center; justify-content: center; gap: 10px; margin: 15px 0; }
.gfx-arrow { color: #8C1C13; font-weight: bold; font-size: 24px; }

.gfx-code {
    background: #2d2d2d;
    color: #D4AF37 !important;
    padding: 2px 6px;
    border-radius: 4px;
    font-family: monospace;
}

.gfx-layer {
    background: rgba(0,0,0,0.02);
    border-left: 4px solid #8C1C13;
    padding: 6px 12px !important;
    margin-bottom: 5px;
    font-size: 16px !important;
    text-align: left;
}
    
.important-box p, 
.gfx-highlight p {
    color: #2D2D2D !important;
    font-size: 18px !important;
    line-height: 1.3 !important;
}

.reveal .ux-card li, 
.reveal .gfx-card li,
.reveal .important-box li {
    color: #2D2D2D !important;
    font-size: 18px !important;
    line-height: 1.3 !important;
    margin-bottom: 10px !important;
}
    
.gfx-step h3 {
    color: #2D2D2D !important;
    font-size: 18px !important;
    margin: 5px 0 !important;
}

.gfx-step p {
    color: #2D2D2D !important;
    font-size: 15px !important;
    line-height: 1.2 !important;
}

.gfx-layer {
    color: #2D2D2D !important;
    font-size: 16px !important;
}
    /* Fix per la nota "vs Swing/JavaFX" nella slide libGDX */
.gfx-mini-note p {
    color: #2D2D2D !important;
    font-size: 17px !important;
    line-height: 1.3 !important;
    text-align: left !important;
    margin: 0 !important;
}

.gfx-mini-note .gfx-mini-title {
    color: #8C1C13 !important;
    font-size: 18px !important;
    font-weight: bold !important;
    text-transform: uppercase !important;
    letter-spacing: 1px !important;
    text-align: center !important;
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

## Introduzione
### Il nostro villaggio

<div style="text-align: center;">
<img src="https://hackmd.io/_uploads/BJ1038DbGe.png" style="border: 4px solid #8C1C13; border-radius: 4px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); max-width: 80%;">
</div>

---

## Il Nostro Workflow
### Linea Temporale dello Sviluppo

<p style="text-align: center; font-size: 22px; color: #8C1C13; margin-top: 50px;">
    Dall'analisi dei requisiti alla sottomissione finale attraverso Sprint Agile.
</p>

---

<h2 class="ux-title">Fase Iniziale: Requisiti e Core Logic (W1-W2)</h2>

<div class="ux-grid">
    <div class="ux-card">
        <i class="fa fa-pencil-square-o"></i>
        <h3>Week 1: Analisi Concettuale</h3>
        <p style="text-align: left !important;">
            <b>Elicitazione:</b> Brainstorming per tradurre la consegna in specifiche atomiche.<br>
            <b>Product Backlog:</b> User Stories (Chi/Cosa/Perché) raffinate secondo criteri <b>INVEST</b>.<br>
            <b>Design Model:</b> Blueprint architetturale tramite UML Use Case e Logical View.
        </p>
    </div>
    <div class="ux-card">
        <i class="fa fa-cogs"></i>
        <h3>Week 2: Sprint 1 - Core Logic</h3>
        <p style="text-align: left !important;">
            <b>Sprint Goal:</b> Sviluppo rapido della logica di base per garantire copertura funzionale.<br>
            <b>Pair Programming:</b> Pratica <b>Extreme Programming</b> per condivisione della conoscenza.<br>
            <b>Milestone:</b> Rilascio del primo Incremento (Minimum Viable Product).
        </p>
    </div>
</div>

---

<h2 class="ux-title">Fase Centrale: Evoluzione e Testing (W3-W4)</h2>

<div class="important-box">
    <h3 style="margin:0">Week 3 & 4: Sprint 2 – Evoluzione</h3>
    <p><b>Features:</b> Integrazione nuove funzionalità | <b>Bug Fixing:</b> Sanamento criticità emesse.<br>
    <b>Daily Scrum:</b> Stand-up meeting quotidiani (15 min) per coordinamento costante.</p>
</div>

<div class="ux-grid" style="margin-top:15px">
    <div class="ux-card" style="border-top-color: #d90429 !important;">
        <i class="fa fa-flask" style="color: #d90429 !important;"></i>
        <h3>Development Testing</h3>
        <p>Unit & Component Testing automatizzati (Setup-Call-Assertion) sui singoli oggetti.</p>
    </div>
    <div class="ux-card" style="border-top-color: #d90429 !important;">
        <i class="fa fa-shield" style="color: #d90429 !important;"></i>
        <h3>System & User Testing</h3>
        <p>Test Black-Box su scenari reali e Alpha Testing con utenti esterni per criticità lato utente.</p>
    </div>
</div>

---

<h2 class="ux-title">Fase Conclusiva: Deploy e Sottomissione (W5)</h2>

<div style="display: block; width: 100%;">
    <div class="file-box">
        <div class="file-name">Final Polish</div>
        <p class="file-desc">Ispezione statica del codice e validazione formale rispetto agli Acceptance Criteria.</p>
    </div>
    <div class="file-box">
        <div class="file-name">Host-Target Deploy</div>
        <p class="file-desc">Risoluzione compatibilità tra ambiente di sviluppo (Host) e di esecuzione (Target).</p>
    </div>
    <div class="file-box">
        <div class="file-name">Packaging</div>
        <p class="file-desc">Generazione eseguibili, documentazione tecnica e stesura del file README.</p>
    </div>
</div>

<div class="important-box" style="text-align: center; border-left: none; border-bottom: 4px solid #8C1C13;">
    <h3 style="margin: 0 !important;">Sottomissione Finale: Deliverable completati</h3>
</div>

---

<h2 class="ux-title">User Stories & Jira: Gli Epic</h2>

<div class="ux-grid">
    <div class="ux-card">
        <i class="fa fa-list-ol"></i>
        <h3>6 Epic Funzionali</h3>
        <p>Suddivisione delle macro-aree del simulatore (Core Logic, Grafica, Interazione, Persistenza) per mappare lo sviluppo in blocchi atomici.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-lightbulb-o"></i>
        <h3>16 User Stories</h3>
        <p>Elicitate e raffinate tramite LLM per validare le idee iniziali, consolidando i requisiti in base ai criteri INVEST.</p>
    </div>
</div>

---

<h2 class="ux-title">Anatomia di una User Story</h2>

<div style="display: grid; grid-template-columns: 1.2fr 0.8fr; gap: 20px; align-items: center;">
    <div>
        <div class="file-box"><div class="file-name" style="min-width:180px">Descrizione</div><p class="file-desc">Definizione pattern: Chi, Cosa, Perché.</p></div>
        <div class="file-box"><div class="file-name" style="min-width:180px">Acceptance Criteria</div><p class="file-desc">Vincoli per Definition of Done.</p></div>
        <div class="file-box"><div class="file-name" style="min-width:180px">Note Tecniche</div><p class="file-desc">Riferimenti a classi e JUnit test.</p></div>
    </div>
    <div style="text-align: center;">
        <img src="https://hackmd.io/_uploads/rJClpGwWGl.png" style="border: 2px solid #8C1C13; border-radius: 8px; max-height: 250px;">
    </div>
</div>

---

<h2 class="ux-title">Gestione Agile in Jira</h2>

<div class="important-box" style="border-left-color: #8C1C13 !important;">
    <h3><i class="fa fa-folder-open-o"></i> Tracciamento Gerarchico</h3>
    <p>Tutte le User Stories sono state organizzate nel Backlog di Jira, garantendo trasparenza sui carichi di lavoro del team.</p>
</div>

<div class="important-box" style="margin-top: 20px;">
    <h3><i class="fa fa-refresh"></i> Raffinamento Continuo</h3>
    <p>Seguendo un approccio empirico, AC e note sono stati aggiornati progressivamente a seguito dei Daily Scrum e dei test di usabilità.</p>
</div>

---

## Stesura del Codice
### La Struttura dell'Applicazione

<div style="display: flex; gap: 20px; justify-content: space-between; margin-top: 40px;">
    <div class="ux-card" style="flex: 1;">
        <h3 style="color:#8C1C13 !important">LOGICA</h3>
        <p>Motore matematico, tick e risorse.</p>
    </div>
    <div class="ux-card" style="flex: 1;">
        <h3 style="color:#8C1C13 !important">MOTORE GRAFICO</h3>
        <p>Rendering, Texture Atlas e Stage.</p>
    </div>
    <div class="ux-card" style="flex: 1;">
        <h3 style="color:#8C1C13 !important">INTERAZIONE</h3>
        <p>Input router, comandi e pannelli UI.</p>
    </div>
</div>

---

<h2 class="gfx-title">Logica del gioco: Backend</h2>

<div class="gfx-grid">
    <div class="gfx-card">
        <i class="fa fa-sitemap"></i>
        <h3>Servizi Specializzati</h3>
        <p>Separazione responsabilità: <span class="gfx-code">HousingService</span>, <span class="gfx-code">TradeService</span>, <span class="gfx-code">ConstructionService</span>.</p>
    </div>
    <div class="gfx-card">
        <i class="fa fa-gamepad"></i>
        <h3>Orchestrazione</h3>
        <p>Il <span class="gfx-code">GameController</span> funge da punto d'accesso principale per le richieste della UI.</p>
    </div>
    <div class="gfx-card">
        <i class="fa fa-clock-o"></i>
        <h3>Motore Tick-Based</h3>
        <p>Il <span class="gfx-code">SimulationEngine</span> mantiene coerenza temporale ed economica.</p>
    </div>
    <div class="gfx-card">
        <i class="fa fa-shield"></i>
        <h3>Dominio Sicuro</h3>
        <p>Backend isolato: comunica con la UI tramite proiezioni immutabili (<span class="gfx-code">Snapshot</span>).</p>
    </div>
</div>

---

<h2 class="gfx-title">TickProcessor</h2>
<p style="text-align: center; margin-bottom: 10px;">Classe centrale che ricalcola lo stato ad ogni turno.</p>

<div class="gfx-flow">
    <div class="gfx-step"><i class="fa fa-gavel"></i><h3>1. Policy</h3><p>Regole villaggio</p></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-users"></i><h3>2. Lavoro</h3><p>Job Assignment</p></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-balance-scale"></i><h3>3. Economia</h3><p>Produzione</p></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-heartbeat"></i><h3>4. Felicità</h3><p>Parametri</p></div>
</div>

<div class="gfx-highlight">
    <p><b>Output:</b> Genera un <span class="gfx-code">TickResult</span> (storico eventi e carenze, es. diserzione samurai).</p>
</div>

---

<h2 class="gfx-title">Gestione degli Edifici</h2>

<div class="ux-grid">
    <div class="ux-card">
        <i class="fa fa-building-o"></i>
        <h3>Gerarchia Edifici</h3>
        <p>Tutti gli edifici estendono <span class="gfx-code">AbstractBuilding</span>: costi legname, residenti e slot lavoro standardizzati.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-map-marker"></i>
        <h3>Posizionamento</h3>
        <p>Regole stringenti: piazzamento possibile solo se i requisiti ambientali sono soddisfatti (es. vicinanza foreste).</p>
    </div>
</div>

---

<h2 class="gfx-title">Gestione delle Risorse</h2>

<div class="important-box">
    <i class="fa fa-balance-scale" style="color:#8C1C13; font-size: 24px;"></i>
    <ul style="margin:0; padding-left: 20px;">
        <li><b>Costi Scalabili:</b> Incremento continuo del costo degli edifici all'aumentare delle unità.</li>
        <li><b>Feedback Punitivi:</b> Carenze prolungate impattano i parametri (abbandono dei cittadini).</li>
    </ul>
</div>

---

<h2 class="gfx-title">Design Patterns Utilizzati</h2>

<div class="file-box">
    <div class="file-name">Facade Pattern</div>
    <p class="file-desc"><span class="gfx-code">GameController</span> nasconde la complessità dei servizi interni.</p>
</div>
<div class="file-box">
    <div class="file-name">Factory Pattern</div>
    <p class="file-desc"><span class="gfx-code">BuildingFactory</span> centralizza e astrae la creazione di strutture.</p>
</div>
<div class="file-box">
    <div class="file-name">Composite Pattern</div>
    <p class="file-desc"><span class="gfx-code">CompositePlacementValidator</span> unisce dinamicamente molteplici regole.</p>
</div>

---

<h2 class="gfx-title">Motore Grafico: Perché libGDX?</h2>

<div class="gfx-grid">
    <div class="gfx-card">
        <i class="fa fa-refresh"></i>
        <h3>Game Loop</h3>
        <p><span class="gfx-code">render(delta)</span> aggiorna e disegna a 60 FPS per una fluidità totale.</p>
    </div>
    <div class="gfx-card">
        <i class="fa fa-picture-o"></i>
        <h3>SpriteBatch</h3>
        <p>Disegno efficiente di migliaia di tile e asset senza sovraccaricare la GPU.</p>
    </div>
</div>

<div class="gfx-mini-note">
    <p class="gfx-mini-title">vs Swing/JavaFX</p>
    <p>libGDX offre controllo diretto su OpenGL, batching nativo e pipeline specifiche per il rendering 2D continuo.</p>
</div>

---

<h2 class="gfx-title">Pipeline Asset</h2>

<div class="gfx-flow">
    <div class="gfx-step"><i class="fa fa-file-image-o"></i><h3>PNG</h3></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-database"></i><h3>Registry</h3></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-th-large"></i><h3>Model</h3></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><i class="fa fa-magic"></i><h3>Renderer</h3></div>
</div>

<div class="file-box">
    <div class="file-name">GameAssetManager</div>
    <p class="file-desc">Gestisce il <span class="gfx-code">missing_asset</span> evitando crash se manca una texture.</p>
</div>

---

<h2 class="gfx-title">Rendering della Mappa</h2>

<div class="gfx-grid">
    <div class="gfx-card" style="text-align: left;">
        <h3 style="text-align:center">Livelli di Disegno</h3>
        <div class="gfx-layer">1. Terreno base</div>
        <div class="gfx-layer">2. Bordi di foresta</div>
        <div class="gfx-layer">3. Feature naturali</div>
        <div class="gfx-layer">4. Edifici e anteprime</div>
        <div class="gfx-layer">5. Animazioni e griglia</div>
    </div>
    <div class="gfx-card">
        <i class="fa fa-video-camera"></i>
        <h3>OrthographicCamera</h3>
        <p>Gestisce pan, zoom pixel-perfect e stabilità visiva del feudo.</p>
    </div>
</div>

---

<h2 class="gfx-title">Disaccoppiamento</h2>

<div class="gfx-flow">
    <div class="gfx-step"><h3>Logica</h3><p>Calcolo regole</p></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><h3>Snapshot</h3><p>Dati immutabili</p></div>
    <div class="gfx-arrow">➔</div>
    <div class="gfx-step"><h3>Renderer</h3><p>Disegno puro</p></div>
</div>

<div class="gfx-highlight">
    <p>Logica e Grafica lavorano in parallelo su un contratto stabile: il renderer non modifica mai il modello di gioco.</p>
</div>

---

<h2 class="ux-title">Cos'è la UX nel simulatore?</h2>

<div class="ux-grid">
    <div class="ux-card">
        <i class="fa fa-mouse-pointer"></i>
        <h3>Interazione Fluida</h3>
        <p>Select & Drag, navigazione mappa (Pan/Zoom) e bottoni coerenti senza conflitti di input.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-eye"></i>
        <h3>Visibilità Contestuale</h3>
        <p>HUD a cornice. Pannelli e dettagli (es. Market) appaiono solo se richiesti dalla selezione.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-bell"></i>
        <h3>Alert Significativi</h3>
        <p>Pop-up cromatici (verde/rosso) e First-Time Warnings per educare senza fare spam.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-sliders"></i>
        <h3>Controllo Utente</h3>
        <p>Menù impostazioni accessibile, controllo velocità logica e slot di salvataggio rapidi.</p>
    </div>
</div>

---

<h2 class="ux-title">I File dell'Interazione</h2>

<div class="file-box">
    <div class="file-name">GameInputProcessor</div>
    <p class="file-desc">Filtra click e movimenti. Ignora azioni fuori griglia e priorità all'HUD.</p>
</div>
<div class="file-box">
    <div class="file-name">CameraController</div>
    <p class="file-desc">Gestisce l'esplorazione (WASD/Frecce) e blocca lo zoom per la prospettiva.</p>
</div>
<div class="file-box">
    <div class="file-name">BuildModeState</div>
    <p class="file-desc">Ricorda se l'utente sta esplorando, piazzando edifici o demolendo.</p>
</div>
<div class="file-box">
    <div class="file-name">InputCommandRouter</div>
    <p class="file-desc">Lo "smistatore": traduce il click in ispezione cella o azione di costruzione.</p>
</div>

---

<h2 class="ux-title">I File dell'Interfaccia</h2>

<div class="file-box">
    <div class="file-name">DashboardHud</div>
    <p class="file-desc">Cornice madre: racchiude BuildMenu, Risorse e parametri ai bordi dello schermo.</p>
</div>
<div class="file-box">
    <div class="file-name">WarningPanel & Modal</div>
    <p class="file-desc">Gestiscono i First-Time Warnings e mostrano eventi casuali con psicologia dei colori.</p>
</div>
<div class="file-box">
    <div class="file-name">SelectedBuildingPanel</div>
    <p class="file-desc">UX contestuale: appare in basso solo quando ispezioni un edificio specifico.</p>
</div>

---

<h2 class="ux-title">Persistenza: JSON & Memento</h2>

<div class="ux-grid">
    <div class="ux-card">
        <i class="fa fa-floppy-o"></i>
        <h3>Memento Pattern</h3>
        <p>Catturiamo uno "snapshot" di risorse, edifici e cittadini senza violare l'incapsulamento.</p>
    </div>
    <div class="ux-card">
        <i class="fa fa-file-code-o"></i>
        <h3>Formato JSON</h3>
        <p>Leggero e leggibile. Permette di debuggare i salvataggi come semplici file di testo.</p>
    </div>
</div>

<div class="file-box" style="margin-top:20px">
    <div class="file-name">VillagePersistenceService</div>
    <p class="file-desc">Gestisce i 5 slot di salvataggio nella cartella utente (<span class="gfx-code">.daimyosimulator</span>).</p>
</div>