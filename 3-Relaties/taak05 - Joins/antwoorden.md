# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   
SELECT game.name, platform.platform FROM game JOIN platform

2. Copy paste je gemaakte SQL query hieronder
   
SELECT game.id, game.name FROM game WHERE game.id < 11;

3. Copy paste je gemaakte SQL query hieronder
   
SELECT game.name, platform.platform FROM game JOIN platform WHERE name = 'Call of Duty: Advanced Warfare'

4. Copy paste je gemaakte SQL query hieronder
   
SELECT platform, name FROM game JOIN platform WHERE name LIKE 'FIFA%'
   
5. Copy paste je gemaakte SQL query hieronder

SELECT platform.platform, game.name FROM game JOIN platform WHERE name = 'Borderlands' OR name = 'Borderlands 2';