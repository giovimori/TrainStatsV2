# TrainStats - Outlier Detection sui Ritardi Ferroviari Italiani

## Descrizione del Progetto

Questo progetto è stato sviluppato per il corso di **Laboratorio di Ottimizzazione, Intelligenza Artificiale e Machine Learning**. L'obiettivo principale è l'identificazione e l'analisi delle anomalie (Outlier Detection) nelle performance della rete ferroviaria italiana attraverso tecniche di apprendimento non supervisionato.

L'analisi mette a confronto due periodi stagionali distinti per valutare l'impatto della stagionalità sui ritardi:
* **Dicembre 2025:** Analisi del traffico nel periodo invernale e festivo.
* **Aprile 2026:** Analisi del traffico nel periodo primaverile.

## Dataset

- **Volume:** ~500.000 corse monitorate (circa 250k per mese).
- **Ambito:** Analisi focalizzata esclusivamente sui **treni passeggeri** (REG, FR, IC, ICN, FA, FB, EC). Sono stati esclusi convogli tecnici, merci e internazionali per garantire la coerenza del modello.
- **Feature Engineering:** Creazione di variabili sintetiche quali fasce orarie (`Ora_Arrivo`), giorno della settimana e indicatore weekend (`Is_Weekend`).

## Come Eseguire il Progetto

1.  Clona la repository o scarica la cartella.
    ```bash
    git clone <url-repository>
    ```
2.  Installa le dipendenze:
    ```bash
    pip install -r requirements.txt
    ```
3.  Avvia il notebook:
    ```bash
    jupyter notebook train_statsV2.ipynb
    ```

## Tecnologie Utilizzate

* **Linguaggio:** Python 3.x
* **Ambiente:** Jupyter Notebook
* **Librerie principali:**
    * Analisi Dati: `Pandas`, `NumPy`
    * Machine Learning: `Scikit-Learn`
    * Visualizzazione: `Matplotlib`, `Seaborn`

## Autori
* **Giovanni Morelli** 

---
*Corso di Laboratorio di Ottimizzazione, Intelligenza Artificiale e Machine Learning | CdL Tecnologie dei Sistemi Informatici | Università di Bologna | A.A. 2025-2026*

Fonte dati: [trainstats.com](https://trainstats.altervista.org/)
