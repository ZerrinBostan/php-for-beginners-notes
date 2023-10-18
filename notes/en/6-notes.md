# Video Notes 6/en

### 1. Arrays

```php
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
</head>

<body>
    <?php

    // Let's store our books in a PHP array.
    $books = [
        "Do Androids Dream of Electric Sheep",
        "The Langoliers",
        "Hail Mary",
    ];
    ?>

    <ul>
        <?php

        // In PHP, the foreach loop iterates over an array and processes each element sequentially.
        // Here, we use the foreach loop to list the books.

        /*
          ┌─────────────────────────────────────────────────────────────────────────────┐
          │         foreach ($books as $book) {                                         │
          │             // Method 1: Printing the book name using "echo"                │
          │             echo "<li>" . $book . "</li>";                                  │
          │                                                                             │
          │             // Method 2: Printing the book name using short syntax          │
          │             echo "<li>{$book}™ </li>";                                      │
          │                                                                             │
          │             // Method 3: Displaying books in a more complex structure       │
          │             echo "<li><div>{$book}™</div></li>";                            │
          │         }                                                                   │
          │         ?>                                                                  │
          └─────────────────────────────────────────────────────────────────────────────┘
         */

        // Alternative method
        foreach ($books as $book): ?>
            <li>
                <?= $book ?>
            </li>
        <?php endforeach; ?>
    </ul>
</body>

</html>

```
