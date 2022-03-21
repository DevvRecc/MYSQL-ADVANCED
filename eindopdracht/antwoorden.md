# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder

SELECT races.name as race, circuits.name as circuit FROM races JOIN circuits ON circuits.circuitId = races.raceId 

2. Copy paste je gemaakte SQL query hieronder
   
SELECT races.name, drivers.surname as surname, driver_standing.points as points FROM races 
JOIN driver_standing ON driver_standing.raceId = races.raceId
JOIN drivers on driver_standing.driverId = drivers.driverId 
WHERE year = 2017 AND driver_standing.points = 10 ORDER BY drivers.surname DESC

3. Copy paste je gemaakte SQL query hieronder
   
SELECT drivers.forename, drivers.surname, pitstops.duration FROM drivers
JOIN pitstops ON pitstops.driverId = drivers.driverId
WHERE pitstops.duration < 25.000

4. Copy paste je gemaakte SQL query hieronder
   
SELECT constructors.name as constructor, races.name as GrandPrix FROM constructors 
JOIN constructor_standing ON constructor_standing.constructorId = constructors.constructorId
JOIN races ON races.raceId = constructor_standing.raceId
WHERE year = 2010 AND constructors.name = 'McLaren'

5. Copy paste je gemaakte SQL query hieronder
   
SELECT circuits.name, circuits.country as country, races.name as GrandPrix, drivers.surname FROM drivers
JOIN driver_standing ON driver_standing.driverId = drivers.driverId
JOIN races ON races.raceId = driver_standing.raceId
JOIN circuits ON circuits.circuitId = races.circuitId
WHERE races.year = 1950 AND drivers.surname LIKE 'F%'