Модуль комментариев для Yii2
============================
Позволяет пользователям оставлять комментарии

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist reketaka/yii2-comments "*"
```

or add

```
"reketaka/yii2-comments": "*"
```

to the require section of your `composer.json` file.

* Выполнить миграцию для создания нужной таблицы в базе данных (консоль):
```
yii migrate --migrationPath=@reketaka/comments/migrations --interactive=0
```

Usage
-----
```php
<?=\reketaka\comments\widgets\CommentListWidget::widget([
    'model'=>$item
])?>

<?=\reketaka\comments\widgets\CommentFormWidget::widget([
    'model'=>$item
])?>