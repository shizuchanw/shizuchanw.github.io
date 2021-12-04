---
layout: post
title: Echo Chamber Project Reflection
---


### What did you achieve in your project? 
We have achievements in mainly 3 aspects: 
1. **Polarity Scores** \
We cleaned a huge dataset of 39M tweets, and calculated the political polarity scores of users of these tweets. \
Scores are calculated based on the tweets that the user produces (what he/she tweets) and consumes (what their followers tweet).

2. **Clusterings** \
We first identified clusterings in users based on their production and consumption scores using Agglomerative Clustering, Spectral Clustering, and Heatmap.\
We then identified communities of users based on user network (ex. A follows B) using the modularity community detection method, and plotted it with Gephi. \
We found the two clusterings we identified are quite similar! i.e. there is a strong correlation between the Twitter social network structures and derived polarity scores! \
We can hypothesize that, the Twitter Echo Chamber also makes people only follow those with the same polarity (i.e. what they want to hear)!


3. **Web App** \
We finally created a webapp to explain what Echo Chamber is to the general public, and to showcase our findings to the informed public!


{% include reflection/agglomerative.html %}
{% include reflection/spectral.html %}
{% include reflection/heatmap.html %}
![network.png]({{ site.baseurl }}/images/Network_Visualization.png)


### What are two aspects of your project that you are especially proud of? 
1. I'm very proud that we were able to deal with such a huge dataset!
2. I'm also proud of the web app: althought there were a lot of bugs when I was building it, it turns out to be very cute and informative.

### What are two things you would suggest doing to further improve your project? 
1. Run the same study on the unfiltered dataset: the current clusterings are identified based on a fitered dataset, which might cause bias
2. Conduct sentimental analysis on each tweet, and use that to adjust the current scores

### How does what you achieved compare to what you set out to do in your proposal? 
We achieved most parts of the proposal, except the sentimental analysis on each tweet. We couldn't do so because we realized that, currently unsupervised sentiment analysis is still a research issue :(

### What are three things you learned from the experience? 
1. how to deal with huge dataset! I learned about batches in tensorflow, pandas read in batches, and sqlite3 database!
2. flask and CSS when building the webapp!
3. text data cleaning & analysis!

### How will your experience completing this project will help you in your future studies or career? Please be as specific as possible. 
I got really interested in networks through this project, and I learned packages (networkx) and skills to analyze networks, which will help me greatly in my future studies.
