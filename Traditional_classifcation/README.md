# Classificazione Tradizionale

- Nel Notebook "Classification.ipynb" è contenuto il codice che ha permesso di ottenere
un dataset per ogni stazione, sui quali sono poi andato ad allenare (con i parametri di
default) e testare i modelli  per i vari algoritmi di classificazione tradizionali.

- Nel Notebook "Tuning.ipynb" è contenuto il codice che ha permesso di effettuare una fase
di finetuning degli iperparametri, tramite la GridSearchCV. I migliori modelli ottenuti
sono stati poi testati sui vari test set.

- Nel Notebook "Tuning_with_treshold.ipynb" è contenuto il codice che ha permesso di effettuare una fase
di finetuning degli iperparametri dell'albero di decisione, tramite la GridSearchCV. 
Nella fase di test dei migliori modelli ottenuti è stata inserita una soglia di probabilità
che ha permesso di aumentare la precisione a discapito del richiamo.
E' stato anche inserito un flag che ha permesso di allenare gli alberi non considerando 
l'informazione relativa al numero di bici disponibili.
Infine, è contenuto il codice che ha permesso di ottenere i cammini di decisione
che hanno determinato la predizione di quei record classificati come “QuasiPiena” 
con un certa soglia di probabilità.

- Nel Notebook "Tuning_with_threshold_Time_Slots.ipynb" è contenuto il codice che 
ha permesso di effettuare una fase di finetuning degli iperparametri,
considerando separatamente le diverse fasce orarie. I migliori modelli ottenuti
sono stati poi testati sui vari test set.

- Nella cartella "trained_models" sono contenuti tutti i modelli ottenuti dalla fase di 
training effettuata utilizzando i parametri di default.

- Nella cartella "tuned_models" sono contenuti tutti i modelli ottenuti dalla fase di 
tuning degli iperpanametri.

- Nella cartella "tuned_models_time_slots" sono contenuti tutti i modelli ottenuti dalla fase di 
tuning degli iperpanametri, considerando le diverse fasce orarie.

- Nella cartella "tuned_models_wo_bikes_inf" sono contenuti tutti i modelli ottenuti dalla fase di 
tuning degli iperpanametri, non considerando le informazioni relative al numero di bici disponibili.

- Nella cartelle "test_results" sono contenuti tutti i risultati delle varie fasi di
test.