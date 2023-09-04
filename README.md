# my2-Nakka
# Nakka Sai Teja Goud
###### My favorite spot is vizag.
**Beaches** are one of my favorite goto places and having large **forest** area and caves add more beauty to vizag.

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
|Badminton:|Increases flexibility:|1 |
|Cricket:|Learns Cordination:|1|
|Foot ball:|Makes you Strong:|1|
|Chess:|Increases intelligence:|1|

***
# 2 PITHY QUOTES BY SCIENTISTS
> "Science is a way of thinking much more than it is a body of knowledge" -*Carl Sagan*

> "Science knows no country, because knowledge belongs to humanity, and is the torch which illuminates the world." - *Louis Pasteur*
# How to add points to a logged-in user after reading a QR code (URL) with MyCred and WordPress
Here is the relevant question on Stack Overflow: [Link to Stack Overflow Question](https://stackoverflow.com/questions/77021074/how-to-add-points-to-a-logged-in-user-after-reading-a-qr-code-url-with-mycred)
``` $("pre").each(function() {
    $preblock = $(this);
    $codeblock = $preblock.find("code");
    $snippets_link = "snippet:add?code=" + encodeURIComponent($codeblock.text()) + "&name=" + $title + "&relatedurl=" + encodeURIComponent(document.location.href);
    $("<a class='snippet-button'>Add to Snippets.app</a>").attr("href",$snippets_link).appendTo($preblock);         
}); 
```


Here is the quick link for the snippets source [link](https://css-tricks.com/new-snippet-buttons/)