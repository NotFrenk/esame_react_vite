# VOLOX

## Descrizione

VOLOX è un'applicazione web per la ricerca di voli. Il frontend è sviluppato con **React** e **Vite**, mentre il backend utilizza **Flask**.

## Tecnologie Utilizzate

- **Frontend**: React, Vite
- **Backend**: Flask
- **Stile**: CSS personalizzato

## Requisiti

Assicurati di avere installati i seguenti strumenti:

- **Node.js** (versione più recente consigliata)
- **Python 3** e dipendenze Flask (`pip install flask flask-cors psycopg2`)

## Installazione

### 1. Clonare il repository
```sh
 git clone <URL_DEL_REPOSITORY>
 cd esame_react_vite
```

### 2. Avviare il backend Flask

1. Esegui il backend:
   ```sh
   python query.py
   ```

Il server Flask sarà avviato su `http://127.0.0.1:5001`.

### 2. Installare le dipendenze del frontend
```sh
npm install
```

### 3. Avviare il frontend
```sh
npm run dev
```

## API disponibili

Il backend fornisce le seguenti API:

- `GET /aeroporti` → Restituisce l'elenco dei voli fuori L'italia.
- `GET /vol.sopra.med` → Restituisce l'elenco dei voli in L'italia.
- `GET /serv.api` → Restituisce l'elenco di tutti i voli.

## Struttura del Progetto

```
│── frontend/
│   ├── src/
│   │   ├── App.jsx       # Componente principale React
│   │   ├── main.jsx      # Punto di ingresso di React
│   │   ├── App.css       # Stili principali
│   │   ├── index.css     # Stili globali
│   ├── public/
│   │   ├── index.html    # File HTML principale
│   ├── package.json      # Dipendenze frontend
│   ├── vite.config.js    # Configurazione Vite
│
│── backend/
│   ├── query.py          # API Flask per interrogare il database
│   ├── requirements.txt  # Dipendenze Python
```
