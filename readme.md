# Декоратор переменной $arResult
## Пример использования

### Обращение к ключам массива как к полям объекта

```php
<?
$arResult = new \Icewood\Nedvijimost\arResultDecorator($arResult);

echo $arResult->NAME; 


```
Мутаторы. Определение кастумных полей на основании массива arResult

```php
<?

class MyDecorator extends \Icewood\Nedvijimost\ArResultObject{
    
    function getCustomField(){
        return $this->NAME . ' - название элемента';
    }
}

$arResult = new MyDecorator($arResult);

echo $arResult->Custom;


```