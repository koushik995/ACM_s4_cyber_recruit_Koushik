# Challenge Description

So last time I went to this place with my friend i ate in a restaurant which was opened in 1980. We ate chicken biryani in the ground floor of that restaurant. I don’t remember the price, can you find out? 
Flag format: ACM{} 
Author: g4l3na

---

# Analysis / Approach

When I first read the challenge, I carefully noted that, Restaurant was opened in 1980, Ate chicken biryani on the ground floor, Went with a friend, An image was provided as Clue

The first thing I did was focus on the image, because in OSINT challenges, images usually contain the main hint.

Step 1 :- Reverse search the image
I Google searched the clue image to identify the location.
From the architecture and surroundings, it clearly matched the Charminar area in Hyderabad.Then I zoomed in for visible signboards in the image. That helped narrow down possible restaurants in that area.

Step 2 :- Using “Opened in 1980” clue
Instead of guessing randomly, I used the 1980 establishment year as a filter.
I searched for the Restaurants near Charminar established in 1980
That led me to "Hotel Shadab". Hotel Shadab is Located near Charminar, Established in 1980, Famous for biryani, has ground floor dining
All clues matched upto here.

Step 3 :- Finding chicken biryani price
Next, I checked the online menu card for Hotel Shadab.

From the verified menu listing, there are many types of Chicken Biriyani's, the price of SP Chicken Biryani is Rs.265, that was matched with me.
In The question it is said that “I don’t remember the price”
So it is asking for the price of the dish, which is Rs.265

---

# Tools or Commands Used

Google Image Search (reverse image search)
Google search (about restaurant establishment, filtered results using the 1980 clue)
Online menu lookup

---

# Final Flag

ACM{265}
