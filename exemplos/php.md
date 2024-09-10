# Criando logs no php com a biblioteca monolog

A biblioteca Monolog é uma biblioteca de logging para PHP que fornece uma maneira fácil de adicionar logging às suas aplicações PHP. Para usar a biblioteca Monolog, você precisa primeiro instalá-la usando o gerenciador de pacotes Composer. Você pode fazer isso adicionando a seguinte linha ao seu arquivo *composer.json*:

```
"require": {
    "monolog/monolog": "^2.0"
}
```
Em seguida, execute o comando *composer install* para instalar a biblioteca Monolog.

ou se você preferir execute o seguinte comando:

```
composer require monolog/monolog
```

Uma vez instalada a biblioteca Monolog, você pode usá-la em sua aplicação PHP da seguinte maneira:


```
<?php

// Carregue o autoloader do Composer
require_once __DIR__ . '/vendor/autoload.php';

// Crie um novo registrador de log usando a biblioteca Monolog
$log = new Monolog\Logger('meu-registrador');

// Adicione um manipulador de log que escreva os logs em um arquivo
$log->pushHandler(new Monolog\Handler\StreamHandler('app.log', Monolog\Logger::WARNING));

// Adicione um log de aviso
$log->addWarning('Um aviso foi gerado');

// Adicione um log de erro
$log->addError('Um erro foi gerado');

```

Isso irá criar um novo registrador de log chamado "meu-registrador" e adicionar um manipulador de log que escreva os logs em um arquivo chamado "app.log". Em seguida, o código adiciona um log de aviso e um log de erro usando os métodos addWarning e addError, respectivamente.

Você também pode adicionar outros manipuladores de log, como um manipulador que envie os logs para um servidor de log remoto ou um manipulador que envie os logs por e-mail. 

Para obter mais informações sobre como usar a biblioteca Monolog, consulte a documentação do [Monolog](https://github.com/Seldaek/monolog).