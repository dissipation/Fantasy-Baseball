# Fantasy-Baseball
* Check out the [website](https://dissipation.github.io/DarshDSPortfolio/) assocated with this repository!
* The goal of this project is to create an accurate way to predict MLB player performance based on historical sabermetric data
* Fangraphs has a wealth of data that can be leveraged to get predict player performance
* The final projections also incorporate [ATC WAR Projections](https://www.fangraphs.com/projections.aspx?pos=all&stats=bat&type=atc&team=0&lg=all&players=0) for comparison/sanity checking and Positional Scarcity Calculations:
[Testing](Images for Readme/ImageforGH.PNG)

# Scoring Metrics
* In 5x5 Roto ranking values for each of the categories are not clear
* However, both Per Plate Appearance (PA) and Inning Pitched (IP) based values are approximately normal (according to an eye and Wilks Shapiro Test). This can be used to help predict per IP and PA values.
* Once predicted, these values are bumped up multiplying by projected PAs or IPs (normalized by the league means)
    * For overall rankings, total pitcher model scores are further normalized to equal total hitter model scores as both should be valued equally in a 5x5 category league
