---
layout: archive
title: "Dårligdommerne"
permalink: /coding/daarligdommerne/
author_profile: true
---

[Dårligdommerne](https://da.wikipedia.org/wiki/D%C3%A5rligdommerne) is a Danish movie podcast. For more than 10 years, Jacob, Troels and Christopher have been watching, primarily, poor Danish movies and along the line they have generated a bunch of data related to their podcast. As a small coding project I've tried to look into this data. 

So, I've downloaded the [IMDb Non-Commercial Dataset (14/08-2024)](https://developer.imdb.com/non-commercial-datasets/) and converted it into parquet files using a custom Python script for easier handling of the very large datasets. And I should mention that, at the moment, I have only included movies and short films - not tv series.

Dårligdommerne has reviewed both short and long films. Let's look at how the movie run time is distributed across the ca. 230 movies included in my present dataset: 

![Distribution of Movie Runtimes](https://github.com/jonashjaeger/jonashjaeger.github.io/blob/master/images/daarligdommerne_runtime_distribution.png)

Let's look at the stats: 

**Count:** 228 movies

**Average runtime:** 90.3 minutes

**Shortest movie:** 6 minutes - Dværgen og Luderen (2009); Blokland (2015); Skizo (2008)

**Median:** 90.5 minutes

**Longest movie:** 242 minutes - Zack Snyder's Justice League (2021)

![Distribution of Movie Runtimes](https://github.com/jonashjaeger/jonashjaeger.github.io/blob/master/images/daarligdommerne_boxplot_runtimes.png)

All in all the guys have wasted around **20.600 minutes** of their lives watching bad movies so the rest of us don't have to. That amounts to **14.3 days** of their lives so far. 

But have they actually been watching all bad movies? Let's look at the IMDb ratings for their impressive port folio: 

![IMDb Ratings](https://github.com/jonashjaeger/jonashjaeger.github.io/blob/master/images/imdb_ratings.png)

And let's just look at the basics stats again: 

**Average IMDb rating:** 5.08

**Median rating:** 5.3

**Worst rating:** 1.6 - Stjerner Uden Hjerner (1997)

**Best rating:** 7.9 (Zack Snyder's Justice League (2021) which doesn't make sense when Commando (1985) is rated 6.7

Of the movies included in my current data set **129** movies are rated *below* the average rating of 5.03 with 99 rated *above* the average IMDb rating. 

Let's look at the directors and we've been through quite a number over the years. **176** of them to be exactly. Of the directors, we've been subjected to more than once, Zack Snyder, once again haunts us with **7** movies:

**Sucker Punch** (2017)

**Batman v Superman: Dawn of Justice** (2016)

**Justice League** (2017)

**Army of the Dead** (2021)

**Zack Snyder's Justice League** (2021)

**Rebel Moon - Part One: A Child of Fire** (2023)

**Rebel Moon - Part One: The Scargiver** (2024)

Now, let's visualise the other very honourable mentions: 

![Directors](https://github.com/jonashjaeger/jonashjaeger.github.io/blob/master/images/daarligdommerne_directors_2%2B.png)

So, let's look into the Søren Bregendal Awards. In my dataset I have identified **240** recipients and some people have received the award more than once: 

![Multiple recipients of the Søren Bregendal Award](https://github.com/jonashjaeger/jonashjaeger.github.io/blob/master/images/daarligdommerne_soren_bregendal_freq.png)



