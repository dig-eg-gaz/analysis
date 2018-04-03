---
layout: page
subheadline: "Thomas Wallace"
title: "Shipping in Colonial Egypt"
date: 2018-04-02
author: "ThomasWallace"
header: no
image:
  title:  <!-- for image-name.png, substitute name you've given your image file -->
  thumb:
  homepage:
  caption:
Credit:
  caption_url: <!-- link-to-page-containing-text? -->
---
The Brainstorm
The world in the twenty first century is one that is connected, by the internet, but also by the seas. The world economy is driven in part by the movement of goods across large bodies of water. The twentieth century was no different as this is when shipping people and goods became something that a middle class person could do. As someone with a minor in geography, how people interact with others on a global scale is of great interest to me. When I learned we would be doing a project such as this in the class I knew I wanted to do something with the globalization of trade. This is the era of the steamship, as shown by the plethora of ads showing off the prices of travel. The steamship revolutionized global trade as it opened up new trade routes that were previously unavailable due to wind patterns. As it is quite obvious how important these steamers are, that raises new questions. Where are these ships going and when? What is on these ships, people or cargo, or both? Did the proportion of ships with humans versus cargo change throughout the years? What about the overall volume of ships going back and forth, did that change? These questions are the ones that this analysis seeks to answer. This is a history class, in part at least, and this microhistory blends well into the overall fabric of industrialization of the twentieth century. Each ship makes up a tiny story in the sea of history (pun intended).

Serial Question
All of the questions listed above are relatively specific, considering the scope of the source material. This topic though can be pulled back a bit to find something that can be applied more generally. My goal is to learn how shipping from and to Egypt changed over the three year period in which the Egyptian Gazette is available for research. Unfortunately the findings of this study can't be too intensely generalized to the shipping world in general because of the scope of the Egyptian Gazette. In light of all of this, I arrived at the question of “What is the usage and frequency change in shipping in 1905-1097 Egypt as represented by the Egyptian Gazette?”.

XPATH Query
In order to search the full contents of the Egyptian Gazette, a Xpath query had to be formulated. This allowed the total contents of the newspaper to be searched in its entirety from 1905 to 1907. This XML search needs two things to be successful, a where and what.

What
The "what" was relatively easy, find anything to do with ships right? No, because that gets every ad and listing in the paper, which there are many. The search needed to be refined, so the "what" changed to "shipping" instead of "ship". This still wasn't good enough to be used in any substantial way. Finally the solution was found, the xml id for a section of the paper called "shipping movements".

Where
The xml id of shipping movements made the where easy, I just then needed to get the content out of the division. This was done by searching for every paragraph inside of the feature "shipping movements" by using the query of //div[@feature="steamerMovements"]//p. I collected the data after updating the working sets to the most current pages. This was done on Wednesday, March 28th.

Challenges
Not all of the sections that were pulled for research were OCR'd correctly so they had to be either corrected by hand if they could be figured out what they were supposed to say, or they had to be deleted if they were too poor to even guess. Often times place names, one of the essential parts of the question, were incomplete or misspelled. Often times there would be awkward spacing or formatting issues. There would be sometimes where the section would be the same for a couple days, showing that a person most likely copy and pasted the same template from either their own issue or from someone else for several days and didn't bother to change the values and content to reflect what the their specific issue said. There is a big possibility for missing out on many instances of the section if people don't use the xml id, as this is the hinge that holds this search together.

Results
From the Xpath query, there were 698 instances where the xml id for "shipping movements" were used. Each paragraph contains a listing of the name of the ship, usually the company, where its going/when its getting to Egypt, the date of arrival, and what they had on board the ship either people, cargo, or both. Sometimes the ship will list some specifics of what cargo they were carrying, listing the amount with its unit measurement ex. (1000 bales cotton).

Visualization
In order to better visualize the data, a word cloud was created in order to display the frequency of destination to and from Egypt. The bigger the word, the more often it occurred in the text.
![Word Cloud](word cloud v1.png)
Interestingly enough, looking at the hard data, the top six is as follows, with number of occurrences provided,
292	Malta
273	Alexandria
207	Liverpool
85	Manchester
74	Marseilles
49	Antwerp
This is very interesting results on their own, but they will eventually contribute to a overall patch work of the wider question. One peculiar thing to come out of this search is the fact that Malta seems to be the top destination for ships to and from Egypt. Looking at bit deeper creates some doubt to the validity of this finding. Malta was very small with a tiny permanent population of people there, how could they be the biggest trading partner for one of the prizes of the British Empire? Looking even deeper into the actual text, often times the listings include that the ship will be going somewhere via Malta, probably due to its location in the Mediterranean as a good stopping point to restock and get ready for the second leg of their journey.
