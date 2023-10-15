# Video Notes 5/en

### 1. PHP Blocks and Using Variables in HTML
We can use the following example as a basis for using a variable defined in PHP blocks in HTML:
First, let's create a variable named "name" in the PHP block:

```php
<?php
     $name = "Dark Matter";
?>
```

Then, let's open an h1 tag between the html tags.
Let's open a PHP tag and write the name variable into the block.

```php
<h1>You have read "<?php echo $name; ?>
```

### 2. How Do We Define Conditional Statements?

Let's assume that you get the information whether the user has read the book "Dark Matter" as a boolean value from the database. If the user has read the book, we want to print "You have read Dark Matter" on the screen, if not, we want to show the message "You have NOT read Dark Matter".

The code uses these variables:
- `name` for the book name,
- `read` variable is defined for the reading information of the book.

Then, if-else conditions are used to edit the message based on the boolean (true/false) value of the `read` variable. If `read` value is true, it displays the message "You have read $name". If false, it displays the message "You have NOT read $name". PHP code that performs this operation:

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

### 3. Alternative Use of the Expression ECHO"

`<?php echo $name; in the code. Shortened form of ?>`, `<?= $name; It is in the form ?>`.

This short notation serves the same function and prints the value of the variable directly to the screen.

### 4. Use of Semicolons

`<?php echo $name; The semicolon in ?>` is used to terminate PHP code after displaying the variable with `echo`.

Adding a semicolon can be a good idea to get into the habit of ending the statement, but it is optional. Adding semicolons can help make code more readable and organized.