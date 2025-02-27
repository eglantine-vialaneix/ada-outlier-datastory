---
layout: page
title: Back to the Future 
subtitle: Back to the Future - Time-Traveling through Wikispeedia
---

# Part 1

The articles present in the Wikispeedia dataset have categories. Do these categories influence your success, Marty? Let's explore that together!


First, how the categories look like? For most of them one main category is followed by more precise subcategories. For example, the mixed-breed dog article has for main category "Science", first subcategory "Biology" and second subcategory "Mammals". For simplicity, we will keep only the first category. You can observe here the distribution of those main categories. HERE::\<insert image of Einstein the dog\>
<iframe src="/ada-outlier-datastory/assets/img/pie_cat.html" width="800px" height="400px" alt='Pie chart of the categories'></iframe>
Back in 2007, science articles represented almost 1/4 of the encyclopedia where as art articles consisted of less than 1% of it! HERE:: more analysis?


Second, we notice that among the 4598 articles, some have more than 1 main category: we count 590 articles with 2 main categories and 8 articles with 3. It complicates our analysis. To keep things simple, we will impose rules on which main category we think is the most important for the article considered. For this, we have created a partial ordering in the categories that is completely arbitrary.

Ok, now we are ready for some data analysis. Let's first look at the links between the articles: from which to which categories go the links? Do they lead to an article from the same category or to another? Is it easy to navigate to another category?
<div class="flourish-embed flourish-sankey" data-src="visualisation/20671114"><script src="https://public.flourish.studio/resources/embed.js"></script><noscript><img src="https://public.flourish.studio/visualisation/20671114/thumbnail" width="100%" alt="sankey visualization" /></noscript></div>
It seems really to reach articles about countries: there are more than twice of links pointing to countries than links going out from countries. It seems logical as for many concepts, the place of invention discovery or birth is mentioned, including the country. Science articles are the ones linking out the less to other categories, with only 41% of links going elsewhere than in science articles. With these data in mind, are there categories of articles harder to guess for players?


To answer this question, we can investigate the categories of starting articles and target articles of the players.
<div class="flourish-embed flourish-sankey" data-src="visualisation/20646616"><script src="https://public.flourish.studio/resources/embed.js"></script><noscript><img src="https://public.flourish.studio/visualisation/20646616/thumbnail" width="100%" alt="sankey visualization" /></noscript></div>

For unfinished paths, the middle step corresponds to the category of the last article visited. In 28% of the cases, the player is already in the good category when he/she stops playing. But do we need to be in the same category as the target article to find it? It depends! For "People" category for example, less than 10% of players who succeeded were on an article in this category right before winning! However, in the case of "Science", the rate goes up to 81%!
<div class="flourish-embed flourish-sankey" data-src="visualisation/20673754"><script src="https://public.flourish.studio/resources/embed.js"></script><noscript><img src="https://public.flourish.studio/visualisation/20673754/thumbnail" width="100%" alt="sankey visualization" /></noscript></div>

Let's do some tests to compare the distribution of categories between finished and unfinished paths.  

Analysis of other datas for finished/unfinished:

![distrib_shortest_paths_duration](/ada-outlier-datastory/assets/img/distrib_shortest_path_duration.png)

Further comparison between finished/unfinished:

![distrib_paths_per_game](/ada-outlier-datastory/assets/img/distrib_paths_per_game.png)

Influence of the shortest path on success:
<iframe src="/ada-outlier-datastory/assets/img/comparison_distrib_paths.html" width="100%" height="2000px" alt='comparison_distrib_paths'></iframe>

Super plot interactif:
<iframe src="/ada-outlier-datastory/assets/img/distrib_path_lengths_wrt_shortest_path.html" width="700px" height="500px" alt='distrib_path_lengths_wrt_shortest_path'></iframe>

Influence of the number of links:
scatter plot

Log. regression:
table with results?








# Part 2

Wikipedia structure comparison : 
overall differences 

![distrib_links_per_article](/ada-outlier-datastory/assets/img/distrib_links_per_article.png)


![diff_links_per_article](/ada-outlier-datastory/assets/img/diff_links_per_article.png)

network differences 

![heatmap_diff](/ada-outlier-datastory/assets/img/heatmap_diff.png)


![reachable_nodes](/ada-outlier-datastory/assets/img/reachable_nodes.png)


# Part 3

# Part 4

