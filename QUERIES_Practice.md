-- MySQL Functions

-- Text
-- CONCAT()
SELECT CONCAT("Mr.", " ", first_name, " ", last_name) AS full_name FROM clients;
-- CONCAT_WS()
SELECT CONCAT_WS(" ", "Mr.", first_name, last_name) AS full_name FROM clients;
-- LENGTH()
SELECT LENGTH(first_name)  AS f_name_len FROM clients;
-- LOWER()
SELECT LOWER(last_name) AS l_name_lowercase FROM clients;

-- Date
-- HOUR()
SELECT HOUR(joined_datetime) AS date_hour, joined_datetime FROM clients;
-- DAYNAME()
SELECT DAYNAME(joined_datetime) AS day_name, joined_datetime FROM clients;
-- MONTH()
SELECT MONTH(joined_datetime) AS month_number, joined_datetime FROM clients;
-- NOW()
SELECT NOW() AS right_now;
-- DATE_FORMAT()
SELECT DATE_FORMAT(joined_datetime, "%W %D %M, %Y") AS date_joined FROM clients;
