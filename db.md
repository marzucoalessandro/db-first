Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato.

database name : Videogames list.
table name : Videogames;

Row:

- ID                   NUMERO MEDIUMINT PRIMARYKEY NOTNULL
- NOME_GIOCO           STRINGA VARCHAR(50) NOTNULL
- BARCODE              NUMBER BIGINT NOTNULL UNIQUE
- DESCRIZIONE          STRINGA TEXT NULL
- CASA_PRODUTTRICE     STRINGA VARCHAR(30) NULL
- CASA_SVILUPPATRICE   STRINGA VARCHAR(30) NULL
- ANNO_DI_USCITA       DATA YEAR NULL
- GENERE               STRINGA VARCHAR(20) NULL
- PIATTAFORMA          STRINGA VARCHAR(30) NOTNULL
- DISPONIBILITA'       NUMBER TINYINT(BOOL) NOTNULL DEFAULT(0)
- NUMERO_UNITA'        NUMBER SMALL NOTNULL
- UNITA'_VENDUTE       NUMBER SMALL NOTNULL
- NUOVA_DISPONIBILITA' DATA DATE NULL
- PREZZO               NUMBER FLOAT(5, 2) NOTNULL
- SCONTO               NUMBER FLOAT(4, 2) NULL DEFAULT(0)
- SCREENSHOT           STRINGA VARCHAR(100) NULL
- SAGA                 STRINGA VARCHAR(30) NULL
- MULTIPLAYER          NUMBER TINYINT(BOOL) NULL
- LINGUE               STRINGA VARCHAR(30) NULL
- DATA_CREAZIONE_ITEM  DATA DATETIME NOTNULL
- ULTIMA_MODIFICA_ITEM DATA DATETIME NOTNULL
