**Producto Mercado Vuelos**: 
Estos scripts generan los DDL con sus respectivos tipos de datos

```sql
## Scripts usados para DDL de las tablas de hechos
CREATE TABLE Itinerarios 
(
    Segment_Departure_Date                varchar(256), 
    Segment_Segment_OW                    varchar(256), 
    Segment_Origen                        varchar(256), 
    Segment_Destino                       varchar(256), 
    Operating_Core_Carrier                varchar(256), 
    "Sked_Departure_Local_(HHMM)"         INTEGER,    
    "Sked_Arrival_Local_(HHMM)"           INTEGER,    
    INDSCH_Scheduled_Frequency            INTEGER, 
    INDSCH_Scheduled_First_Cabin_Seats    INTEGER, 
    INDSCH_Scheduled_Economic_Cabin_Seats INTEGER, 
    INDSCH_Scheduled_Business_Cabin_Seats INTEGER 
);

CREATE TABLE mercados 
(
    OD_Flight_Date                 Date, 
    OD_OW                          varchar(256), 
    OD_Path                        varchar(256), 
    Segment_OW                     varchar(256), 
    OD_Operating_Core_Carrier      varchar(256), 
    Segment_Operating_Core_Carrier varchar(256),
    OD_cabin_Name                  varchar(256),
    Segment_Cabin_Name             varchar(256),
    "Scheduled_Departure(HHMM)"    INTEGER,    
    "CO_Elapsed_Time_(Min)"        INTEGER,    
    Lengthy_of_Stay_Band           INTEGER,  
    MIDT_Segment_Pax               INTEGER, 
    MIDT_OD_Pax                    INTEGER
);

```
```python
## Escriba su script aqui
```
