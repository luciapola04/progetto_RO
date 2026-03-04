# Progetto RO

Questo progetto implementa un algoritmo in **Python** per la verifica dell'ottimalità di una soluzione candidata in un problema di Programmazione Lineare (PL) tramite il **Teorema degli Scarti Complementari**.

Il tool è progettato per gestire problemi in forma canonica, analizzare la regione ammissibile e risolvere il sistema duale associato, garantendo robustezza anche in presenza di **vertici degeneri**.

## 🚀 Caratteristiche
- **Parser Testuale:** Inserimento dei vincoli e della funzione obiettivo tramite stringhe (grazie a Regex).
- **Analisi dell'Ammissibilità:** Controllo automatico del rispetto dei vincoli primali ($x \in X$).
- **Verifica Duale:** Costruzione e risoluzione del sistema duale associato tramite `scipy.optimize.linprog`.
- **Gestione Degenerazione:** Algoritmo ottimizzato per gestire vertici in cui il numero di vincoli attivi è superiore al numero di variabili.

## 🛠 Installazione e Utilizzo
Il progetto è ottimizzato per essere eseguito su **Google Colab** o in locale tramite Jupyter Notebook.

### Requisiti
```bash
pip install numpy scipy
