Yii2 Expo Push Notifications
=========
Yii2 extension for working with Expo push notifications

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist open20/amos-expo "*"
```

or add

```
"open20/amos-expo": "*"
```

to the require section of your `composer.json` file.


Config
------

Once the extension is installed, add it to your config file(main.php)  :

```
'expo' => [
            'class' => 'open20\expo\ExpoPush'
        ],
```

Usage
-----
```
$data = [
    'title' => 'Some title',
    'text' => 'Some text'
];
$notification = ['body' => $text, 'data' => $data];
\Yii::$app->expo->notify('ExponentPushToken[xxxxxxxxxxxxx]', $notification);
```  
`$data` is optional
