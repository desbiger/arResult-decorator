# ��������� ���������� $arResult
## ������ �������������

### ��������� � ������ ������� ��� � ����� �������

```php
<?
$arResult = new \Icewood\Nedvijimost\arResultDecorator($arResult);

echo $arResult->NAME; 


```
��������. ����������� ��������� ����� �� ��������� ������� arResult

```php
<?

class MyDecorator extends \Icewood\Nedvijimost\ArResultObject{
    
    function getCustomField(){
        return $this->NAME . ' - �������� ��������';
    }
}

$arResult = new MyDecorator($arResult);

echo $arResult->Custom;


```