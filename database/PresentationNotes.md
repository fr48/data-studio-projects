Writing about data breaches is a big part of the cybersecurity beat. I write about different types of information that are stolen, and how the pieces can be used. Some of the damage is obvious: Credit Card information stolen is bad. But it isn't obvious just want email addresses can be used against you. Or IP addresses.  Given an email address, what I could I find? I knew it was a lot, but I wanted a taste.

Starting with my Outcomes first---- 

I learned a valuable lesson: Just because you have geographic location doesn't mean it will make a good map. I should have listened at the onset when Jonathan said so.

Guess that's the second. When someone says a map is going to be boring, believe them.

The biggest challenge I had was trying to think about this dataset as a map, which is what Jonathan warned me about. I was able to find the geographic information--longitude and latitude--pretty easily since I was focused on IP addresses being part of the stolen data set. But even then, trying to think "Where are the data breach victims located?" was less compelling. Trying to figure out what was the most popular social media site, or what the most commonly stolen pieces of information are, were a lot more compelling. I was pretty intrigued that the most damaging -- number of information lost, for my users, were not from the largest data breaches. But that doesn't map well.

I tried a straight location of where my victims are located. It was all concentrated in the US, obviously. The state map was a bit better, as it gave me some insight on where my users are in the state. But there wasn't much of an interactive component.

I started looking at trying to make a map that would tell me what the most common lost piece of data was for that location. The map I had in my head was having what the most common data type would be *after email address* for each location.

That was my other map lesson: Just because it can be a map doesn't mean it is a valuable map. 

So going back and looking at what I did to get to this point:
I didn't want to trawl the criminal forums or buying any databases. So I thought I would stick with Google. It's a little frightening just how many people are on Reddit asking, "Anyone know where I can get..." I found Collection 1 in just a matter of minutes with a Google search. I chose not to use it. So I went to one source that made me feel less gross: Pastebin.

Most of the pastebin dumps tend to be usernames and passwords, but I didn't want to traffic in passwords if I could help it. I also didn't want "old" data, since these dumps can become stale pretty quickly. I began with two dumps with IP addresses and email addresses.

My secondary sources once I had those two pieces of information were Email Reputation and Have I Been Pwned.

I had a lot of fun working with the Geolocation database, and got really good at comparing columns in dataframes and doing lookups. But I wound up abandoning that whole set because the database had limited accuracy. Switching to an API gave me nearly 95% of all the addresses, but it was not nearly as satisfying.

One valuable lesson is that dumps are raw. That's a good thing, actually. That means whoever is using these lists for bad aren't just downloading and good to go. They have to spend time cleaning up and moving things around.

Looking forward:
I am torn. I want to try to work more on getting an interesting map out of this. But maybe I am just doubling down on this, and it's just not a very mappable dataset and I should cut my losses.

This dataset would benefit more from histograms and charts. 


