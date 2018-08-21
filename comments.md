# NLP_mpis_comments
Natural Language Processing on driver comments.

[AJ] NLProcessor.py Line 49: What's this function for?

[JH] NLProcessor.py: include docstrings for all functions as

"""
comment, purpose, etc.
"""
at the start of each function.  This allows you to see a popup when you do a ctrl-space or whatever intellisense
hotkeys you are using making it easier to infer intent 

[JH] NLProcessor.py Line 36: this function seems like a really convoluted way to avoid doing 
something like set(pandas.field) or list(set(pandas.field))

[JH] NLProcessor.py Line 44: this function is redundant because it is doing the same thing as the previous one

[JH] NLProcessor.py Line 51: arbitrary lists like this are usually maintained in the header or in a seperate configuration file to 
make maintenance easier

[JH] NLProcessor.py Line 54-61: repeat of the above functions but nested in another function

[JH] NLProcessor.py Line 66: what is this doing?

[JH] NLProcessor.py Line 64: It seems like the purpose of this function could have been done with the intersection or non-intersection of a vector with a mask?

[JH] NLProcessor.py Line 84: Is the reason you built 64 because you have to have a customer tokenizer for the tool?

[JH] NLProcessor.py Line 107: some better notes on the purpose of the KMeans would be helpful.  I only
vaguely understand the process and what's being accomplished because we've talked, but I don't know from the code itself

[JH] NLProcessor.py Line 123: not sure this needs a comment, but explaining tuples for the uninitiated like Hunter would be helpful
in the future, not necessarily in the code

[JH] NLProcessor.py Line 129: how do you know the cluster names without knowing the outcome of the processing?

[JH] NLProcessor.py Line 170: Isn't it redudant to set the ticks to blank, then make them invisiable?

[JH] NLProcessor.py EOF:  I would like a walkthrough on the logic and tools.  I like that you are dumping a matplotlib to HTML
I find that incredibly interesting and would like to know more.

[JH] NLProcessor.py Line 24: Afterthought, after looking at the class.  This seems like an awakward work around
to simply doing a pd.open_csv?  Is there a reason for building a custom entity and then feeding a line
at a time through it and turning comment lines into objects?

**[TB] Stemming stop words**
