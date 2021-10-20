----------------INSTALLATION-----------------------------

DOCKER 
(you have to be installed docker + docker-compose)
1. Clone this repository from github
2. Create config/local.db.php and copy text below(I do this for another type of installation and for secure work with credentials)
```
<?php

return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=test-db;dbname=test',
    'username' => 'root',
    'password' => 'pass',
    'charset' => 'utf8',
    
];
```
Run script ```make init```

Run script ```make migrations```

Now your host - localhost:8888. If you want to change port - you can edit docker-compose.yml
```
-------------DOCUMENTATION---------------------