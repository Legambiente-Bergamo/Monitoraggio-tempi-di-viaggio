# Monitoraggio tempi di viaggio

La repository contiene i risultati del monitoraggio dei tempi di viaggio in auto, aggiornati quotidianamente, 
lungo alcune direttrici interessate da futuri interventi viabilistici. I risultati sono raccolti nel file 
travel_times.csv e sono ottenuti in tempo reale chiamando la [API Google 
Routes](https://developers.google.com/maps/documentation/routes/overview). I percorsi sono "vincolati", cioè non 
variano nel corso della giornata: questo comporta che il percorso seguito non sia necessariamente il più veloce, 
ma consente di valutare gli effetti della congestione sulle prestazioni della rete stradale.

I campi del file di riepilogo sono i seguenti:
 - "Percorso": nome del percorso completo;
 - "Tratta": nome della parte di percorso:
 - "Direzione": 0 se la direzione è quella indicata nel nome della tratta, 1 se è il ritorno;
 - "Distanza_m": lunghezza del percorso in metri;
 - "Durata_m": durata effettiva del viaggio in minuti;
 - "Durata_scarica_m": durata teorica del viaggio (a rete scarica, cioè senza congestione) in minuti;
 - "Data": data del viaggio e della chiamata all'API;
 - "Ora": ora del viaggio e della chiamata all'API.
