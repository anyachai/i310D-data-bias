# i310D-data-bias
For this assignment, I looked at the false positive rates in certain queries that I made using the get_toxicity_score function. I hypothesized that the model would fail when presented with comments that contained words commonly seen as negative but were used in a positive non-toxic connotation.

Three queries were made that show this phenomenon in effect:
1. "i'm so hungry i could eat a pig"
   This comment had a toxicity score of 0.8060606 which is relatively high and was scored as such because of the negative connotation that the word 'pig' has even though in this context it is simply referring to the animal.
3. "hey bitch i love you"
   The B word is a slur that has since been reclaimed by the women it refers to and is now used in regular conversation both in person and online. Even though this comment is being said in a friendly way, it still has a toxicity score of 0.93232936.
5. "she's serving cunt"
   In the LGBTQ+ community, this would mean something similar to "serving realness" or "serving" (bringing it) to a very extreme extent, which is a positive thing. However, this comment receives a score of 0.94992846 because of its use of the C word.

Within the dataset itself, I found an example of a false postive that is similar to previous comments in that it uses words commonly associated with negative intent but not necessarily in a non-toxic way. This comment, which I had included in the notebook, had a toxicity score of 0.825715 due to the multiple uses of the B word.

From the exploration of the dataset, its clear that extracting meaning or defining the tone of comments is very diffcult because the context that certain words are being used in changes so much. In addition, comments in this dataset were scored by humans with their own biases who might not understand certain vernaculars or terms in communities they aren't a part of (ex. "serving cunt" in LGBTQ+ communities).

Since the grading of comments is subjective in nature due to it being scored by humans, potential biases in the data could be lessened if comments were scored by multiple people with different perspectives/backgrounds to make sure its covered by as many bases as possible. However, this itself is difficult, since the dataset is dealing with such sensitive and disturbing content that people (especially of marginalized groups) shouldn't have to be exposed to. Overall, this assignment had been really insightful in terms of how Natural Language Processing works and how it can be used, and I truly believe further development of models can make the internet a safer and less toxic place.
