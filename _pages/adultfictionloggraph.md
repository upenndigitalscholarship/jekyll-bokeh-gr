---
layout: vis
title: Adult (Log-Net)
display_site_title: true
display_page_title: true
order: 4
permalink: /adultfictionloggraph/
vis_include: vis/goodreads_genre_nokids_anonymous_tsne_log_graph.html
---

[This is the Log-Network t-SNE visualization. 
To hide, add `hidden: true` to the front matter of this page,
anywhere between the two lines (`---`).]
This visualization is based on the same way of visualizing the taste profiles of readers as in our Reader Network map.  The only difference is that here we have applied a log transformation to the distances between readers.  On the non-transformed Reader Network map, distance between two readers is the actual probability of one reader having read a random book from the other reader's review shelf. In this version, we use the log probability, which tends to make distances on different scales easier to interpret by creating greater spread between unsimilar user-points. 

In other respects, the t-SNE algorithm is identical.  Similarity or difference between two readers' tastes was calculated according to the specific books they have reviewed rather than just the genres of those books. The code generates a distance matrix by treating all the books and all the users as part of a bimodal network -- that is, a network with two kinds of nodes that only connect to nodes of the other type. It then "imagines" a process: suppose you talk to a random user and ask for a recommendation. They randomly pick one of the books they've reviewed. Then you talk to other random users until you find one who has also reviewed that book, and ask them for a new recommendation ... ad infinitum. The probability of going from a given user to another in this scenario is the "distance" between them (actually, it's 1 - p instead of p). 

To make things work nicely we posit that all the users have reviewed one amazingly popular book that we don't know the title of. This ensures all users are at least slightly connected in the network. You might say that this imaginary book is goodreads.com.
