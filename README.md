# General idea

Fund a Kaggle-style competition with forecasting a large ecological data set

# Things to think about:

## Data set

* BBS is the obvious choice, but it would make sense to explore other options
  * Not clear that predicting 1 year forward at sites that have already been visited dozens of times is an interesting enough task
  * Need to get permission from BBS
  * Need to work around their schedule for posting data
    * Possible issue: can't predict when they'll release data, so can't give date for competition victory
    * Possible issue: what private data can we use for the public leaderboard?
  * Might need to allow multiple submissions for each site, depending on weather conditions, time of day of actual transect
* A data set that's already been collected and is not public could have logistic advantages over BBS
* A plant data set (where the weather on the day of collection doesn't matter as much) could have advantages over BBS
* Need to prevent "[leakage](https://www.kaggle.com/wiki/Leakage)" from training set to test set.
* Kaggle can put restrictions on the license of the data, if data source wants

## Auxiliary data sets

* Should provide as many good environmental variables as we can
* Should probably allow competitors to any public data set under certain conditions (I think that some competitions say the  competitors have to announce what data sets they're using on the forums)

## Evaluation metric

* Dave likes joint likelihoods, but could be tricky to implement unless we ask for a batch of Monte Carlo predictions for each site. Unclear if there's a simpler alternative that accomplishes the same thing
* Shawn pointed out that we could also ask domain experts and managers what they want to optimize
* Kaggle doesn't have any [examples of metrics](https://www.kaggle.com/wiki/Metrics) that would work well for abundance data, but I don't think they'd object to something like negative binomial log-likelihood as a metric.

## Timing/duration

* Timing may be depend a lot on the data provider
* 2-3 months seems like typical competition length
  * Heritage Health Prize was much longer (years) but had a complicated structure
* What trade-offs are associated with longer versus shorter?

## Prize money

* 10K, split among victors, seems to have worked well for other competitions (e.g. whales)
* Some competitions also have prizes for separate contributions (e.g. best visualization
* Kaggle will take a cut of the money, so total cost will be higher than total payout

## Post-competition incentives

* Paper or special issue about the competition and methods
* Mini-conference or symposium with talks by winners and organizers

## Cost centers

* Prize money
* Open access fees
* If mini-conference or working group, travel money?
* Time investment
  * before competition:
    * Coordinating with Kaggle 
    * Coordinating with data provider(s)
    * Curating the data
    * Picking a metric
    * Writing the website blurbs
    * [Other checklist items](https://www.kaggle.com/wiki/CompetitionLaunchChecklist)
  * during competition: 
    * Publicize competition
    * Responding to user questions on the forum
  * after competition:
    * Evaluating winners (e.g. confirming that they followed the rules)
    * Organizing paper or special issue
    * Organizing symposium

## Alternatives to Kaggle as host

I have no idea if any of these are any good

* CrowdANALYTIX
* Tunedit
* InnoCentive
* Topcoder
* HackerRank

## More information about hosting a competition on Kaggle

* Case study reports: https://www.kaggle.com/solutions/customers
* Checklist: https://www.kaggle.com/host/faq/checklist
* FAQ for hosts: https://www.kaggle.com/host/faq (link is now a redirect, but might be on archive.org.  Much of the information seems to have migrated to the wiki)
* Wiki:
  * Information for hosts: https://www.kaggle.com/wiki/InformationForHosts
* Quora answers: https://www.quora.com/Is-it-worth-hosting-a-Kaggle-money-competition
