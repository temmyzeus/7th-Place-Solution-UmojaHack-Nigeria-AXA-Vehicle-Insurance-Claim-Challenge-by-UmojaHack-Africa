# 7th-Place-Solution-UmojaHack-Nigeria-AXA-Vehicle-Insurance-Claim-Challenge-by-UmojaHack-Africa
Notebook containing the 7th Place Solutiion for UmojaHack Nigeria: AXA Vehicle Insurance Claim Challenge by UmojaHack Africa hosted on Zindi Africa

Link to Competition   [HERE](https://zindi.africa/hackathons/umojahack-nigeria/leaderboard)

Approach was extracting the day,month & year for the 3 datetime features in the dataset, and a new feature called "Policy Duration days" representing how long the policy lasted or will last in measure of days.

Missing Values which are all categorical were filled just with the word "missing". Due to the presence of some values being present in train and absent in test and vice versa, the train and test we're simply concatenated and pandas factorize was used to encode them.

### Modelling

Simple Random Forest Classifier was used with predict probabilities and a custo function was used the threshold the probabilities to 0's and 1's with the threshold itself being set at 0.388
