# my2-Nakka
# Nakka Sai Teja Goud
###### My favorite spot is vizag.
**Beaches** are one of my favorite goto places and having large **forest** area and caves add more beauty to vizag

****
# My favorite 3 activities in Vacation Spot
    1. Trecking
    2. Dance
    3. Cooking favorite food
    
    List of dishes i get at vacation spot
    * Chicken
    * Fish

click here for my personal details and image <MyStats.md>
***

# Recommending best 4 types of sports 
Here are some of best 4 sports game that makes our life better.
|Name|Reason of reccomendationn|Total hours spent|
|-------|---------:|--------|
|Badminton|Increases flexibility|1 |
|Cricket|Learns Cordination|1|
|Foot ball|Makes you Strong|1|
|Chess|Increases intelligence|1|

***
# 2 PITHY QUOTES BY SCIENTISTS
> "Science is a way of thinking much more than it is a body of knowledge" -*Carl Sagan*

> "Science knows no country, because knowledge belongs to humanity, and is the torch which illuminates the world." - *Louis Pasteur*
# How to add points to a logged-in user after reading a QR code (URL) with MyCred and WordPress
Here is the relevant question on Stack Overflow: [Link to Stack Overflow Question](https://stackoverflow.com/questions/77021074/how-to-add-points-to-a-logged-in-user-after-reading-a-qr-code-url-with-mycred)

``` function set_mycred_points($point, $pass) {
    // Define the correct passcode
    $correct_pass = "thecustompassword";

    // Check if the passcode is correct
    if ($pass !== $correct_pass) {
        wp_redirect('/qr-error/'); 
        exit; // Make sure to exit to prevent further execution
    }

    $user_id = get_current_user_id();
    $today = date('Y-m-d');

    // Get the date when the user last performed the action
    $last_performed_date = get_user_meta($user_id, 'mycred_last_performed_date', true);

    if ($last_performed_date != $today) {
        // User has not performed the action today, so add points
        mycred_add('Store Visit Points', $user_id, $point, 'Earned Store Visit Points');

        // Update the date when the user last performed the action
        update_user_meta($user_id, 'mycred_last_performed_date', $today);
    } else {
        // User has already performed the action today, redirect to a specific page
        wp_redirect('/point-error/'); 
        exit; // Make sure to exit to prevent further execution
    }
}

if (isset($_GET['action']) && $_GET['action'] == 'setpts' && isset($_GET['point']) && isset($_GET['pass'])) {
    $point = intval($_GET['point']); // Sanitize the point value as an integer
    $pass = $_GET['pass']; // Get the passcode from the GET parameters
    set_mycred_points($point, $pass);
}
```


Here is the quick link for the snippets source:  [link](https://css-tricks.com/new-snippet-buttons/)