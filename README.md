# CAPSTONE BAYESIAN OPYIMISATION PROJECT

My approach to this challenge was split into phases. Using a combination of exploration and exploitation.

## PHASE 1:
In the first week I very much focused on Exploration. I decided to use 3 of my guesses to search the space a far as I could. To achieve this I wrote my own function that would generate many random point in the search space (100,000). I then worked out the Euclidean distance of each point to the existing points and chose the one that was furthest away from the others. I did this 3 times.
At this point I had a few lucky guesses that put me near the top of the tables.
I used one file per function and they were identical except for the different dimensions.

## PHASE 2:
In the second week I employed some more conventional techniques that I had learned during the course. These were Upper Confidence Bound and Probability of improvement.
I wrote functions for both of these and generated some guesses along with some more ‘faraway’ random guess (using the function above’ to explore the space)
These functions only improved my maximisation values slightly.

## PHASE 3:
At this point in the competition I switched into ‘Lazy Bones’ mode, and started to look for code that I could modify for my purposes.
I found an optimisation package called ‘scikit-optimize’. I utilised the packages, and code, to develop a function to give me my next guess. 
Because the optimizer used in the package was one for minimisation problems. I flipped the Y-data with a minus sign to turn a maximisation problem into a minimisation problem.
The application of these functions helped me improve my maximisation of most functions.
I adopted this strategy for a few weeks.

## PHASE 4:
In this last phase I was made aware of another optimisation package by our instructor. This was Trust Region Bayesian Optimization.
This package was quite difficult to understand and implement, but I was able to finally implement it.
At this stage I combined all functions into one file. I wrote some code around the packages to take the input data straight from the excel file, perform the optimisation and return the guesses to be inputted directly into the Google form. At this point some new data was also released.
I used this strategy until the end of the competition.

## SUMMARY:
Overall I felt, as a beginner, I didn’t do to badly.
I know that it wasn’t a true competition, but I was proud to have been hovering just outside the top 10 for the competition.
I felt that because I was still grappling with the coding and general concepts I wasn’t able to fully optimise my code for each function.

## FURTHER WORK & REFLECTIONS:
As I said I am happy with my submission and I learnt about the power of Bayesian optimisation. I was still getting to grips with the coding and concepts to fully optimise the functions. Some things I would have improved or done differently are:
- Stopped maying so many random guesses at the beginning and started using some optimisation functions sooner.
- Searching for different optimisation functions. I used the same optimisation strategy for each function. However, some of the functions that we were trying to maximise were quite different. E.g. some were noisy, some were sparce, etc. Therefore, I would have looked at what other strategies could have suited each function individually.


