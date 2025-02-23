# VOLOX

VOLOX è un'applicazione web che permette di visualizzare informazioni sui voli disponibili. Il progetto utilizza **React con Vite** per il frontend e **Flask** con per il backend.

## Tecnologie Utilizzate

- **Frontend**: React (Vite)
- **Backend**: Flask
- **CSS**: Stili personalizzati con `App.css` e `index.css`

## Installazione

### 1. Clonare il repository
```sh
 git clone <repo-url>
 cd volox
```

### 2. Installare le dipendenze frontend
```sh
 cd frontend
 npm install
```

### 3. Avviare il frontend
```sh
 npm run dev
```

### 4. Installare le dipendenze backend
Assicurati di avere **Python 3** installato. Poi esegui:
```sh
 cd backend
 pip install -r requirements.txt
```

### 5. Configurare il database PostgreSQL
Modifica le credenziali di accesso al database nel file `query.py`:
```python
DB_CONFIG = {
    "host": "localhost",
    "port": "5432",
    "dbname": "postgres",
    "user": "postgres",
    "password": "postgres",
}
```

### 6. Avviare il backend
```sh
 python query.py
```

Il backend sarà disponibile su `http://localhost:5001`

## Struttura del Progetto

```
volox/
├── frontend/
│   ├── src/
│   │   ├── App.jsx        # Componente principale React
│   │   ├── main.jsx       # Punto di ingresso di React
│   │   ├── App.css        # Stili principali
│   │   ├── index.css      # Stili globali
│   ├── public/
│   │   ├── index.html     # File HTML principale
│   ├── package.json       # Dipendenze frontend
│   ├── vite.config.js     # Configurazione Vite
│
├── backend/
│   ├── query.py           # API Flask per interrogare il database
│   ├── requirements.txt   # Dipendenze Python
```

## API Disponibili

- **GET /aeroporti**: Restituisce un elenco di aeroporti disponibili.
- **GET /vol.sopra.med**: Restituisce i voli con durata sopra la media.
- **GET /serv.api**: Restituisce gli aeroporti serviti da più di una compagnia.

## Utilizzo dell'App
Una volta avviati frontend e backend:
1. Apri `http://localhost:5173` nel browser.
2. Usa i pulsanti per interrogare le API e ottenere i risultati.

## Contributi
Se vuoi contribuire, sentiti libero di aprire una pull request o segnalare problemi nella sezione Issues!

---

**Autore**: [Il tuo nome]  
**Licenza**: MIT

