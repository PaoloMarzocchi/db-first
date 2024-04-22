### Traccia

Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.


# DATABASE

DB_NAME: cars_dealer

Table name: used_cars

ID  
Data immatricolazione           
Vin 
Numero di telaio 
Targa veicolo 
Marca
Modello
Alimentazione
Cilindrata
Prezzo
Km percorsi
N° porte
N° posti
Consumi
Mano
Cambio
N° marce
Descrizione
Peso
Foto
Colore
Capienza bagagliaio



- `id` | NOTNULL | UNIQUE | BIGINT
- `registration_date` | NOTNULL | DATE | DEFAULT('YYYY/MM/DD')
- `vin` (Vehicle Identification Number) | NOTNULL | UNIQUE
- `vehicle_plate` | NULL | UNIQUE | CHAR(7)
- `brand` | NOTNULL | VARCHAR(30) | DEFAULT('Car Brand')
- `model` | NOTNULL | VARCHAR(50) | DEFAULT('Car Model')
- `fuel` | NULL | VARCHAR(20)
- `displacement` | NULL | SMALLINT
- `price` | NULL | MEDIUMINT
- `mileage` | NULL | MEDIUMINT
- `doors_number` | NULL | TINYINT
- `seats_number` | NULL | TINYINT
- `fuel_consumption` | NULL | VARCHAR(20)
- `ownership` | NULL | VARCHAR(20)
- `transmission` | NULL | VARCHAR(20)
- `gears_numb` | NULL | TINYINT
- `weight` | NULL | SMALLINT
- `photos` | NULL | VARCHAR(255)
- `color` | NULL | VARCHAR(20)
- `cargo_capacity` | NULL | VARCHAR(20)
- `description` | NULL | TEXT