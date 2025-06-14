## Analysis of Ammonia System Density in the Galaxy

Published: 15 Aug 2017 on Canonn (https://canonn.science/codex/analysis-of-ammonia-system-density-in-the-galaxy/)

Content: A report by [CMDR Maligno](https://canonn.science/user/maligno/).

## Executive Summary (i.e. the bottom line upfront)

This is a report of some analysis I’ve been doing this past week. My objective was to answer the following two questions:

1. Is there something special about the abundance of ammonia systems in the Thargoid “bubble” centered around Merope?
2. Can we use that information to help us find other possible Thargoid habitation bubbles elsewhere in the galaxy?

As I will demonstrate below, **the answer to the first question is NO**. The density of ammonia systems in the Merope region is not significantly higher or different than in the region around Sol (which serves as a benchmark because we know it is not host to Thargoid sites). In fact, the density appears to be lower than other regions within 2000 Ly from Sol.

**The answer to the second question is also NO**

## Introduction

As you all know, when one activates the Unknown Device it displays what appears to be a star map. Some have theorized that the dots shown in the map are not actual individual stars but perhaps other Thargoid “bubbles”, similar to the one centered around Merope where all Unknown Structures are found.

I was playing around with the following thought: is the “density” of ammonia bodies, such as ammonia worlds and ammonia giants, higher in the Merope Thargoid bubble than elsewhere in the galaxy?

## Analysis

For starters, I looked at the data available from EDDB and made a “heatmap” of all the discovered systems in the galaxy. The heatmap is 2D histogram with 100 Ly bins and the counts are shown in a log scale (10\*log10(N)). I setup the bins so that sol lands right in the middle of the of the “x=0,z=0” bin.

[![](https://canonn.science/wp-content/uploads/2017/08/SKgnfVT.png)](https://canonn.science/wp-content/uploads/2017/08/SKgnfVT.png)

As you can see, it’s a beautiful picture that essentially highlights the main areas explorers like to visit. There are parts where it looks like a web.

Below is the corresponding heatmap of systems with Ammonia worlds, Ammonia Giants, Ammonia water worlds, and Ammonia HMCs. It shows a similar exploration pattern, but it’s markedly less busy than the inclusive plot above.

[![](https://canonn.science/wp-content/uploads/2017/08/c1m1dZF.png)](https://canonn.science/wp-content/uploads/2017/08/c1m1dZF.png)

Now, when we look at the heatmap for all the discovered systems and zoom around Sol, we get the plot below:

[![](https://canonn.science/wp-content/uploads/2017/08/Cj0vznU.png)](https://canonn.science/wp-content/uploads/2017/08/Cj0vznU.png)

The corresponding zoomed-in heatmap of ammonia systems is shown below:

[![](https://canonn.science/wp-content/uploads/2017/08/CdTd1BD.png)](https://canonn.science/wp-content/uploads/2017/08/CdTd1BD.png)

The pattern shown in the two plots above is no surprise: the more a region of space is visited by explorers the more systems will be reported.

In order to remove the reporting bias, we first need to understand the “normal” ratio of discovered systems and ammonia systems. I looked at the nine bins around Sol (that would make it a 300x300Ly region) in order to get a good number of systems (I could have used the “Sol bin” only, but again I’m trying to smooth out statistical fluctuations). This ratio turned out to be 25.294, so around 25 systems for each ammonia system.

So, if divide a given bin in the ammonia heatmap by the corresponding bin in the general heatmap and multiply that by the normal ratio described above, we should get a number close 1 when the relative abundance is similar to that of Sol’s vicinity. A region of space with enhanced ammonia system abundance (as I presumed the Merope region has) would show a ratio much higher than 1.

The plot below shows the adjusted ratio (as described above) of ammonia systems to all discovered systems in a 2000×2000 Ly square around Sol. I should note that what’s shown is a log scale because otherwise the whole thing would appear as blue and not show minute variations in the adjusted ratio. Remember, 10\*log10(1) = 0, so anything higher than 0 represents higher than normal system density. Now, what I see here is that the bin containing Merope is not that much higher or different than that of Sol. **That means there’s nothing special about the ammonia system density in the Merope region**. In fact there’s another region nearby (bottom right corner) that shows higher density.

[![](https://canonn.science/wp-content/uploads/2017/08/qFxu3iF.jpg)](https://canonn.science/wp-content/uploads/2017/08/qFxu3iF.jpg)

## Conclusion

There is nothing special about the density of ammonia systems in the Merope region, it’s actually quite similar to that of Sol’s. So, as far as I can tell, we cannot leverage ammonia system density to find other possible Thargoid bubbles elsewhere in the galaxy. I might extend the analysis to systems that contain ammonia even in Icy Bodies and Rocky Ice Worlds. But for now, I’ll just go on beige patrol =).