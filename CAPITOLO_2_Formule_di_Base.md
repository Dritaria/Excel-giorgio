# Formule di Base in Excel

## Teoria sulle formule
Le formule in Excel costituiscono una parte fondamentale dell'utilizzo del programma, permettendo di eseguire calcoli e manipolazioni dei dati. Una formula inizia sempre con il simbolo `=` seguito da una combinazione di numeri, celle, e operatori.

## Operatori Aritmetici
Gli operatori aritmetici sono i seguenti:
- **`+`** (Addizione)
- **`-`** (Sottrazione)
- **`*`** (Moltiplicazione)
- **`/`** (Divisione)
- **`^`** (Esponenziazione)

### Esempio:
Presupponiamo di avere i seguenti dati:
- Cell A1: 10
- Cell A2: 5

La formula per sommare A1 e A2:
```
= A1 + A2
```
Risultato: 15

## Riferimenti Assoluti e Relativi
In Excel, i riferimenti possono essere relativi o assoluti:
- **Riferimento Relativo**: cambia quando la formula viene copiata in un'altra cella. (es. `A1`)
- **Riferimento Assoluto**: rimane fisso quando la formula viene copiata. (es. `$A$1`)

### Esempio:
Se in cella B1 scriviamo `=A1`, e poi copiamo la formula in B2, diventerà `=A2`. Se scriviamo `=$A$1`, rimarrà sempre `=$A$1` anche se copiata.

## Operatore di Concatenazione
L'operatore di concatenazione in Excel è `&`. Questo operatore permette di unire il contenuto di più celle o stringhe di testo.  

### Esempio:
Se in A1 abbiamo "Ciao " e in B1 "Mondo", la formula per concatenare:
```
= A1 & B1
```
Risultato: "Ciao Mondo"

![Screenshot esempio concatenazione](screenshot_url)

## Considerazioni Finali
Utilizzare le formule in Excel rende il lavoro con i dati molto più efficiente. Con la pratica e la comprensione dei diversi operatori e riferimenti, è possibile eseguire compiti complessi con notevole facilità.

---

### Screenshot Descrizioni:
- L'immagine mostra un esempio di utilizzo degli operatori aritmetici.
- L'immagine illustra la differenza tra riferimenti assoluti e relativi.
- Un esempio di concatenazione con i dati di partenza e il risultato finale.

