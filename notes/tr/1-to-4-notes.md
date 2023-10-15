# Video Notes 1-4/en

1. **The Content in the PHP Blog**
   - The content written within the PHP blog should be considered in PHP, not as HTML.

2. **Different Approaches for Transferring Data to UI**
   - In the first step, you need to create a variable. For example:
     ```php
     $greeting = "Hello";
     ```
   - Then, to display the phrase "Hello Everyone" on the screen, you can use the following method:
     ```php
     echo $greeting . " " . "Everyone";
     ```
   - If you want to try a shorter method, you can use the following code:
     ```php
     echo $greeting . " Everyone";
     ```

3. **Single and Double Quotes Usage**
   - You can consider the difference between single and double quotes with the following examples:
     - `'$greeting Everyone'` -> When used in this way, it doesn't recognize the variable and displays `"$greeting Everyone"` on the screen.
     - `"$greeting Everyone"` -> When double quotes are used, it recognizes the variable and displays "Hello Everyone" on the screen.