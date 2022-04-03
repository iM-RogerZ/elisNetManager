# elisNetManager

Script per l'autenticazione automatica alla rete ELIS.org Studenti.

Sono necessari i 3 file:
- elisNetAutoLogin.exe: script che esegue varie richieste http per l'autenticazione. Lo script sarà eseguito in background.
- elisNetAutoLoginSettings.json: file json autogenerato dallo script, dove andranno inserite le credenziali necessarie per l'accesso ad ELIS.org Studenti
- elisNetAutoLogin.xml: file XML contenente le informazioni di una Task Windows che funge da trigger. Ogni volta che ci si collega ad una rete, la task windows lancia lo script per l'autoconnessione. Lo script è in grado di capire se la connessione necessita di una utenticazione da gstatic.com, di conseguenza si chiude immediatamente se la rete non è quella elis.

Tutti i file saranno all'interno della cartella C:\Windows\System32\elisNetManager

RICORDA di modificare le credenziali presenti nel file elisNetAutoLoginSettings.json nella cartella C:\Windows\System32\elisNetManager
