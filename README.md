# traffic-stops
## Project Background
* Is there evidence of (racial) inequity in the amount of traffic stops by police?
* Attach this analysis with broader demographics in each state/region - how likely is a traffic stop for a random person based on demographics? For what reason?
* Working paper: https://5harad.com/papers/traffic-stops.pdf
* Data source: https://openpolicing.stanford.edu/data/
* Visualization Inspiration: https://www.nytimes.com/interactive/2018/03/19/upshot/race-class-white-and-black-men.html

## Data Notes
* More than 60 million (63.7) state patrol stops
* 20 States
* Between 2011-2015

### Analysis Method

1. Quantify racial disparities in stop rates and post-stop outcomes
_Black drivers stopped more often than White relative to driving-age population, but Hispanic drivers stopped less often than White... Black and Hispanic drivers more likely to be ticketed, searched, and arrested_

2. Investigate the degree to which these differences may result from discrimination - focusing on search decisions
_Bar for searching Black and Hispanic drivers is lower than searching White drivers_

3. Effects of drug policy on stop outcomes
_Legalization of recreational weed in WA and CO reduced search and misdemeanor rates across the board, though relative race gap still exists_

### Data to visualize?
[Aggregated cleaned data set](https://github.com/5harad/openpolicing/blob/master/results/data_for_figures/combined_data.csv)
* __stop_rate__: "the rate at which white, black, and Hispanic drivers are stopped, relative to their
share of the driving-age population" (p. 4). _driving-age population is readily available, accurately estimated by US Census bureau, doesn't take into account race-specific differences in driving behavior (I am ok with this)_ (Figure 2, pg. 4)
⋅⋅* https://github.com/5harad/openpolicing/blob/master/results/data_for_figures/fig2_stop_rate_county.csv.  

* __speeding citation rate?__: "the probability a driver stopped for speeding is given a citation as opposed to a warning (or no penalty at all) - (p. 6)"

* __search_rate__: Likelihood of getting searched for drugs, weapons, contraband after you're stopped. 2% white, 3.5% black, 3.8% hispanic (p. 6)

* __consent searches__: officers must seek permission from drivers to search their vehicles - _probable cause_ searches don't need consent but have a higher standard of evidence.

* __arrest rates__: % of stops resulting in the arrest of the drivers (p. 7)

* __hit rate__: The proportion of searches that successfully turn up contraband (p. 8) - nine states include race, location of stop, search, and contraband found fields. Hispanic hit rates lower than whites (22%), white=black rates (28%) (a lower hit rate means more discrimination, since this suggests double standard of searching more on less evidence)

* __threshold test__: In effect, what is the "threshold" of suspiciousness that an officer has when evaluating whether to search a driver. A higher threshold = more trust, so a lower threshold shows more bias, which will require some though on how to actually visualize this in the context of more drivers - maybe using that threshold.
