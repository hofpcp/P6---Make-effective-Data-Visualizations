# P6 - Make effective Data Visualizations
Project 6 in the Udacity Data Analyst Nanodegree Program  
Peter Carsten Petersen

## Summary

The presented visualization is an explanatory overview of the combined attendance for the Danish Premier Football League "Superliga", for
seasons 2010/2011 to 2016/2017. The data is presented as accumulated attendance data for participating teams for their respective first 8 
home games per season. The aim is to visualize the effect of a change in structure of tournament beginning with the 2016/2017 season. 
This Visualization can also be viewed directly via Gist https://bl.ocks.org/hofpcp/eb9e877db477327b796e7da36e85a72e

## Design
Initial thoughts for this visualization was to do a line chart over the periods. 1 line per team with specified points per match, but it quickly became apparent from the data collection, that this would lead to a very messy and low information visulization, as there are many teams with comparable attendance figures, where lines would overlap and big differences between individual matches depending very much on the strength of opponent, i.e. many peaks and valleys with no visually clear trends.  



Variables
Attendance accumulated: Type: Quantitative, Encoding: Y Axis, Chart Type: Stacked Bar chart
Seasons: Quantitative, Encoding: Y Axis
Individual Teams: Categorical, Encoding: Color Value & Label

### Visualization updates from feedback
- Issues with visualization when all teams were un-toggled solved
- Abbreviations spelled out.  
- Text updated for clearer explantion of visualization and findings on same.  
- Tooltip altered to show team specific trend over same period as the accumulated view, this adding a further analysis opportunity on the visualization.  

**Feedback not included in updated visualization**
- Fixed y-axis scale not included as the adjusting y-axis scale is viewed as more explanatory.  
- Side by side bar chart not chosen over stacked bar chart, as main point of visualization is to show overall attendance. "Compromise" was to alter tooltip to show team specific trend  
- Listbox instead of legend not chosen, as I believe the legend works equally well
- Omitting "Extra Teams 16/17" in initial wiew not included, as there is much value in the initial information when including in initial view.



## Feedback

### Feedback 1 in Danish

Fra: Kim Mikkelsen
Sendt: 2. december 2016 16:37
Til: Peter Carsten Petersen
Emne: RE: Superliga Tilskuertal visualisering

Et par småting.
 
- Bør Y-aksen ikke være konstant selvom man ekskluderer enkelte hold – således at søjlen blot falder, når man klikker hold væk ? 
  Men det er en visuel ting, som jeg måske ville synes var bedre.
- Synes det er meget forståeligt.

### Feedback 1 Translation

From: Kim Mikkelsen
Sent: 2. december 2016 16:37
To: Peter Carsten Petersen
Subject: RE: Superliga Attendance visualization

A couple of small comments:

- Should the y-axis not be fixed, so even when excluding teams the total bar is decreasing for each team excluded? 
  However this is just a visual preference
- I think it is very understandable.

### Feedback 2 in Danish

Fra: Jacob Vinzent [jacob_vinzent@hotmail.com]
Sendt: 7. december 2016 10:20
Til: Peter Carsten Petersen
Emne: Re: Superliga Tilskuertal visualisering

Hej Peter,

Undskyld den sene tilbagemeldning, umiddelbart flot, men her kommer et par punkter:

1. Du skal være opmærksom på, at i en stacked bar chart er det svært at sammenligne på tværs, tag eksempelvis Brøndby i 2013/14 
sammenlignet med 2015/16. Der er faktisk en %-vis relativ stor forskel, men det er svært at se. Derfor kunne der være en idé, at lave 
hver klub til sin egen bar, så grouped istedet for stacked. Her mister du så totaltallet, men det kunne evt. vises på en linie der 
ligger over dine bars eller en prik der ikke er forbundet (men vigtig at du ved en prik ikke mister trendfornemmelsen).

2. Det er lidt svært når legend og selection smelter sammen. Derfor synes jeg en listbox eller lign. på højreside, hvor man kan vælge og 
fravælge og altid ser hvad der er med ville være godt. At du så kan gøre det ved klik på legends kan være en bonus (bare den anden også 
opdaterer ved brug af legend og omvendt). Bare det at man er nød at skrive det ved siden af legend fortæller at det ikke er helt 
intuitivt.

3. Jeg synes hover effecten er cool, men du kunne overveje at lave click effekten til noget der laver grafen om noget mere detaljeret 
omkring den klub du har klikket på. Som der er nu viser et click en total af alle de klubber der er under, men hvad betyder det? Så 
afhænger hvor du rammer y-axsen af den sorteting du har i dit array.


### Feedback 2 Translation

From: Jacob Vinzent [jacob_vinzent@hotmail.com]
Sent: 7. december 2016 10:20
T0: Peter Carsten Petersen
Emne: Re: Superliga Attendance Visualization

Hi Peter,

Sorry for the late reply, i like the visualization, a few small comments:

1. You should be aware that in a Stacked bar chart, it is difficult to analyse across. E.g. "Brondby IF" in 2013/2014 compared to 2015/2016. There is a %-wise big difference, but it is difficult to see. Therefore it could be an idea, to instead make a bar chart not stacked but side by side for each team/season and possibly add a circle above each group to reflect total of all teams (important a circle does not loose the ability to show trend). 

2. It is a little difficult when Legend and Selection blends together. Therefore i think a listbox on the rightside of chart, where you can add/remove and always see what is included would be good. Keep legend click available as well, but have both update when one or the other is changed. Writing in the text that you have to click next to legend text, tells me it is not absolutely intuitive.

3. I like the hover effect (tooltip), but you could consider having the effect present some more detail regarding the team. As is now the tooltip shows a total of team + all teams situated underneath, and what does that mean? So it depends on where you are on the y-axis and the chosen and sorted array.


### Feedback 3

CtrlAltDelForum Mentor4d
Hi @Peter-394378,

Thank you for sharing this visualization! It is well rendered, axes and legend labels are appropriately sized and I like the interactive feature.

The one suggestion I would make is to enhance the explanatory nature of the visualization. I was not able to discern any particular finding when looking at this visualization. That could just be me, so please seek additional feedback rather than taking my word for it.

More specifically:

It is obvious from the analysis that total attendance has decreased in 2016/2017 y-o-y, despite of the new structure.
This is not obvious to me, if I converted this into a line plot it would have a bit of a wiggle except for 2013/2014, where it would peak. Out of curiousity, what was going on in 2013/2014? Has any test been performed to determine if there is a significant difference in attendance as a function of year and/or the new structure? This isn't required, but just by eye-balling it I'm not seeing a substantial difference.

Some viewers may not immediately realize what y-o-y means. Please consider spelling out year after year or use a phrase by year, or something to that effect.

This decrease even more significant when excluding the attendance for "Extra Teams 16/17" so that comparison is like for like on number of teams. This shows 2016/2017 attendance to be lower than any other year in the analysis.
That is true, once I clicked away extra teams (again, great job on that interactive feature :slight_smile: ) this clearly is the lowest attendance year. This may be something to focus on. One question I have though is now legitimate it is (I have no idea, just playing devil's advocate) to compare attendance of 12 vs. 14 teams since they are all using the same potential pool of attendees. As I know very little about this domain I don't know.

Digging one layer deeper it is noted that the decrease y-o-y is shared by all teams except for one "FC Midtjylland"
This is interesting. It does look like FC Midtjylland does not experience a substantial decrease. However, it does look like this is true of at least one other team, Aab

Please consider using feedback providers to help hone in a a key finding that will stand out in the initial view of the visualization. It may be that some different design elements could bring out a finding.

On a technical note, it looks like the legend toggle may not be working quite as intended. Everything works as intended unless you actually untoggle all teams. After that, the color encoding for whichever team was de-toggled last, persists.

Thanks again for sharing this visualization. It would be great to see any future versions.


## Resources

- **Data Sources:** www.superliga.dk / www.superstats.dk  
- **Dimplejs.org code snippets:** http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends / 
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_lollipop_with_hover  
- **stackoverflow code snippet:** http://stackoverflow.com/questions/29177336/dimple-stacked-bar-chart-adding-label-for-aggregate-total


