# Video Notları 1-4/tr

### 1. Php Blok İçeriği
   - Php blogunun içeriği, HTML yerine PHP olarak ele alınmalıdır.

### 2. Ui'ya Veri Aktarma İşlemi İçin Farklı Yaklaşımlar
   - İlk adımda, bir değişken oluşturmanız gerekmektedir. Örnek olarak:
     ```php
     $greeting = "Hello";
     ```
   - Daha sonra, "Hello Everyone" ifadesini ekrana yazdırmak için şu yöntemi kullanabilirsiniz:
     ```php
     echo $greeting . " " . "Everyone";
     ```
   - Daha kısa bir yol denemek isterseniz, aşağıdaki kodu kullanabilirsiniz:
     ```php
     echo $greeting . " Everyone";
     ```

### 3. Tek Tırnak ve Çift Tırnak Kullanımı
   - Tek tırnak ve çift tırnak kullanımı arasındaki farkı aşağıdaki örneklerle göz önünde bulundurabilirsiniz:
     - `'$greeting Everyone'` -> Bu şekilde kullanıldığında, değişkeni algılamaz ve ekrana `"$greeting Everyone"` şeklinde yansıtır.
     - `"$greeting Everyone"` -> Çift tırnak kullanıldığında, değişkeni algılar ve ekrana `"Hello Everyone"` olarak yansıtır.