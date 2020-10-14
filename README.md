Thai Words Split Lib
==========

Lib ตัดคำภาษาไทย สำหรับ PHP ทดลองใช้กับ MPDF


การใช้งาน:
```php
    $words = $segment->get_segment_array($text);
    $text = implode("|",$words);
```


Config: 
```php
    $mpdf->useDictionaryLBR = false;
```

Edit Mpdf.php ค้นหา `3) Break at SPACE`:
```php
    if ($prevchar == '|') {
        $breakfound = [$contentctr, $charctr, $cutcontentctr, $cutcharctr, 'discard'];
    }
```
    
    
    
