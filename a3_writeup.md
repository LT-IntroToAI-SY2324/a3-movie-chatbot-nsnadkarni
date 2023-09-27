# Assignment 3 - Writeup

Assignment 3 is all about creating this natural language query system.  In order to do so, you have to write a lot of functions to retrieve infomation.  You will also have to write a function to return answers from a pattern-action list.  There is a lot of work to accomplish in this assignment, but this portion is intended for you to write about what you accomplished.

## Reflection Questions
1. In your own words describe the `search_pa_list` function.

The search_pa_list function takes in what the 

2. What movie did you add to the `movies.py` file?  What year was it made? Any specific reason you added that movie?

I added Hum Aapke Hain Koun, one of my favorite bollywood movies that I watched a lot as a kid

3. What pattern / action did you add to the paList data structure?  Why do you think that is a useful pattern / action?

I added (str.split("in what movies did % act"), title_by_actor) and (str.split("in what movies did % act in"), title_by_actor), so somebody could write "In what movies did Spike Lee act" or "In what movies did Spike Lee act in". I feel like this is useful as (str.split("in what movies did % appear"), title_by_actor), the previous title_by_actor, would not be frequently used as 

4. What is chatbot would you create that would be like this?  Describe why you would create it and what it would do.


5. What was the most difficult portion of this assignment?


6. Did you write a new assert for your pattern action?

Yes, I wrote one for both.

