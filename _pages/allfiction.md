--- 
layout: vis
title: All Fiction 
display_site_title: true
display_page_title: true
order: 3 
permalink: /allfiction/
vis_include: goodreads_genre_anonymous.html
---

This version of our t-SNE projection includes the books that are most often
shelved in Goodreads as Young Adult, Children’s, or Graphic Fiction.  Some
reviewers of these books are young people, who fall outside the scope of our
study; others are adults recommending books that their children have
enjoyed—i.e. reporting on the reading tastes of someone else, and thus
potentially misleading with respect to their own preferences.  Otherwise, the
data are unchanged, and the t-SNE algorithm applied in the same way to project
as simple two-dimensional distances these ~1750 readers’ multi-dimensional
relationships of similarity and difference from one another.  Each reader is
represented as a point, color-coded to show the primary genre of their reading.
The t-SNE outputs have been visualized with the Bokeh presentation tool.
Points that are near to each other represent readers who like similar kinds of
books; points that are distant represent readers whose tastes diverge.  Points
that are near to differently colored points correspond to readers who are
relatively “omnivorous” in their consumption of fiction.  Points surrounded
exclusively by same-color points correspond to “univores,” readers who do not
stray far from their one favored genre.
