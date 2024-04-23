### Traccia

Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.


# DATABASE

DB_NAME: cars_dealer

Table name: used_cars

- `id` | NOTNULL | UNIQUE | BIGINT| AUTOINCREMENT | PRIMARY KEY
- `registration_date` | NOTNULL | DATE 
- `vin` (Vehicle Identification Number) | NOTNULL | UNIQUE
- `vehicle_plate` | NULL | UNIQUE | CHAR(7)
- `brand` | NOTNULL | VARCHAR(30) 
- `model` | NOTNULL | VARCHAR(50)  
- `fuel` | NULL | VARCHAR(20)
- `displacement` | NULL | SMALLINT
- `price` | NULL | float(7,2)
- `mileage` | NULL | MEDIUMINT
- `doors_number` | NULL | TINYINT
- `seats_number` | NULL | TINYINT
- `fuel_consumption` | NULL | VARCHAR(20)
- `ownership` | NULL | VARCHAR(20)
- `transmission` | NULL | VARCHAR(20)
- `gears_numb` | NULL | TINYINT
- `weight` | NULL | SMALLINT
- `photo` | NULL | VARCHAR(255) | default('image')
- `color` | NULL | VARCHAR(20)
- `cargo_capacity` | NULL | VARCHAR(20)
- `description` | NULL | TEXT