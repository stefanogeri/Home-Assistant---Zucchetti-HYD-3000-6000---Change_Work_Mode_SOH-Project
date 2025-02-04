# Home-Assistant---Zucchetti-HYD-3000-6000---Change_Work_Mode_SOH-Project

Descrizione del Progetto: Configurazione e Automazione della Modalità Carica-Scarica per Inverter Solarman
Questo progetto si propone di automatizzare la configurazione della modalità Carica-Scarica di un inverter Solarman utilizzando il protocollo Modbus RTU attraverso Home Assistant. L'obiettivo è garantire che i parametri di carica e scarica della batteria vengano impostati correttamente, permettendo un utilizzo ottimizzato dell'energia in base agli orari definiti.
Caratteristiche Principali:
✅ Scrittura dei parametri Modbus: Invio di pacchetti Write Multiple Holding Registers (0x10) per configurare i registri dell’inverter.
✅ Orari personalizzabili: Definizione flessibile di fasce orarie per la carica e la scarica dell’energia in base alle esigenze dell’utente.
✅ Notifiche dettagliate: Ogni configurazione viene verificata tramite notifiche persistenti che mostrano i valori scritti e quelli letti effettivamente dai sensori.
✅ Test e Debug: Implementazione di diverse versioni di test per ottimizzare l'invio dei comandi e validare il comportamento dell’inverter.
✅ Interfaccia in Home Assistant: Integrazione diretta con Home Assistant per il monitoraggio dei registri tramite sensori Modbus.
Funzionamento:
1.	Configurazione Parametri: Lo script imposta orari di carica e scarica, oltre alla potenza massima supportata.
2.	Attivazione Modalità: Dopo aver inviato i parametri, viene attivata la modalità Timed Charge and Discharge Mode.
3.	Verifica dei Registri: Dopo l’invio dei comandi, Home Assistant legge i registri e genera notifiche con i valori effettivamente impostati.
4.	Monitoraggio: L'utente può controllare in tempo reale i parametri di carica e scarica attraverso i sensori Modbus esposti su Home Assistant.
Obiettivo Finale
Questo progetto consente un controllo intelligente ed efficiente della gestione energetica dell’inverter, garantendo un utilizzo ottimale della batteria garantendo che le stesse siano caricate al 100%, eventualmente con rete elettrica, con cadenza periodica anche in caso di settimane di brutto tempo
