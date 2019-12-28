# Michigan Amicus Project

**Word Frequencies**

Transforming amicus briefs into tokens to be analyzed. With stop words being removed, there are approximately 1.3 million words used though 420 Amicus Briefs. Most words are fairly generic, but that should not be entirely surprising considering that all briefs have been submitted to the Michigan Supreme Court. In the graph, the top 15 words from amicus briefs are shown. Numerical values have been removed from the graph.

[![Freq](https://i.imgur.com/XzuWuj5.png)]()

The words that are used by amici follow a similar path when ranking word usages. A word like "court" is ranked "1". However, as shown, the word variety used by amici is vast. Some filers will use approximately 10,000 unique words across all the briefs that they file. The dotted red line is the slope of the rank based on the actual frequency of the words at given ranks. 

[![Freq Map](https://i.imgur.com/F6MpNfM.png)]()

**Word Positions**

The position of words can provide insight into the overall structure of amicus briefs. There are two primary ways that words can be sorted to show their location. First, they can be sorted to show which words are more likely to show up at the beginning or end of the amicus brief. Second, words that are over-represented at specific points in the text can be mapped. 

In the first, figure the top 15 words that are shifted to both the beginning and end of an amicus brief is shown. It is clear that certain words might be used more at either the beginning or end of a narrative. A word like "statement" is very likely to show up in the beginning of an amicus brief, while "respectfully" is almostly guaranteed to show up at the very end of an amicus brief (unsurprising since many briefs end with a "respectfully, <insert lawyer name here>"). 

[![Start End](https://i.imgur.com/f3QmJHR.png)]()

Another way to show where words show up in a amicus brief is mapping the word's specific location throughout the entirity of an amicis brief. Much like the figure above, the figure below is able to map out specific locations of words through a text. A word like "association" is likely to show up near the beginning and end, but is more slightly more likely towards the beginning of a brief. Yet, "landlord" usages peaks near the middle of a brief, but is fairly common throughout amicus briefs.

[![Start End 2](https://i.imgur.com/C5odfUJ.png)]()

Rather than focusing on either the beginning or end of an amicus brief, more information can be gathered by breaking up an amicus brief into more sections. In this example, each brief is broken into deciles (10 percent increments). For every brief, regardless of length, each decile is compared across every amicus brief. The words appear are words that are most over-represented in the specific decile. For example, the words "line", "jurors", "tenancy", "distinction", "waiver", "areas", "payments", and "original" are over-represented in the sixth decile. In other words, about 60 percent of the way through any amicus brief, these words would be more likely to appear than any other part of the brief. 

[![Over 1](https://i.imgur.com/U33Msj9.png)]()

In the figure below, it takes the same information from the previous figure, but takes the top 3 over-represented words from deciles 2 - 9 and maps their location through the entirity of an amicus brief. For each word, there is a fair amount of fluctuation between its peak and other points. A word like "dictionary" peaks fairly early in a brief, before showing up semi-frequently towards the end of a brief. 

[![Over 2](https://i.imgur.com/CXGa5hk.png)]()

**Bigrams**

Bigrams present the directionality of words that appear within amicus briefs. In the Michigan Supreme Court, amicus filers will use word pairs like "trial court", "amicus curiae", and "common law" with relative frequency. Each of these word pairs would be a single bigram. 

When only looking at bigrams that appear 180 times across all narratives, the word pairs reveal common legal jargon that would appear to support an argument or claim within court. However, there is strong indication that specific pairs are tied to specific areas of law. For example, "reasonable doubt" is likely tied to criminal procedings in which the burden of evidence must be proved beyond a "reasonable doubt". Yet, other themematic bigrams appear as well like "real property" or "medical malpractice". To a certain degree, bigrams can highlight various trends and patterns among cases appearing before the Michigan Supreme Court. 

[![Bigran](https://i.imgur.com/6NcxmSm.png)]()

**Word Correlations**

Similar to bigrams, word correlations focus on pairs of words. However, unlike bigrams, word correlations do not care as much about directionality. Word correlations only care about how frequently two words appear together. In the situation of word correlations the words "zoning" and "ordinance" are connected. While it is likely that the bigram would be "zoning ordinance", word correlations do not care if it reads "zoning ordinance" or "ordinance zoning". All that matters is that the words are connected in some way. 

Word correlations provide more information about the types of cases that appear before the Michigan Supreme Court than bigrams. In the lower left of the figure, many terms are connected, yet there is a trend of cases dealing with damages. In general, there appears to be many different torts that are being litigated in the Michigan Supreme Court, ranging from medical malpractice, liability claims, and potentially workplace claims. On the far right of the figure, issues tied to marijuana appear (in some of the earlier cases marijuana was frequently spelled wrong). In both civil and criminal cases, marjiuana issues drew significant amicus attention. However, the word correlations highlight that cases that appear before the Michigan Supreme Court touch on both possession (criminal case) as well as concerns of medical marijuana usage (civil cases). While other legal matters appear, the word correlations also point to the language that amici use to bolster their claims, ranging from legislative, statuory, and constitutional matters.

[![Word Corr](https://i.imgur.com/vIaACfZ.png)]()

**Sentiment Analysis**

Sentiment analysis is a way to conceptualize text as either positive or negative. To conduct this analysis, I am primarily using the AFINN lexicon, which ranks words on a -5 to +5 scale, where -5 is most negative and +5 is most positive. When all 420 amicus briefs are analyzed in this project, language usage is slightly negative (dropping to a low of about -0.3). However, one thing to consider is that sentiment analysis is unable to discern the context that words are used in. For example, if a negative word such as "kill" appears in a brief for a murder case, the word will be treated as negative. However, if "kill" appears in the context of "did not kill", "kill" would still be treated as negative. 

[![Sent Trend](https://i.imgur.com/TrEHq4y.png)]()

Of course, looking at the sentiment of all amicus briefs does not reveal anything about the language usage of specific amicus filers. Looking at the language usage of the most frequently filing groups reveals fairly significant variation in language usage. When an Attorney General or the Prosecuting Attorney's Association of Michigan file a brief, they use the most negative language. Conversely, the Michigan Municipal League uses some of the most positive language. 


[![Sent Trend Group](https://i.imgur.com/pmT65bU.png)]()

However, looking at groups by themselves hides the fact that different attorneys file briefs for the group. Consider, the Attorney General had to individuals in the position from 2008-2016: Michael A. Cox and Bill Schuette. Below, it shows that the language usage by both Attorney Generals is very different from one another. Michael A. Cox used very positive language, while Bill Schuette used more negative language. 

[![Sent Trend AG](https://i.imgur.com/YLq6DGq.png)]()

Consequently, when we view the language usage across some of the most frequent filing attorney's, regardless of group, actual language usage becomes a bit more clear. For the most part, attorney's use negative language. However, for Michael A. Cox, Richard C. Kraus, and Liisa R. Speaker, the language usage is noticeably more positive than other frequent, filing attorneys.

[![Sent Trend Attorney](https://i.imgur.com/b4w2kOx.png)]()

Beyond specifc actors, sentiment can also be analyzed across different grouping categories, such as which ligant's position the brief is filed on behalf of. When filing for an appellant or respondent, the language difference is not very significant. However, when a group chooses to not support either litigant, the language usage does appear to be different. However, in the sample of cases, there were not many filers supporting neither litigant, so this may skew the data. (Note: For support of Appellant or Responded, coding was conducted where if a case is "Party A v. Party B", Party A was the Appellant and Party B was the Respondent)

[![Sent Trend Support](https://i.imgur.com/CTliOJf.png)]()

**Gendered Analysis**

Gendered word analysis uses bigrams at the core to determine which words are more like to come after specific words, such as "he" or "she". Gendered analysis is not perfect as the analysis does not include pronoun varients like "himself" or "herself", nor does it include sweeping pronouns like "they". Yet, it can still be interesting to look at which words are more likely to show up after "he" and "she" respectively. 

In amicus briefs, "she" is more likely to have "suffered". "fails", and "needed". On the other hand, "he" is more likely to have "confessed", "contends", and "explained".

[![Gendered 1](https://i.imgur.com/u1gsVlZ.png)]()

The figure below is another example of how to map gendered word usage. It is not surprising that common linking verbs like "is", "was", and "had" are most commonly used words and are not strongly steered towards "he" or "she". The word "or" is the one outlier in the figure. However, this is likely tied to frequently usages of the phrase "he or she".

[![Gendered 2](https://i.imgur.com/uUsxARH.png)]()

To get a more nuanced view of words showing up after "he" and "she" respectively, words can be selected. The words selected have stronger action connotations. The words were chosen by looking at the total frequency of the word usage. In this context, "she" is more likely to have "suffered", "fails", and "covets". On the other hand, "he" is most likely to have "confessed", "explained" and "committed". This figure also shows how the tense of a specific word matters. "She" is most likely to "fails", while "he" is mostly likely to have "failed". 

[![Gendered 3](https://i.imgur.com/BTZatTz.png)]()




