# Railway Data Processor

Script Python per il parsing, la geolocalizzazione e la gestione di dati ferroviari provenienti da file JSON archiviati in **Azure Blob Storage** (i dati sono raccolti da <a href="https://trainstats.altervista.org/">TrainStats</a>, con salvataggio su database **PostgreSQL**.

## Link base dati
<a href="https://www.dropbox.com/scl/fo/uv5rz6y6gqpkpciyymg0b/ALu4uc7oD0v_iGdFsSYYJZE?rlkey=smo0xhqe4ha7bxjnwfsooagg3&st=tg1ugil5&dl=0">LINK</a>

## Funzionalità

- Connessione sicura a PostgreSQL e Azure Blob Storage via `.env`
- Parsing dei file JSON con informazioni su treni e fermate
- Geolocalizzazione delle stazioni con `geopy` e `Nominatim`
- Inserimento strutturato dei dati nelle tabelle `station` e `train`
- Supporto a caching dei nomi per evitare duplicazioni
- Pulizia e reset automatico delle tabelle prima del caricamento

---

## Requisiti

Assicurati di avere installato i seguenti pacchetti:

```bash
pip install -r requirements.txt
