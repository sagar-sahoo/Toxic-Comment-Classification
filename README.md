# Toxic-Comment-Classification


Discussing things you care about can be difficult. The threat of abuse and harassment online means that many people stop expressing themselves and give up on seeking different opinions. Platforms struggle to effectively facilitate conversations, leading many communities to limit or completely shut down user comments.

The Conversation AI team, a research initiative founded by Jigsaw and Google (both a part of Alphabet) are working on tools to help improve online conversation. One area of focus is the study of negative online behaviors, like toxic comments (i.e. comments that are rude, disrespectful or otherwise likely to make someone leave a discussion). So far they’ve built a range of publicly available models served through the Perspective API, including toxicity. But the current models still make errors, and they don’t allow users to select which types of toxicity they’re interested in finding (e.g. some platforms may be fine with profanity, but not with other types of toxic content).

Here, I built a  model that’s capable of detecting different types of of toxicity like threats, obscenity, insults, and identity-based hate. I used a training dataset of 159571 comments from Wikipedia’s talk page edits. The trained Model was used to predict the hate category for 153164 comments (Test Dataset)

Libraries Used - pandas, sklearn (TfidfVectorizer, LogisticRegression, model_selection)

Results:

CV score for class toxic is 0.9700949143980843
CV score for class severe_toxic is 0.9877221710996867
CV score for class obscene is 0.9849319646541103
CV score for class threat is 0.983317402444328
CV score for class insult is 0.9781087047384173
CV score for class identity_hate is 0.9746353857844813

Total CV score is 0.979801757186518

