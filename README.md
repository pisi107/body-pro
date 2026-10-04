# Body Pro · Training Club

App di allenamento in italiano, pubblicata con GitHub Pages.

## Funzioni

- Demo immediata e profili locali separati; password derivate con PBKDF2.
- 24 esercizi, 48 fotografie incluse nel sito, istruzioni e ricerca.
- Programmi basati su livello, attrezzatura, durata, obiettivo e focus.
- Schede modificabili, duplicazione e annullamento dell'eliminazione.
- Sessioni con recupero, conteggio serie, ripetizioni effettive e carichi.
- Storico, calendario, registrazione del peso e grafico.
- Esportazione e importazione di backup JSON.
- Layout mobile, icone, manifest e service worker per uso offline dopo il primo caricamento completo.

## Dati

I dati vengono conservati nel browser del dispositivo, senza sincronizzazione cloud.
Esporta un backup dal profilo prima di cancellare i dati del browser o cambiare dispositivo.
La demo usa il profilo condiviso locale admin / admin; crea un profilo personale per separare i dati.
Il recupero password via email non è disponibile: non esiste un backend di autenticazione.
Il generatore usa regole e un catalogo di esercizi, senza chiamate a modelli AI.

## Esecuzione

Servire la cartella con un server HTTP locale, ad esempio: python3 -m http.server 8000.
Pubblicare tutti i file alla radice di GitHub Pages.
Le funzioni di profilo e PWA richiedono HTTPS oppure localhost.

## Foto

Le foto provengono da [Free Exercise DB](https://github.com/yuhonas/free-exercise-db), revisione f00c92c7dcf1216a928a52c3706c7ce8e2f71ed5, distribuito sotto Unlicense.
Le copie locali evitano dipendenze dagli URL delle immagini.
