# My Biblion 
> Questo blog online ti permette di pubblicare articoli di qualsiasi genere e di leggere quelli dei tuoi amici.


<div align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E">
  <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white">
  <img src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white">
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white">
  <img src="https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white">
</div>




## Come lanciare il sito
* Scaricare il file .zip
* Aprire il terminale 
* Posizionarsi nella directory \backend\
* Lanciare il comando _"npm install"_
* Per avviare il server, lanciare il comando _"npm start"_
* Due possibili opzioni:
  * Tramite cartella: cliccare sul file index.html per avviare il sito
  * Tramite VScode: utilizzando l’estensione Live server



## Schermate del sito

### Pagina di Login / Registrazione
![](images/login.PNG)

### Home Page
![](images/home.PNG)

### Profilo Utente
![](images/profile.PNG)

### Scrittura articolo
![](images/writepost.PNG)

### Articolo Pubblicato
![](images/article.PNG)

### Numeri di click sull'articolo
![](images/statistic.PNG)


## Struttura del progetto

* _index.html_: è il file utilizzato da script.js per far visualizzare le varie pagine che l’utente che può selezionare. E’ una specie di contenitore, che in base all’interazione che l’utente ha con la pagina, cambia dinamicamente il suo contenuto. Per evitare errori legati alle cors, nell’head del file sono linkati tutti i file di stile css presente nella directory \styles, che vengono rimossi dallo script.js quando necessario.

* _script.js_: è il file responsabile della logica del sito. Tramite JQuery manipola il file index.html per effettuare il routing tra le pagine in base alle richieste dell’utente. Parte dal rendering della pagina di Log-In tramite 
funzione ‘load’ di JQuery, e successivamente, tramite metodi di gestione degli eventi di JQuery vengono mostrate le altre pagine
 
* _\styles\login.css_: foglio di stile relativo alla pagina login.html
* _\styles\style_home_post_page.css_: foglio di stile relativo alla home page, alla pagina di un articolo singolo e alla pagina del profilo utente
* _\styles\write_post.css_: foglio di stile relativo alla pagina per scrivere un articolo
* _\src\home_page.html_: pagina html relativa alla home page
* _\src\login.html_: pagina html relativa alla pagina di Log-in / Register
* _\src\post_page.html_: pagina html relativa alla pagina  di un articolo singolo
* _\src\write_post.html_: pagina html relativa alla pagina di scrittura di un articolo
* _\assets\_ : contiene tutte le immagini usate nel sito
* _\.vscode\settings.json_: file responsabile per disattivare live reload
* _\backend\database.js_: il file serve ad aprire una connessione con il database usando SQlite
* _\backend\server.js_: il file è responsabile di far partire il server e gestisce tutte le richieste HTTP che vengono fatte dal client utilizzando la connessione al database
* _\backend\db.sql_: il file contiene il database, visualizzabile da VScode tramite l’estensione SQlite Viewer
* _\backend\package.json_: file di configurazione per installare pacchetti con npm
