# is120-project1-Spencer-Kimball

** HW 7 - CSS Responsive Design Readme **

I am choosing project 1's index.html to make responsive. And it was made with the mobile version first approach for project 1, so now I am going to make it responsive for a desktop version. The original_index.html is the file unaltered for easy reference to see how the web pages differ. The original was stacked cards that didn't change their position based on the widening of the screen. Now I am hoping to change this html to make the cards go into a row position after some breakpoint. 

Attempting to add a body container class for the responsive aspect for my 3 main cards.

**What changes you made (media queries, any other restructuring to the existing code)**

Added the book favicon which looks good while you are on the page, but if you go to a different tab it has a weird square border around it even though I have already removed the background from the image.

I tried adding the "grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); " line of code for my body container class and it made it look AWFUL for the desktop version. On the original I have this cute little button called "top" at the bottom of the page, and including the repeat auto fit made the top button as big as the regular cards, and it changed to so many different widths as the screen size widened.

Top button is irrelevent once the cards are aligned as a row for the desktop view. The top button didn't need to be in the container for the cards, so taking that out of the container fixed the issues with the top button.

The option 2 card is going off the view width so then you have to side scroll for some reason. And they aren't evenly spaced in the center. The first card is smushed up against the left side of the screen. And there are huge gaps between each of the cards inside of the container.

Having width: 100vw; and grid-template-columns: repeat(auto-fit); helped get it back to be mobile version friendly, but no longer putting them next to each other in a row.

**Justify why you picked the custom breakpoints that you did. Look up Tailwind and Bootstrap standard breakpoints, are yours similar at all?**
**If you had to build this page differently at the start to make it more responsive, what would you have done?**


























** Project 1 Readme **

**Brief Description of my project:**

My wife has a book binding hobby and she makes these as gifts for people for birthdays or baptisms.
I think she does a really good job and makes it look great. I have also seen other people's websites
that charge crazy amounts for custom bound books. This website is an initial attempt at building
a website for her start up business to create custom bound books.



**Problems I ran into:**

I used the property that we learned in HW 5 to add a notification icon onto my shopping
cart navigation button. As of right now it is a permanent 1 with a circle around it
since I don't know how to create a counter that increases as a user clicks on the 
add to cart buttons for the different products listed on the page.

I learned about the format of the border-radius option of css. That 4 border-radius
options are altering the rounding angle for each of the corners of whatever you are
creating a class for. So if the line is border-radius: 12px 12px 12px 12px; every
single corner is being rounded to the same angle. Where as if you have 
border-radius: 12px 12px 0 0; this is only rounding the top two corners.

I struggled while trying to make the checkout page and adding things to the cart. It looks like
that will include javascript or something like that. Basically anywhere on the page
that I want to get input from what the user is doing on the page can't be done using
just html and css.

The design and layout of this website I was hoping to be more mobile friendly with the skinnier group of cards. 
I did this by stacking them on top of each other instead of in-line at least for the main page.
I think my product pages still may not be very mobile friendly since those are made in-line
with each other.

I have been struggling to find where I would use id tags where it would need to be a unique tag
and therefore could only be used in one spot. Most of the tags that I have created are pretty 
versatile across the website and therefore made more sense to be used as a class instead of 
an id tag. However, I found that adding a TOP button on the bottom of the main page is a good
example of something that could use a unique tag since it will only be used in that one spot.

Another thing that I definitely need to improve on is organizing my css file and naming
my classes better. As of right now, as I am working on an html page if I want to add a different
color for text or a card, I copy and paste a different card that was close to what I wanted,
paste it and make the minor edit. This approach has made my css code long and hard to navigate.

Struggled to center a div, and finally got the answer after trying for 30 minutes.
I now have a better understanding of those memes where there is such a small fraction
of people who know how to center a div.