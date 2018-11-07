--- 
layout: vis
display_site_title: true
vis_include: vis/goodreads_genre_nokids_anonymous_tsne.html
---

This is a visualization of ~1750 of the most active users on the Goodreads social
reading site.  They were randomly selected from the half million or so users who
have published at least 150 reviews on the site.   Each reader is represented as
a point, color-coded to show the primary genre of their reading, excluding
non-fiction and fiction for children and young people. (A visualization that
includes YA, children’s lit, and graphic fiction is [here](/allfiction/)).  We used an
algorithm called t-SNE and a presentation tool called Bokeh to visualize
readers’ taste profiles as proximity or distance from one another.  Mousing over
a point reveals the breakdown of that reader’s fiction reading by genre.  Points
that are near to each other represent readers who like similar kinds of books;
points that are distant represent readers whose tastes diverge.  Points that are
near to differently colored points correspond to readers who are relatively
“omnivorous” in their consumption of fiction.  Points surrounded exclusively by
same-color points correspond to “univores,” readers who do not stray far from
their one favored genre.

Where would you place yourself on this map? 
