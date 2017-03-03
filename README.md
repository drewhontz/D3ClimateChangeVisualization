# Visualizing Global Warming in US Cities

## Summary

This visualization is meant to show the percentage change in average annual temperature in cities across the United States.

I found the data set on [kaggle.com](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data); the data comes from the Berkeley Earth Surface Temperature Study that itself, is a combination from 16 reputable pre-existing temperature reports.

I chose to only use the US cities included in this set, and again filtered out data pre-1960 as earlier recordings had average temperature uncertainty that could explain most of the effect I was looking to explain.

## Design

I felt that this was a pretty straightforward visualization. Some ideas I fiddled with but did not implement were:

- Using a chloropleth map

  - I did not select this approach because I didn't have enough data to fill most of the US counties and I felt that showing change at the state level was less interesting than at the city level

- Using a continuous color scale from blue to red, to show the degree to which the percentage increased or decreased.

  - I figured since change in size is easier for us as humans to see as compared to change in hue, I selected size as our encoding for degree of change.

- Using percentage change from 1960 as opposed to degree difference.

  - I was originally using percentage change as the figure for which to scale the radius of our circles but once I realized that cities like Cincinnati, who had a % increase of ~ 228% which translated to ~0.7 degrees Celsius, I figured degree change would be less misleading/dramatic.

## Feedback

I am paraphrasing a bit but here is what my friends said when I sent them the gif.

- Person 1: "I understand this is meant to show change since 1960 and that other years are irrelevant but let me explore other years through a dropdown list. I can see some midwest cities look unaffected by climate change in 2013 but I think they were marked red in earlier years and I can't verify this. As it stands I am left to assume that whatever is blue at the end of the animation is/has not been affected."

- Person 2: "Is this viz going to be about voting groups? The basic red and blue colors look very much like the colors used to represent conservatives and liberals in the US. Why not use a continuous scale for color to avoid confusion, or choose different colors, or add a legend. Otherwise it makes sense, although I was immediately able to discern that the change in size and color was relevant to temperature change, I wasn't sure of the metric used to display this change. I.E. without reading the title I am not immediately aware that this is degree change since 1960"

- Person 3: "Anaheim is not that far South or West. Use other colors, red and blue near an election year is confusing."

### Incorporating this Feedback

- Changed colors to other shades of red and blue, still using discrete colors instead of a continuous scale. Size is easier for us to see according to our class.

- Added a legend

- Added buttons for an 'exploratory' experience after our animation

## Resources

- [Michelle Chandra's Basic US State Map](http://bl.ocks.org/michellechandra/0b2ce4923dc9b5809922)
- [Mick Bostock Let's Make a Map](https://bost.ocks.org/mike/map/)
