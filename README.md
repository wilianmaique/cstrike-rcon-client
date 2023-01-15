# RCON CLIENT
Lib simples para enviar comandos rcon a servidores de cs 1.6.

# Como usar

index.php
```PHP
<?php
require __DIR__ . '/vendor/autoload.php';

use WilianMaique\RconClient\RconClient;

$rcon = new RconClient('177.0.0.0', '123', '27015');

// using the text protocol
echo $rcon->exec('stats');

// using the binary protocol
var_dump($rcon->getInfo());
```