# Offline Data Analysis On Browser

Un'app web offline (unico file html) per analizzare file CSV/Excel/JSON nel browser con SQL. Visualizza dati in tabelle e grafici interattivi, modifica ed esporta in sicurezza. Nessun dato lascia il tuo computer. Supporto multilingua e temi chiaro/scuro.

<img width="953" height="468" alt="image" src="https://github.com/user-attachments/assets/40f8a365-d9aa-4eb3-ba9b-11b1abdcdd0d" />


----

**Data Analysis** è un'applicazione web potente e completamente offline per l'analisi dei dati. Permette di caricare file CSV, Excel e JSON, importarli in un database SQLite eseguito direttamente nel browser (tramite WebAssembly) e interrogare i dati utilizzando un editor SQL avanzato. I risultati possono essere visualizzati in tabelle interattive, trasformati in grafici e esportati in vari formati.

Tutta l'elaborazione avviene localmente nel tuo browser, garantendo che i tuoi dati rimangano privati e sicuri al 100%.


## **✨ Funzionalità Principali**

Questa applicazione è dotata di un set completo di strumenti per l'analisi dei dati:

#### **📂 Caricamento Dati Flessibile**

* **Multi-formato:** Carica file .csv, .xlsx, .xls e .json.  
* **Parser CSV Intelligente:** Rileva automaticamente il delimitatore (virgola, punto e virgola, ecc.) e determina se la prima riga è un'intestazione, gestendo anche nomi di colonna duplicati.  
* **Supporto Multi-file:** Carica più file contemporaneamente; ognuno verrà convertito in una tabella separata nel database.

#### **🚀 Database In-Browser (SQLite-WASM)**

* **100% Offline:** Dopo il primo caricamento, l'applicazione funziona interamente senza connessione a Internet.  
* **Privacy Garantita:** Nessun dato viene inviato a server esterni. Tutto rimane all'interno del tuo browser.  
* **Import/Export del Database:** Salva l'intera sessione di lavoro (tutte le tabelle) in un file .db e ricaricala in un secondo momento.

#### **✍️ Editor SQL Avanzato**

* **Potente e Intuitivo:** Basato su Monaco Editor (il motore di VS Code).  
* **Autocompletamento Intelligente:** Ricevi suggerimenti per parole chiave SQL, funzioni di SQLite e, soprattutto, per i **nomi delle colonne** quando digiti l'alias di una tabella seguito da un punto (es. alias.).  
* **Esecuzione Rapida:** Esegui le query con CTRL+ENTER o F9.  
* **Esecuzione Selettiva:** Esegui solo la query in cui si trova il cursore (se separate da ;) o solo il testo che hai selezionato.

#### **📊 Visualizzazione Dati Interattiva**

* **Tabella Avanzata:** I risultati sono mostrati in una tabella basata su Tabulator, con:  
  * Paginazione.  
  * Ordinamento per colonna.  
  * Filtri per colonna.  
  * **Modifica inline** dei dati (facendo doppio clic su una cella).  
  * **Ricerca locale** per filtrare istantaneamente i risultati della query.  
* **Modulo Grafici Integrato:**  
  * Passa dalla visualizzazione tabellare a quella grafica con un clic.  
  * Crea grafici a **barre, linee, torta e scatter** selezionando le colonne per gli assi X e Y.  
  * Esporta qualsiasi grafico come immagine .png.

#### **🎨 Interfaccia Utente Personalizzabile**

* **Tema Chiaro e Scuro:** Scegli il tema che preferisci per un comfort visivo ottimale.  
* **Layout Flessibile:** I pannelli (Schema DB, Editor SQL, Risultati) sono ridimensionabili per adattarsi al tuo flusso di lavoro.  
* **Sidebar Richiudibile:** Massimizza lo spazio di lavoro nascondendo la sidebar.  
* **Supporto Multilingua:** L'interfaccia è disponibile in Italiano, Inglese, Albanese, Francese, Tedesco e Cinese.

#### **📚 Risorse Utili**

* **Schema Explorer:** Visualizza tutte le tabelle caricate, le loro colonne e i tipi di dato. Clicca su tabelle e colonne per generare query automaticamente.  
* **Cheatsheet SQL Completo:** Un pratico riferimento rapido per comandi e funzioni SQLite, accessibile direttamente dall'editor.

## **🚀 Come Usarlo**

L'applicazione è progettata per essere il più semplice possibile da usare:

1. **Download:** Scarica il file dashboard\_analisi\_dati.html.  
2. **Apertura:** Apri il file con un browser web moderno (Chrome, Firefox, Edge, Safari).  
3. **Caricamento:**  
   * Clicca su **"Carica File"** per importare i tuoi file di dati (CSV, Excel, JSON).  
   * In alternativa, clicca su **"Importa"** per caricare un database .db salvato in una sessione precedente.  
4. **Analisi:**  
   * Usa lo **Schema DB** sulla sinistra per esplorare le tabelle.  
   * Scrivi le tue query nell'**Editor SQL**.  
   * Premi **CTRL+ENTER** o il pulsante **"Esegui"**.  
5. **Visualizzazione:**  
   * Esplora i dati nella **Tabella** interattiva.  
   * Passa alla tab **"Grafico"**, seleziona il tipo e le colonne, e clicca **"Genera"**.  
6. **Esportazione:**  
   * Esporta i risultati della tabella in CSV, JSON o Excel.  
   * Esporta il grafico come PNG.  
   * Esporta l'intero database in un file .db per riprendere il lavoro in seguito.

## **🛠️ Tecnologie Utilizzate**

* **HTML, CSS, JavaScript (Vanilla)**  
* **Tailwind CSS:** Per un'interfaccia moderna e reattiva.  
* **SQLite-WASM (sql.js):** Per il database SQL eseguito nel browser.  
* **Monaco Editor:** Per l'editor di codice avanzato.  
* **Tabulator.js:** Per la griglia di dati interattiva.  
* **Plotly.js:** Per la creazione di grafici.  
* **SheetJS (xlsx):** Per la lettura di file Excel.  
* **Phosphor Icons:** Per le icone dell'interfaccia.

## **📄 Licenza**

Questo progetto è rilasciato sotto la **Licenza MIT**.
