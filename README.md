# Il Capodanno di Nainggolan — App Calcetto

App web del gruppo per le partite di calcio a 5, 7, 8 e 11.

- **Classifica** per stagione e tipo di partita: presenze, vittorie, pareggi, sconfitte, gol, rigori, autogol, gol subiti, rigori parati, media voto e media fantavoto.
- **Partite**: il presidente crea le partite, fa le squadre (Bianchi / Scuri) e inserisce risultato e tabellino.
- **Voti**: chi ha giocato vota gli altri da 0 a 10 (passi di 0,25) entro 48 ore dal risultato.
- **Coppie**: partite giocate insieme e contro, con vittorie, pareggi e sconfitte.
- **FantaNunnaree**: rosa di 15 giocatori di movimento con 150 crediti, quotazioni che cambiano in base alle prestazioni. Ogni giornata si schiera 1 portiere + 7 di movimento.

## Tecnologia
- Sito statico (`index.html` + `config.js`) pubblicato con GitHub Pages.
- Dati su Supabase (Postgres). Le tabelle non sono leggibili direttamente: tutto passa da funzioni che controllano login e ruolo. Le password sono cifrate.

## Configurazione
In `config.js` vanno l'URL del progetto Supabase e la chiave **publishable** (mai la secret).
