# P6---Make-effective-Data-Visualizations
Project 6 in the Udacity Data Analyst Nanodegree Program
Peter Carsten Petersen

## Summary

The presented visualization is an explanatory overview of the combined attendance for the Danish Premier Football League "Superliga", for
seasons 2010/2011 to 2016/2017. The data is presented as accumulated attendance data for participating teams for their respective first 8 
home games per season. The aim is to visualize the effect of a change in structure of tournament beginning with the 2016/2017 season. 
Visualization can also be viewed directly via Gist https://bl.ocks.org/hofpcp/raw/eb9e877db477327b796e7da36e85a72e/

## Design



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

### Translation

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


