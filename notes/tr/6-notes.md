# Video Notes 6/tr

### 1. Arrays
```php
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
</head>

<body>
    <?php

    // Kitaplarımızı bir PHP dizisinde saklayalım.
    $books = [
        "Do Androids Dream of Electric Sheep",
        "The Langoliers",
        "Hail Mary",
    ];
    ?>

    <ul>
        <?php

        // PHP'de foreach döngüsü, bir diziyi ele alır ve her öğeyi sırayla işler.
        // Burada kitapları listelemek için foreach döngüsünü kullanıyoruz.
        
        /* 
          ┌─────────────────────────────────────────────────────────────────────────────┐
          │         foreach ($books as $book) {                                         │
          │             // 1. Yöntem: "echo" kullanarak kitap adını yazdırma            │
          │             echo "<li>" . $book . "</li>";                                  │
          │                                                                             │
          │             // 2.Yöntem: Kitap adını kısa yazım ile ekrana yazdırma         │
          │             echo "<li>{$book}™ </li>";                                      │
          │                                                                             │
          │             // 3. Yöntem: Kitapları daha karmaşık bir yapı içinde gösterme  │
          │             echo "<li><div>{$book}™</div> </li>";                           │
          │         }                                                                   │
          │         ?>                                                                  │
          └─────────────────────────────────────────────────────────────────────────────┘
         */

        // Alternatif yöntem
        foreach ($books as $book): ?>
            <li>
                <?= $book ?>
            </li>
        <?php endforeach; ?>
    </ul>
</body>

</html>
```