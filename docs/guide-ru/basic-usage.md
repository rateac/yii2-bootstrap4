Базовое использование
===========

Yii не оборачивает базовый Bootstrap в PHP код, поскольку HTML, в этом случае, прост сам по себе. Вы можете найти подробную информацию об использовании на [сайте документации bootstrap](http://getbootstrap.com/css/). Тем не менее, Yii обеспечивает удобный способ включения bootstrap assets на ваших страницах добавленим одной строки в `AppAsset.php` расположенной в вашей `@app/assets` директории:

```php
public $depends = [
    'yii\web\YiiAsset',
    'yii\bootstrap4\BootstrapAsset', // this line
];
```

Использование загрузки Bootstrap через Yii asset manager позволяет минимизировать ресурсы и объединить с вашими собственными ресурсами, когда это будет необходимо.