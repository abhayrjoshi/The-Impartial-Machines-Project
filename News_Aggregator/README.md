# The Impartial Machines Project

## Issue
https://github.com/MozillaFestival/open-leaders-7/issues/21

## News Aggregator

This is the first step, where we first collect the news article and then summarize it in such a way that it represents the news in a nutshell. To run this module, follow the below steps.

We use Python 3X Version only.

    $ pip3 install -r requirements.txt
    
    $ sudo apt-get install libxml2-dev libxslt-dev
    
    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3

    $ python -m spacy download en

    $ python summary.py

Now, we get the news summary of one article, which we have defined in sumarry.py

## Method

    1. We collect the news article from the web

    2. We use spacy model to summarize the text into 5 sentences.


### Input

URL of Article -[https://edition.cnn.com/2019/04/29/asia/japan-imperial-abdication-akihito-reiwa-intl/](https://edition.cnn.com/2019/04/29/asia/japan-imperial-abdication-akihito-reiwa-intl/)


### Ouput

##### Summary of the above article in 5 sentences
    
	"I am worried that it may become difficult for me to carry out my duties as the symbol of the state with my whole being, as I have done until now," the soft-spoken Emperor said in 2016, in his second TV speech in three decades.

 	 In 1992, the Emperor became the first Japanese monarch to visit China, where he said he felt a "deep sadness" for the "unfortunate period in which my country inflicted great suffering on the people of China. A "love match" that won over Japan Michiko Shoda, now known as Empress Michiko, departs her home for the Imperial Palace in the early hours of April 10, 1959, the day of her marriage to Crown Prince Akihito. But I think that it is important today, when memories of the war are fading, to look back humbly on the past and correctly pass on the tragic experiences and history Japan pursued from the generation which experienced the war to those without direct knowledge. I want to earnestly fulfill my duties by always being close to the people, and sharing with them their joys and sorrows," he said at a press conference.


## Contributing

Thanks for your interest in contributing to The Impartial Machines Project! There are many ways to contribute. To get started, take a look at [CONTRIBUTING.md](CONTRIBUTING.md). Please check our issues in the repo and get started by contributing!

## Participation Guidelines

This project adheres to a [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to abhay.joshi.in@ieee.org or ssai.thejeshwar.in@ieee.org.

