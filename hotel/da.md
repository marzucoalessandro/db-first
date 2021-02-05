Provare a strutturare il seguente database che modellizza un hotel: Ci sono varie stanze, ognuna con le proprie caratteristiche. Le diverse stanze vengono prenotate per periodi di tempo, da ospiti. Ad ogni prenotazione devono essere associati tutti gli ospiti della stanza.
Nella repo mettete sia il file del diagramma che il file esportato come immagine.

nome database: Hotel;

TABLE: STANZE
ROW:
-ID          NUMERO TINYINT PRIMARYKEY NOTNULL
-TIPOLOGIA   STRINGA VARCHAR(50) NOTNULL
-PREZZO      NUMERO FLOAT(5, 2) NOTNULL
-DESCRIZIONE STRINGA TEXT NOTNULL
-LETTI       NUMERO TINYINT NOTNULL
-FOTO        STRINGA VARCHAR(50) NOTNULL


TABLE: OSPITE
ROW:
-ID           NUMERO INT PRIMARYKEY NOTNULL
-ID STANZE    
-NOME         STRINGA VARCHAR(30) NOTNULL
-COGNOME      STRINGA VARCHAR(30) NOTNULL
-DOC_IDEN     STRINGA VARCHAR(30) NOTNULL
-C_FISCALE    STRINGA VARCHAR(20) NOTNULL
-INDIRIZZO    STRINGA VARCHAR(30) NOTNULL
-CITTA'       STRINGA VARCHAR(30) NOTNULL
-CAP          NUMBER TINYINT NULL
-PERIODO      DATA DATE NOTNULL


TABLE: PERIODO

ROW:
-ID         NUMERO INT PRIMARYKEY NOTNULL
-ID STANZE
-ANNO       DATA DATE NOTNULL
-MESE       DATA DATE NOTNULL
-GIORNO     DATA DATE NOTNULL
