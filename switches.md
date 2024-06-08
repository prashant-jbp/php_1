
## html part
```html
<form action="#" method="POST">
    <label for="d">Input Day Number </label>
    <input type="number" id="d" name="week_day" min="1" max="7"> <br>
    <button type="submit">Submit</button>
</form>
```
```php
<?php
if ($_SERVER['REQUEST_METHOD'] == 'POST') {
    $day = $_POST['week_day'];
    switch ($day) {
        case 1:
            echo " $day is Monday";
            break;
        case 2:
            echo "$day is Tuesday";
            break;
        case 3:
            echo "$day is Wednesday";
            break;
        case 4:
            echo "$day is Thursday";
            break;
        case 5:
            echo "$day is Friday";
            break;
        case 6:
            echo "$day is Saturday";
            break;
        case 7:
            echo "$day is Sunday";
            break;
        default:
            echo "wrong input try again";
            break;
    }
}
```
