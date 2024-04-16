# Analisi delle serie temporali sul cambiamento delle temperature mondiali

## Panoramica

Questo progetto si propone di analizzare la serie temporale del cambiamento delle temperature mondiali dal 1750 ai giorni nostri. L'obiettivo è comprendere i pattern, identificare trend, rilevare stagionalità, esaminare l'autocorrelazione e la stazionarietà, e sviluppare un modello di previsione.

## Metodologia

Per l'analisi, abbiamo utilizzato la libreria Python `statsmodels`. Le tecniche di decomposizione applicate ci hanno permesso di separare la serie in componenti di tendenza, stagionalità e residui, distinguendo gli effetti a lungo termine dalle fluttuazioni stagionali e dai disturbi casuali.

## Obiettivi

- **Esame dei Dati**: Esaminare attentamente la serie temporale delle temperature per identificare tendenze a lungo termine e valutare la presenza di stagionalità.
- **Modello di Previsione**: Utilizzare il modello SARIMA per fare previsioni sul comportamento futuro delle temperature.
- **Autocorrelazione**: Analizzare i coefficienti di autocorrelazione parziale e semplice per identificare dipendenze temporali.

## Analisi dei dati

**Fase 1 - Analisi globale:**

1.  **Pulizia e preprocessing:**

    - Eliminazione di dati duplicati e normalizzazione dei nomi dei paesi.
    - Rimozione di dati incompleti o mancanti.
    - Estrazione della temperatura media per paese e creazione di una mappa interattiva del globo.

2.  **Analisi temporale:**

    - Calcolo della temperatura media globale per anno e per stagione.
    - Creazione di grafici a linee per visualizzare i cambiamenti nel tempo.
    - Focus sui dati dal 1900 al 2015 per l'analisi di trend e stagionalità.

3.  **Scomposizione della serie temporale:**

    - Separazione della serie nelle componenti di trend, stagionalità e residui.
    - Analisi dei pattern e delle caratteristiche di ciascuna componente.

4.  **Verifica della stazionarietà:**

    - Utilizzo del test di Dickey-Fuller aumentato (ADF test) per verificare la stazionarietà della serie.
    - Applicazione della differenziazione per rendere la serie stazionaria se necessario.
    - Calcolo dell'autocorrelazione (ACF) e dell'autocorrelazione parziale (PACF) per identificare le relazioni temporali.

**Fase 2 - Caso studio della città di Ancona:**

1.  **Estrazione e preprocessing:**

    - Filtraggio dei dati per isolare la città di Ancona.
    - Pulizia e selezione del periodo di analisi (1900-2012).

2.  **Analisi temporale:**

    - Calcolo della temperatura media mensile e annuale.
    - Creazione di grafici a linee, box plot e heatmap per visualizzare i cambiamenti nel tempo e la stagionalità.
    - Studio della media mobile per identificare le tendenze a lungo termine.

3.  **Verifica della stazionarietà:**

    - Applicazione dell'ADF test per verificare la stazionarietà della serie.

4.  **Modello predittivo SARIMA:**

    - Divisione del dataset in training set, validation set e test set.
    - Applicazione del modello SARIMA per prevedere la temperatura mensile.
    - Valutazione del modello con metriche di errore (MAE, MSE, RMSE, R-squared).
    - Analisi dei risultati e confronto con una previsione di base.

## Risultati e Discussione

L'analisi evidenzia un trend di aumento della temperatura globale e stagionale, confermato anche dal caso studio di Ancona. Il modello SARIMA dimostra una buona capacità predittiva con un basso margine di errore. Questi risultati supportano l'evidenza del cambiamento climatico e l'importanza di un monitoraggio costante delle temperature.

## Conclusioni

L'analisi delle serie temporali è uno strumento fondamentale per comprendere il cambiamento climatico e le sue implicazioni. Il progetto ha dimostrato l'utilità di Python e della libreria statsmodels per l'analisi di dati climatici. Le previsioni generate dal modello SARIMA possono essere utili per pianificare strategie di mitigazione e adattamento ai cambiamenti climatici.

## Notebooks

- **Prima parte:** Analisi del dataset e studio della temperatura globale.
- **Seconda parte:** Analisi della temperatura di Ancona e sviluppo del modello SARIMA.

## Dataset Utilizzati

- `GlobalLandTemperaturesByCountry.csv`: Temperature per ogni nazione dal 1743.
- `GlobalLandTemperatures.csv`: Media della temperatura globale per ogni mese dell'anno dal 1743.
- `GlobalLandTemperaturesByCity.csv`: Dati per alcune delle maggiori città mondiali, inclusa un'analisi dettagliata sulla città di Ancona.

## Strumenti

- Libreria Python statsmodels per l'analisi delle serie temporali.
- Librerie Python pandas, numpy, seaborn, matplotlib e plotly per la manipolazione dei dati e la visualizzazione.
