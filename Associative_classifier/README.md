# Classificatore Associativo

In questa fase, dopo aver ottenuto i dataset desiderati, è stata eseguita nuovamente
l'estrazione ed il filtraggio dei pattern tramite le configurazioni individuate nelle 
fasi precedenti. Dopo di che si è proseguito con i diversi esperimenti riguardanti il 
classificatore associativo.

Di seguito sono descritti i vari Notebook utilizzati:

### OTTENIMENTO DEI DATASET
- Il Notebook "Dataset_manipulation.ipynb" contiene il codice che ha permesso lo spit
del dataset desiderato in train e test set. Questi ultimi saranno poi utilizzati 
in fase di classificazione.

### ESTRAZIONE E FILTRAGGIO DEI PATTERN
- Il Notebook "Pattern_Extraction_StateChange_Normal_almostFull.ipynb" contiene 
il codice relativo all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Normale" e "QuasiPiena". Variando il valore dell'intervallo
temporale, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "Pattern_Extraction_Time_slots_StateChange_Normal_almostFull.ipynb" 
contiene il codice relativo all'estrazione dei pattern per le diverse fasce orarie
considerando come evento di interesse soltanto il cambiamento di stato agli stati 
"Normale" e "QuasiPiena". 

- Il Notebook "Pattern_filtering.ipynb" è stato utilizzato per il filtraggio dei pattern,
utilizzando i diversi parametri messi a disposizione.

### ESPERIMENTI CON IL CLASSIFICATORE ASSOCIATIVO


### FOLDER
- La cartella "Results_pattern_extraction" contiene i pattern risultanti dalle fasi di estrazione 
e filtraggio.