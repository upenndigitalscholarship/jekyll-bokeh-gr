---
layout: vis
title: Readers Mapped by Genre-Mix
display_site_title: true
display_page_title: true
order: 1
permalink: /adultfiction/
vis_include: vis/goodreads_genre_nokids_anonymous_tsne.html
---

This is an interactive Bokeh visualization of ~1750 of the most active users on the Goodreads social
reading site.  They were randomly selected in 2017 from all users who
had then published at least 150 reviews on the site.   Each reader is represented as
a point, color-coded to show the primary genre of their reading, excluding
non-fiction and fiction for children and young people. Our reason for excluding those
genres is that in many cases they represent the preferences of a user's child rather 
than those of the user herself. A visualization that includes YA, children’s lit, and 
graphic fiction is [here](/allfiction/). 

Altogether these users have reviewed about 200,000 different works of fiction.  We assigned
each work to a genre category based on how its readers tend to "shelve" 
it in their Goodreads collections.  A book that is shelved as "historical fiction" by 
30% of its readers, "literary fiction" by 10% of its readers, "mystery" by 55% of its 
readers, and various other genres by 5% of its readers would be assigned to our 
Mystery/Crime/Detective genre category (color = grey).

Based on the particular mix of genres in their reading and reviewing, their "taste profile,"
we used an algorithm called t-SNE and a presentation tool called Bokeh to visualize
readers as standing at various Euclidean distances from one another.  Mousing over
a point reveals the breakdown of that reader’s fiction reading by genre.  Points
that are near to each other represent readers who like a similiar genre-mix of books,
e.g. they both might read mainly historical fiction with occasional works of science fiction. 

Points that are near to differently colored points correspond to readers who are relatively “omnivorous” in their 
consumption of fiction.  Points surrounded exclusively by same-color points correspond 
to “univores,” readers who do not stray far from their one favored genre. The fact that 
each genre appears as a fairly well-defined color-zone -- a green (Romance) neighborhood 
at one side of the graph and a brown (Literary Fiction) neighborhood at the other side 
-- suggests a predominant pattern of univorousness.   This is by no means the whole 
story; our published articles develop a more complex interpretation of what is figured 
here.  Other interactive visualizations, which you can explore via the menu above, 
measure the similarity of readers' taste profiles by other  metrics, e.g. taking into 
account the specific books a user has read rather than merely the genres of those books.  
But this graph is a good starting point.

Where would you place yourself on this map?
