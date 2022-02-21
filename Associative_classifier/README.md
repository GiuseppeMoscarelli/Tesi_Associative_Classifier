# Classificatore Associativo

In questa fase, dopo aver ottenuto i dataset desiderati, è stata eseguita nuovamente
l'estrazione ed il filtraggio dei pattern tramite le configurazioni individuate nelle 
fasi precedenti. Dopo di che si è proseguito con i diversi esperimenti riguardanti il 
classificatore associativo.

Di seguito sono descritti i vari Notebook utilizzati:

#### OTTENIMENTO DEI DATASET
- Il Notebook "Dataset_manipulation.ipynb" contiene il codice che ha permesso lo spit
del dataset desiderato in train e test set. Questi ultimi saranno poi utilizzati 
in fase di classificazione.

#### ESTRAZIONE E FILTRAGGIO DEI PATTERN
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

#### ESPERIMENTI CON IL CLASSIFICATORE ASSOCIATIVO
- Il Notebook "Testing_rules_multiple_match.ipynb" contiene il codice relativo alla 
classificazione associativa tramite il test dei pattern estratti, utilizzando una
soglia indicante il numero di pattern da verificare affinché un record di test sia classificato
in un certo modo. Variando i parametri a disposizione, sono stati effettuati diversi esperimenti.

- Il Notebook "Testing_rules_cascade_classifiers.ipynb" si differenzia da 
"Testing_rules_multiple_match" in quanto è stato introdotto in cascata un albero di 
decione per tutti quei sample che vengono classificati come "Normal". In questo modo 
è stato possibile provare ad incrementare il richiamo.

- Il Notebook "Increase_interpretability_ass_classifier.ipynb" contiene il codice con cui
si è andati a salvare in un file i pattern verificati in un paio di situazioni in 
cui la predizione è stata "QuasiPiena" e quelli in un paio di situazioni in cui la 
predizione è stata "Normal". Questo ha permeso di capire se fosse possibile incrementare 
l'interpretabilità del classificatore associativo.

- Nel Notebook "Testing_rules_multiple_match_Time_Slots.ipynb" è stata effettuata la
classificazione associativa per le diverse fasce orarie considerate.

- Il Notebook "Dumb_Classifier.ipynb" contiene un classificatore stupido che 
classifica tutti i record con lo stato che avevano all’istante precedente.

- Il Notebook "Testing_rules_State_Change.ipynb" contiene un classificatore 
che considera l'effettivo cambio di stato durante la fase di classificazione. Quindi 
prima di classificare un record del test set come QP, viene valutato prima se 
all'istante precedente la stazione si trovava effettivamente in uno stato diverso.

#### FOLDER
- La cartella "Results_pattern_extraction" contiene i pattern risultanti dalle fasi di estrazione 
e filtraggio.