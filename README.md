---
title: Daimyo Simulator - Presentazione Progetto
ga: ua-123456-1
mode: slide
theme: night
transition: slide
---

<style>
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
### Implementazione con libGDX e Gestione Asset

<div class="todo-box">
    <div class="todo-title">SLIDE DA COMPLETARE — REQUISITO PER: LUCA FEGGI & ANTONIO SABOANU</div>
    <p><b>Indicazioni per lo sviluppo della slide:</b></p>
    <ul>
        <li>Spiegare l'integrazione con il framework <b>libGDX</b> e l'uso dei componenti Scene2D (Stage, Table, Actors).</li>
        <li>Illustrare il sistema di caricamento e renderizzazione delle <b>Textures</b> e degli <b>Sprites 2D</b> della mappa di gioco.</li>
        <li><b>Focus Tecnico (Luca & Antonio):</b> Analizzare nel dettaglio il problema riscontrato con gli sfondi bianchi degli asset grafici e spiegare la soluzione adottata per ripulire i canali alpha o ottimizzare i file sorgente.</li>
    </ul>
</div>

---

## Interazione Utente & UI Layout
### Gestione degli Input e Flusso dei Comandi

<div class="todo-box">
    <div class="todo-title">SLIDE DA COMPLETARE — REQUISITO PER: ANTONIO SABOANU</div>
    <p><b>Indicazioni per lo sviluppo della slide:</b></p>
    <ul>
        <li>Spiegare l'architettura dell'interfaccia utente in-game (HUD delle risorse, Build Menu strutturato a colonne, Market dinamico).</li>
        <li>Approfondire il funzionamento del sistema dei comandi (es. InputInputCommandRouter) per passare le azioni del mouse (costruzione, demolizione) dalla UI alla logica senza generare accoppiamento stretto.</li>
        <li>Mostrare la gestione del pannello delle impostazioni (regolazione dei volumi audio asincrona) e l'integrazione del sistema di alert bicromatico (verde/rosso).</li>
    </ul>
</div>