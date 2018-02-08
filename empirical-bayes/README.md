# Empirical Bayes
Wait. What? We can do some Bayesian work without having to pull out a conjugate prior? What gives? Isn't this just cheating? Let's see. I think that there might be value in trying to recreate one of the simple, early in the chapter examples. Jonathan brought up a few times the claims data in insurance.

## Insurance Claims Data
Can we produce the same results as the claims data that is printed on p.76 of the PDF? Similarily, can we produce something akin to the estimates and plots produced for this working example?

## Shakespeare Corpus
Can we work to produce a *hold one out* cross validation of the Shakespeare corpus for word uniqueness? I've placed a corpus into the folder `./shakespeare-plays-plus/`. We could also just use the NLTK shakespeare corpus, but that is a little more contrite than this one. In this corpus is a folder for each class of play -- (1) comedies; (2) histories; (3) tragedies. Inside each category is a `.txt` entry for each work of that categoy. Additionally, there is a folder for each work. I think for our purposes, the folder isn't really necessary, because this just breaks down the content by character within the play.

I think the task at hand is to produce the following flow:

- Select `n-1` plays
- Calculate the number of unique works in that set
- Produce an estimate of the number of unique words that exist in the held-out play
- Count the number of unique words in the held-out play.

An add-on task might look at subsetting into class of play? Cross that bridge if you like. 

