# Assignment 3 - Writeup

Assignment 3 is all about creating this natural language query system.  In order to do so, you have to write a lot of functions to retrieve infomation.  You will also have to write a function to return answers from a pattern-action list.  There is a lot of work to accomplish in this assignment, but this portion is intended for you to write about what you accomplished.

## Reflection Questions
1. In your own words describe the `search_pa_list` function.

The search_pa_list function takes in what the user says, goes through all scenarios it knows (stored in the pa_list variable) and tries to match it to one of them. If it cannot find a suitable solution, it will iterate through all scenarios then tell the user that it didn't understand what they were asking. If it finds a suitable pattern, it will go to the function associated with that pattern and return whats found to the user. With a longer set of patterns in pa_list, the function will have a higher chance of understanding what the user was asking.

2. What movie did you add to the `movies.py` file?  What year was it made? Any specific reason you added that movie?

I added Hum Aapke Hain Koun, as it is one of my favorite bollywood movies that I watched a lot as a kid. It was made in 1994.

3. What pattern / action did you add to the paList data structure?  Why do you think that is a useful pattern / action?

I added a genre to each movie (I asked ChatGPT to add it to all of them so I can't 100% attest to the validity of all the genres. I did this so I didnt have to hand write a bunch of genres) and added an action and pattern to a3.py to search for these genres and return the title of the movie to the user. The pattern is (str.split("what movies are a _"), title_by_genre) so somebody could say, "What movies are a romance?" and get back the answer "flirting".

4. What is chatbot would you create that would be like this?  Describe why you would create it and what it would do.

I would like to create a more conversational chatbot, which goes in more layers than this one. This one, you ask a question and it gives you an answer, one layer. I would like to make one where if you ask it a question, it can ask you follow up questions etc. and have a full conversation. It could be about anything, I just want to explore this multi-dimensional aspect and how it would work.

5. What was the most difficult portion of this assignment?

The most difficult portion was the search_pa_list function, as I first tried to hardcode the scenarios using the tupples, but then I realised I could just iterate through the tupples and see when the pattern worked. My next issue was calling the function through the tupple, as I had pa_list[i][1] completely forgetting to pass in an argument like pa_list[i][1](match(pa_list[i][0], src)). I managed to figure out this was my problem through many print statements, as I thought it was a logic problem before I added the print statements.

6. Did you write a new assert for your pattern action?

Yes, I wrote one for my new action and it passed the assert.

