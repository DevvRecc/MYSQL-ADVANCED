# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   
SELECT name, platform, genre FROM game JOIN platform ON platform.id = game.platform_id JOIN genre ON genre.id = game.genre_id WHERE name LIKE 'b%'

2. Copy paste je gemaakte SQL query hieronder

SELECT name, platform, publisher, year FROM game JOIN platform ON platform.id = game.platform_id JOIN publisher ON publisher.id = game.publisher_id WHERE year LIKE 2013

3. Copy paste je gemaakte SQL query hieronder

SELECT name, genre, year, global_sales FROM game JOIN genre ON genre.id = game.genre_id WHERE genre.id = 5 OR year > 2000

4. Copy paste je gemaakte SQL query hieronder

SELECT name, platform, year, genre, publisher, jp_sales FROM game JOIN platform ON platform.id = game.platform_id JOIN genre ON genre.id = game.genre_id JOIN publisher on publisher.id = game.publisher_id WHERE name LIKE 'Mario%';

5. Copy paste je gemaakte SQL query hieronder
   
SELECT name, genre, publisher, platform, year FROM game JOIN platform ON platform.id = game.platform_id JOIN genre ON genre.id = game.genre_id JOIN publisher ON publisher.id = game.publisher_id WHERE platform = 'PC'
