[English](README.md) | **Italiano**

# 🎬 Netflix Clone — React (JavaScript)

Prima versione del Netflix Clone: un'applicazione front-end che replica l'interfaccia di Netflix, sviluppata con **React, JavaScript e Vite**. I dati relativi a film e serie TV vengono recuperati dalle API di **The Movie Database (TMDB)**.

> 🔄 **Di questo progetto esiste una versione più recente.** È stato successivamente rifattorizzato in **TypeScript**, e le chiamate a TMDB sono state spostate su un back-end dedicato in Java Spring che funge da proxy, in modo da non esporre più la chiave API lato client.
> Nuova versione: [Netflix-Clone-Refactor-JS-to-TS](https://github.com/giannibussoletti/Netflix-Clone-Refactor-JS-to-TS) · [Demo live](https://netflixcloneportfolio.vercel.app/)

---

## ✨ Funzionalità

- **Home** — carosello a tutto schermo con i film in uscita, seguito dai caroselli di film popolari, serie TV più votate e serie TV popolari
- **TV Show** — pagina dedicata alle serie TV, organizzata in caroselli
- **Movies** — pagina dedicata ai film, organizzata in caroselli
- **Ricerca** — barra di ricerca nella navbar che cerca contemporaneamente film, serie TV e persone
- **Pagina di dettaglio** — raggiungibile dal carosello principale o da un poster nei caroselli secondari; riporta poster e logo del titolo, trama, anno di uscita, durata, generi e voto
- **Login Page** — mockup dell'interfaccia di accesso Netflix, esclusivamente visivo, senza un sistema di autenticazione reale
- **Settings** — mockup della pagina delle impostazioni con profili, dettagli account, piano di abbonamento e lingua

---

## 🛠️ Stack tecnico

- [React](https://react.dev/) 19
- JavaScript (JSX)
- [Vite](https://vitejs.dev/)
- [React Router](https://reactrouter.com/)
- [React Bootstrap](https://react-bootstrap.github.io/) e [Bootstrap](https://getbootstrap.com/)
- [FontAwesome](https://fontawesome.com/)

**Dati:** [API TMDB](https://developer.themoviedb.org/reference/intro/getting-started), interrogate direttamente dal front-end tramite `fetch`.

---

## 🚀 Avvio del progetto

### Prerequisiti

- [Node.js](https://nodejs.org/) (versione LTS consigliata) e npm
- Un **API Read Access Token** di TMDB, ottenibile gratuitamente da [themoviedb.org/settings/api](https://www.themoviedb.org/settings/api) dopo aver creato un account

### Installazione

1. Clonazione del repository:

   ```bash
   git clone https://github.com/giannibussoletti/Netflix_Clone_React_Build.git
   cd Netflix_Clone_React_Build
   ```

2. Installazione delle dipendenze:

   ```bash
   npm install
   ```

3. Creazione di un file `.env` nella root del progetto con il token di TMDB:

   ```env
   VITE_API_KEY=il_tuo_api_read_access_token_tmdb
   ```

4. Avvio del server di sviluppo:

   ```bash
   npm run dev
   ```

   L'applicazione risulta disponibile all'indirizzo [http://localhost:5173](http://localhost:5173).

> ⚠️ In questa versione le richieste a TMDB partono dal browser, quindi il token finisce nel codice lato client. Per l'uso in locale va bene, ma è uno dei motivi per cui il progetto è stato ricostruito con un back-end proxy nella [versione TypeScript](https://github.com/giannibussoletti/Netflix-Clone-Refactor-JS-to-TS).
