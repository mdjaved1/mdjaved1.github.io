---
layout: post
title: BlocJams
feature-img: "img/sample_feature_img.png"
thumbnail-path: "https://d13yacurqjgara.cloudfront.net/users/3217/screenshots/2030966/blocjams_1x.png"
short-description: Blocjams is a music application , made as a practice project.

---
This is an example of a post which includes a feature image specified in the front matter of the post. The feature image spans the full-width of the page, and is shown with the title on permalink pages.
# Blocjams
## Blocjams is a music api made to practice Html and Javascript
### The following are the main issues i encountred while creating Blocjams and how i solved them :
1. While creating bloc jams i ran into an issue where the site would load zoomed out and the text would shrink if viewd on a mobile site , i fixed this issue by using a viewport tag which scales the page to fit the width .
2. While creating the nextbutton for the player bar in the music app i ran into a problem where the pause button in the song row would not change with the pause button in the player bar . To fix this issue i had to make sure all three of my player bar functions used the playerbar and the song row template that i had previously created.
  {% highlight javascript %}
  var nextSong = function(){

    ....
    $nextSongNumberCell.html(pauseButtonTemplate);
   $lastSongNumberCell.html(lastSongNumber);
  }
 {% endhighlight %}
3. Another problem i encounterd was that the songNumbercell would not update , to solve this problem i converted my string to an int using .
  {% highlight javascript %}

  var songNumber = parseInt(songNumberCell.attr('data-song-number'));

  {% endhighlight %}
4. As this was my practice Porject one of the main issues i faced was spending too much time on the same problem and going down a rabbit hole trying to find it , to resolve this issue i figured it would be best to step away from that one issue work on other parts of the project and come back to it with a fresh prespective .

### In conclusion i learned alot from this project , everything from conpensating for different screen sizes to running code more efficently and faster .
