# Task 

Create a combat function that takes the player's current health and the amount of damage recieved, and returns the player's new health. Health can't be less than 0.

## Solution with logic (comments)

```
<?php
function combat($health, $damage) {
  if ($health > 0) {
    $newLavelOfHealth = $health - $damage;
    if ($newLavelOfHealth < 0) {
      // If New Level Of Health less then 0 
      return 0;
    } else {
      return $newLavelOfHealth;
    }
  } else {
    return "You are dead";
  }
}

?>
```
