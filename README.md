# General idea

Fund a Kaggle-style competition with forecasting a large ecological data set

# Things to think about:

## Data set

* BBS is the obvious choice, but it would make sense to explore other options
  * Need to get permission from BBS
  * Need to work around their schedule for posting data
    * Possible issue: can't predict when they'll release data, so can't give date for competition victory
    * Possible issue: what private data can we use for the public leaderboard?
  * Might need to allow multiple submissions for each site, depending on weather conditions, time of day of actual transect
* A data set that's already been collected and is not public could have logistic advantages over BBS
* A plant data set (where the weather on the day of collection doesn't matter as much) could have advantages over BBS
* Need to prevent "[leakage](https://www.kaggle.com/wiki/Leakage)" from training set to test set.

## Evaluation metric

* Dave likes joint likelihoods, but could be tricky to implement unless we ask for a batch of Monte Carlo predictions for each site. Unclear if there's a simpler alternative that accomplishes the same thing
* Shawn pointed out that we could also ask domain experts and managers what they want to optimize

## Prize money

* 10K, split among victors, seems to have worked well for other competitions (e.g. whales)
* Some competitions also have prizes for separate contributions (e.g. best visualization

## Post-competition incentives

* Paper or special issue about the competition and methods
* Mini-conference or symposium with talks by winners and organizers

## Cost centers

* Prize money
* Open access fees
* If mini-conference or working group, travel money?
* Time investment
