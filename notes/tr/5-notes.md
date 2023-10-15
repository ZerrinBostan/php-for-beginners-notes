# Video Notları 5/tr

### 1. PHP Blokları ve HTML'de Değişken Kullanımı
PHP blokları içinde tanımlanan bir değişkenin HTML içinde kullanmak için aşağıdaki örneği baz alabiliriz:
ilk önce PHP bloğunda "name" adında bir değişken oluşturalım:

```php
<?php 
    $name = "Dark Matter";
?>
```

Ardından html etikleri arasına h1 tagi açalım.
Php tagi açarak blok içerisine name değişkenini yazalım.

```php
<h1>You have read "<?php echo $name; ?>
```

### 2. Koşullu İfadeleri Nasıl Tanımlarız? 

Kullanıcının "Dark Matter" kitabını okuyup okumadığı bilgisini veri tabanından bir boolean değer olarak aldığınızı düşünelim. Eğer kullanıcı kitabı okuduysa ekrana "You have read Dark Matter" yazdırmak, okumadıysa "You have NOT read Dark Matter" mesajını göstermek istiyoruz.

Kod şu değişkenleri kullanır:
- Kitap ismi için `name`,
- Kitabın okunma bilgisi için `read` değişkeni tanımlanır.

Ardından, `read` değişkeninin boolean (true/false) değerine göre mesajı düzenlemek için if-else koşulları kullanılır. Eğer `read` değeri true ise, "You have read $name" mesajını gösterir. Eğer false ise, "You have NOT read $name" mesajını gösterir. bu işlemi gerçekleştiren PHP kodu:

```php
<?php
$name = "Dark Matter";
$read = false;

if ($read) {
    $message = "You have read $name";
} else {
    $message = "You have NOT read $name";
}
?>

<h1>
    <?php echo $message; ?>
</h1>
```

### 3. ECHO İfadesinin Alternatif Kullanımı

Kod içindeki `<?php echo $name; ?>` kullanımının kısaltılmış hali, `<?= $name; ?>` şeklindedir. 

Bu kısa gösterim, aynı işlevi görür ve değişkenin değerini direkt olarak ekrana yazdırır.

### 4. Noktalı Virgül Kullanımı

`<?php echo $name; ?>` içindeki noktalı virgül, değişkeni `echo` ile görüntüledikten sonra PHP kodunu sonlandırmak için kullanılır. 

Noktalı virgül eklemek, ifadeyi sonlandırma alışkanlığı kazandırmak açısından iyi bir fikir olabilir, ancak isteğe bağlıdır. Noktalı virgül eklemek, kodun daha okunaklı ve düzenli olmasına yardımcı olabilir.

