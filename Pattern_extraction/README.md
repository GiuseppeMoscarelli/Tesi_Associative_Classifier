# Fase di estrazione e filtraggio dei pattern

#### EXTRACTION NOTEBOOKS
- Il Notebook "AllStates.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze di tutti gli stati critici. Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "Empty_almostEmpty.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze degli stati "Vuota" e "QuasiVuota". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "Full_almostFull.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze degli stati "Piena" e "QuasiPiena". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "Full_Empty.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze degli stati "Piena" e "Vuota". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "StateChange_Empty_almostEmpty.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Vuota" e "QuasiVuota". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "StateChange_Full_almostFull.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Piena" e "QuasiPiena". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "StateChange_Normal_Full_almostFull.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Normale","Piena" e "QuasiPiena". 
Variando i parametri a disposizione, si sono ottenute diverse configurazioni 
usate per l'estrazione.

- Il Notebook "StateChange_Normal_almostEmpty.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Normale", Vuota e "QuasiVuota". 
Variando i parametri a disposizione, si sono ottenute diverse configurazioni 
usate per l'estrazione.

- Il Notebook "StateChange_Normal_almostEmpty.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Normale" e "QuasiVuota", in cui lo stato 
"QuasiVuota" comprende anche lo stato "Vuota". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "StateChange_Normal_almostFull.ipynb" contiene il codice relativo 
all'estrazione dei pattern considerando come evento di interesse soltanto il
cambiamento di stato agli stati "Normale" e "QuasiPiena", in cui lo stato
"QuasiPiena" include anche lo stato "Piena". Variando i parametri a 
disposizione, si sono ottenute diverse configurazioni usate per l'estrazione.

- Il Notebook "Empty_almostEmpty_time_slots.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze degli stati "Vuota" e "QuasiVuota", 
dividendo l'arco della giornata in varie fasce orarie ed effettuando l'estrazione
singolarmente per ciscuna fascia. Variando i parametri a disposizione, si sono ottenute diverse 
configurazioni usate per l'estrazione.

- Il Notebook "Full_almostFull_time_slots.ipynb" contiene il codice relativo all'estrazione
dei pattern considerando tutte le occorrenze degli stati "Piena" e "QuasiPiena", 
dividendo l'arco della giornata in varie fasce orarie ed effettuando l'estrazione
singolarmente per ciscuna fascia. Variando i parametri a disposizione, si sono ottenute diverse 
configurazioni usate per l'estrazione.

- Il Notebook "Pattern_filtering.ipynb" contiene il codice per il filtraggio
dei pattern interessanti tra tutti quelli ottenuti. Oltre ai risultati ottenuti, 
per ogni file in input, vengono salvati i plot "supporto-confidenza" ed un plot
che mostra la distribuzione dei pattern ottenuti dopo il filtraggio, in base alla 
loro confidenza.

#### RESULT FOLDERS
- Nella cartella "Results_extraction" sono contenuti tutti i pattern estratti dalle
varie configurazioni utilizzate.

- Nella cartella "Results_filtered_patterns" sono contenuti tutti i pattern ottenuti
dopo l'applicazione del filtro.



