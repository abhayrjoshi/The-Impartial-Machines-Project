# The Impartial Machines Project

# Issue
https://github.com/MozillaFestival/open-leaders-7/issues/21

# Vision
We are working with the community to help deliver a Dual AI Engine which tries to eliminate the potential influences/bias in the news by the means of similarity indexing and version control and helps connect the dots in facilitating the dissemination of impartial news conforming to the highest code of ethics possible.

We are working open because we believe that news should be non-influential to circumstances, operate independently from any influences/bias and should be prioritized based on the importance, free of any ulterior motives and validated by employing a proper community feedback loop. 

# Description
In the rapidly expanding Artificial Intelligence (AI) driven world, we can observe that AI is already making humongous decisions in our lives. Off late, we have reached arealization where we have understood that AI can work, &#39;as long as&#39; the input data is accurate and that decisions made by AI aren’t always right. &quot;When we blithely train algorithms on historical data, to a large extent we are setting ourselves up to merely repeat the past. We&#39;ll need to do more, which means examining the bias embedded in the data.” - Cathy O&#39;Neil.

There is tremendous need for AI conform to the highest code of ethics possible. Adhering to the ethics is predominantly required for the news ecosystem to ensure proper dissemination of information.

Our project proposes a state-of-the-art Dual-AI Engine system which in the first phase eliminates potential influences in the news viz. utilizing the first engine to scour over various news outlets /sources to collect the news and generate the unbiased news while the other engine cross validates the generated news. Over a period of time, with due feedback from the human community as well, while the first engine tries to learn how to surpass the second engine, the second engine learns the ability to not let the first engine do so. This cross-validation of content would help us reach a point which will help generate news that is potentially free of any influences as far as possible. 

In the second phase of delivery, the generated news is weighted for importance and potential impact on the society rather than relying on the driving Target Rating Point (TRP) mechanism adopted by various outlets with potential ulterior motives. We have
already experienced first-hand that a large pool of the electorate is vulnerable to the information being dissemination over these various networks which concludes that it potentially sway the future of world.

## Getting Started

The process is something which is very familiar to how our human brains works. 

Generally, How we read the Newspaper? First we skim through the titles of the articles in the whole newspaper, and then we go on prioritise the articles based on our interest and read them. Now, If I have written an unreliable article but, the title of it very promising. How a human will identify it? First he goes through the article, and based upon his previous knowledge and cross verifies it with other sources in the internet. Similarly, our engine will gets updated with all the events that’s happening. Now, given an news article, it tries to validate the similarity between the title and the article.( The process of it more technically is given below.) Once it finds more than 60-70% similarity (Threshold can be changed) then it picks the article and then cross validates it’s sources. Them if the source is reliable, the news is said to be reliable.

Here, the First Engine keeps itself updated from the news sources and creates a web of similarity articles. Now, if anything comes to second engine, it checks the similarity with title and then sends it to the first engine. If First engine too finds the similarity, then the article has by passed the test and proves to be valid. 

## Technical Explanation

With the latest updates in the field of Natural Language Processing, similarity checking is relatively simple when compared to a decade ago. 

First, the text form of data has to be converted to some kind of vectors so that our algorithm can understand it. 
For this there are say dictionaries like, for a given word there is already a vector generated. We need not reinvent the wheel. GLOVE, tf-idf, word2vec, etc., We need to first identify which model better suits us. We feel BERT Model (Google’s NLP Open Sourced Model) will best suit us. 

Once the vectors are formed, we have to check the similarity. For this here are many techniques. But, the underlying math is very simple across them. For Example, imagine a X-Y Axis Graph. Draw two straight lines form origin with an angle (theta) between them. Here Line 1 is Vector A, Line 2 is Vector B.(Actually we need to plot the vectors generated from the previous step). If the angle is too low then they are very similar and vice-versa. If that angle between them is considered as Cosine then his method is called Cosine Similarity.

## Contributing

Thanks for your interest in contributing to The Impartial Machines Project! There are many ways to contribute. To get started, take a look at [CONTRIBUTING.md](CONTRIBUTING.md).

## Participation Guidelines

This project adheres to a [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to abhay.joshi.in@ieee.org.

