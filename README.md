camper: /project$ psql --username=freecodecamp --dbname=postgres
Border style is 2.
Pager usage is off.
psql (12.17 (Ubuntu 12.17-1.pgdg22.04+1))
SSL connection (protocol: TLSv1.3, cipher: TLS_AES_256_GCM_SHA384, bits: 256, compression: off)
Type "help" for help.

postgres=> \c universe
SSL connection (protocol: TLSv1.3, cipher: TLS_AES_256_GCM_SHA384, bits: 256, compression: off)
You are now connected to database "universe" as user "freecodecamp".
universe=> INSERT INTO asteroid (name, galaxy_id, diameter, mass, is_metallic, is_hazardous) VALUES
universe-> ('Ceres', 1, 946, 10, FALSE, FALSE),
universe-> ('Vesta', 1, 525, 10, TRUE, FALSE),
universe-> ('Pallas', 1, 544, 10, FALSE, FALSE),
universe-> ('Hygiea', 1, 434, 10, FALSE, FALSE),
universe-> ('Juno', 1, 247, 10, FALSE, FALSE);
INSERT 0 5
universe=> INSERT INTO moon (name, planet_id, diameter, mass, orbital_period, has_rings) VALUES
universe-> ('Moon', 3, 3474, 7.342, 27.32, FALSE),
universe-> ('Phobos', 4, 22.2, 10, 0.3189, FALSE),
universe-> ('Deimos', 4, 12.6, 10, 1.2624, FALSE),
universe-> ('Io', 5, 3643, 10, 1.769, FALSE),
universe-> ('Europa', 5, 3122, 10, 3.551, FALSE),
universe-> ('Ganymede', 5, 5268, 10, 7.154, FALSE),
universe-> ('Callisto', 5, 4821, 10, 16.689, FALSE),
universe-> ('Titan', 6, 5149, 10, 15.945, TRUE),
universe-> ('Rhea', 6, 1528, 10, 4.518, FALSE),
universe-> ('Iapetus', 6, 1469, 10, 79.33, FALSE),
universe-> ('Dione', 6, 1123, 10, 2.737, FALSE),
universe-> ('Tethys', 6, 1062, 10, 1.888, FALSE),
universe-> ('Enceladus', 6, 504, 10, 1.370, FALSE),
universe-> ('Mimas', 6, 396, 10, 0.942, FALSE),
universe-> ('Ariel', 7, 1158, 10, 2.520, FALSE),
universe-> ('Umbriel', 7, 1169, 10, 4.144, FALSE),
universe-> ('Titania', 7, 1577, 10, 8.706, FALSE),
universe-> ('Oberon', 7, 1523, 10, 13.463, FALSE),
universe-> ('Triton', 8, 2707, 10, 5.877, FALSE),
universe-> ('Nereid', 8, 340, 10, 360.13, FALSE);
INSERT 0 20
universe=> ALTER TABLE galaxy ADD COLUMN kocka INT;
FATAL:  terminating connection due to administrator command
SSL connection has been closed unexpectedly
server closed the connection unexpectedly
        This probably means the server terminated abnormally
        before or while processing the request.
The connection to the server was lost. Attempting reset: Succeeded.
SSL connection (protocol: TLSv1.3, cipher: TLS_AES_256_GCM_SHA384, bits: 256, compression: off)
universe=> ALTER TABLE galaxy ADD COLUMN kocka INT;
ALTER TABLE
universe=> ALTER TABLE galaxy ADD COLUMN kocka1 INT;
ALTER TABLE
universe=> 
