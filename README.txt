Inserire in questo documento:
1.	(obbligatorio) Una descrizione dei file del progetto che state allegando a questo compito (cioè un README del file zip contenente i file del progetto)

README per il lancio del sito:
1.	Aprire il terminale 
2.	Posizionarsi nella directory \backend\
3.	Lanciare il comando ‘npm install’
4.	Lanciare il comando per avviare il server ‘npm start’
5.	Due possibili opzioni:
1.	Tramite directory: cliccare sul file index.html per avviare il sito
2.	Tramite VScode: utilizzando l’estensione Live server

Nella cartella allegata (MyBiblion) sono presenti i seguenti file:
1.	index.html: è il file utilizzato da script.js per far visualizzare le varie pagine che l’utente che può selezionare. E’ una specie di contenitore, che in base all’interazione che l’utente ha con la pagina, cambia dinamicamente il suo contenuto. Per evitare errori legati alle cors, nell’head del file sono linkati tutti i file di stile css presente nella directory \styles, che vengono rimossi dallo script.js quando necessario.

2.	script.js: è il file responsabile della logica del sito. Tramite JQuery manipola il file index.html per effettuare il routing tra le pagine in base alle richieste dell’utente. Parte dal rendering della pagina di Log-In tramite 
funzione ‘load’ di JQuery, e successivamente, tramite metodi di gestione degli eventi di JQuery vengono mostrate le altre pagine

3.	\styles\login.css: foglio di stile relativo alla pagina login.html
4.	\styles\style_home_post_page.css: foglio di stile relativo alla home page, alla pagina di un articolo singolo e alla pagina del profilo utente
5.	\styles\write_post.css: foglio di stile relativo alla pagina per scrivere un articolo
6.	\src\home_page.html: pagina html relativa alla home page
7.	\src\login.html: pagina html relativa alla pagina di Log-in / Register
8.	\src\post_page.html: pagina html relativa alla pagina  di un articolo singolo
9.	\src\write_post.html: pagina html relativa alla pagina di scrittura di un articolo
10.	\assets\ : contiene tutte le immagini usate nel sito
11.	\.vscode\settings.json: file responsabile per disattivare live reload
12.	\backend\database.js: il file serve ad aprire una connessione con il database usando SQlite
13.	\backend\server.js: il file è responsabile di far partire il server e gestisce tutte le richieste HTTP che vengono fatte dal client utilizzando la connessione al database
14.	\backend\db.sql: il file contiene il database, visualizzabile da VScode tramite l’estensione SQlite Viewer
15.	\backend\package.json: file di configurazione per installare pacchetti con npm

