# CAPITOLO 7: Ricerca Corrispondenza

## Teoria delle Funzioni di Ricerca in Excel

Excel offre diverse funzioni di ricerca che consentono di trovare i dati all'interno di un foglio di calcolo. Le funzioni più comunemente usate includono VLOOKUP, HLOOKUP, INDEX, MATCH e XLOOKUP. Di seguito vengono descritte ciascuna di queste funzioni, con esempi e considerazioni sulle loro differenze e applicazioni.

### 1. VLOOKUP (Vertical Lookup)
- **Sintassi**: `VLOOKUP(valore_cercato, tabella_array, indice_colonna, [intervallo])`
- **Esempio**: `=VLOOKUP(A2, B2:D5, 3, FALSO)` cerca il valore in A2 nella colonna B e restituisce il valore corrispondente dalla terza colonna.

### 2. HLOOKUP (Horizontal Lookup)
- **Sintassi**: `HLOOKUP(valore_cercato, tabella_array, indice_riga, [intervallo])`
- **Esempio**: `=HLOOKUP(G2, A1:D4, 2, FALSO)` cerca il valore in G2 nella riga 1 e restituisce il valore dalla seconda riga.

### 3. INDEX (Restituisce il valore di una cella in una tabella) 
- **Sintassi**: `INDEX(tabella_array, num_riga, [num_colonna])`
- **Esempio**: `=INDEX(A1:C3, 2, 3)` restituisce il valore nella seconda riga e terza colonna.

### 4. MATCH (Restituisce la posizione di un valore in un array) 
- **Sintassi**: `MATCH(valore_cercato, array, [tipo])`
- **Esempio**: `=MATCH(D2, A1:A5, 0)` restituisce la posizione di D2 nell'array A1:A5.

### 5. XLOOKUP (Nuova funzione di ricerca in Excel)
- **Sintassi**: `XLOOKUP(valore_cercato, cerca_in, restituisci, [se_non_trovato], [modalità_correspondanza], [modalità_ricerca])`
- **Esempio**: `=XLOOKUP(E2, F1:F5, G1:G5, "Non trovato")` cerca il valore in E2 nell'intervallo F1:F5 e restituisce il corrispondente in G1:G5.

### Tabella di Confronto
| Funzione | Tipo di Ricerca | Limiti | Esempio di Utilizzo |  
|----------|----------------|-------|--------------------| 
| VLOOKUP  | Verticale      | Solo a sinistra | `=VLOOKUP(A1, B1:C3, 2, FALSE)` |
| HLOOKUP  | Orizzontale    | Solo sopra | `=HLOOKUP(A1, B1:D3, 2, FALSE)` |
| INDEX    | Generale       | Nessun limite | `=INDEX(A1:C10, 2, 3)` |
| MATCH    | Posizionamento  | Selettivo | `=MATCH(A1, A1:A10, 0)` |
| XLOOKUP  | Verticale/Orizzontale | Definito dall'utente | `=XLOOKUP(A1, A2:A10, B2:B10)` |

### Gestione degli Errori
- Utilizzare `IFERROR` per gestire gli errori nelle funzioni di ricerca.
    - Esempio: `=IFERROR(VLOOKUP(A1, B1:C10, 2, FALSE), "Valore non trovato")`

### Scenario Pratico in un Database
Immagina di avere un database di prodotti e desideri cercare il prezzo di un prodotto specifico. Puoi utilizzare VLOOKUP per cercare il prodotto in una lista e restituire il suo prezzo.

Esempio di database:
| Prodotto | Prezzo | Categoria |
|----------|--------|-----------|
| Prodotto A | 10 | Categoria 1 |
| Prodotto B | 20 | Categoria 2 |  
| Prodotto C | 15 | Categoria 1 | 

Utilizza `=VLOOKUP("Prodotto B", A2:C4, 2, FALSE)` per ottenere il prezzo di Prodotto B. 

Con il passare del tempo, considera di aggiornare le tue formule e la loro applicabilità con le versioni più recenti di Excel.

---