<?php
// Function to determine age based on date of birth
function calculateAge($dob) {
    $dob = new DateTime($dob);  // Convert the input string into a DateTime object
    $today = new DateTime('today');  // Get the current date
    $age = $dob->diff($today)->y;  //Calculate the difference in years between the two dates
    return $age;
}

// Provided values for input
$name = "    Ariho Ronald";
$dob = "8-12-2004";  
$address = "  Rukiga";

// Determine the age.
$age = calculateAge($dob);

// Display a message.
echo "$name, Welcome home!\n";
echo "Your address is: $address\n";
echo "You are $age years old!\n";
?>

