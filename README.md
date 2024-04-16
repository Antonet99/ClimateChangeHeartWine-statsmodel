# Analisi delle Serie Temporali sul Cambiamento delle Temperature Mondiali

## Panoramica

Questo progetto si propone di analizzare la serie temporale del cambiamento delle temperature mondiali dal 1750 ai giorni nostri. L'obiettivo è comprendere i pattern, identificare trend, rilevare stagionalità, esaminare l'autocorrelazione e la stazionarietà, e sviluppare un modello di previsione.

## Metodologia

Per l'analisi, abbiamo utilizzato la libreria Python `statsmodels`. Le tecniche di decomposizione applicate ci hanno permesso di separare la serie in componenti di tendenza, stagionalità e residui, distinguendo gli effetti a lungo termine dalle fluttuazioni stagionali e dai disturbi casuali.

## Obiettivi

- **Esame dei Dati**: Esaminare attentamente la serie temporale delle temperature per identificare tendenze a lungo termine e valutare la presenza di stagionalità.
- **Modello di Previsione**: Utilizzare il modello SARIMA per fare previsioni sul comportamento futuro delle temperature.
- **Autocorrelazione**: Analizzare i coefficienti di autocorrelazione parziale e semplice per identificare dipendenze temporali.

## Risultati e Discussione

Discuteremo i risultati ottenuti dall'analisi e dal modello di previsione, evidenziando le implicazioni per lo studio del cambiamento climatico e l'importanza di un'analisi accurata delle serie temporali.

## Dataset Utilizzati

- `GlobalLandTemperaturesByCountry.csv`: Temperature per ogni nazione dal 1743.
- `GlobalLandTemperatures.csv`: Media della temperatura globale per ogni mese dell'anno dal 1743.
- `GlobalLandTemperaturesByCity.csv`: Dati per alcune delle maggiori città mondiali, inclusa un'analisi dettagliata sulla città di Ancona.
