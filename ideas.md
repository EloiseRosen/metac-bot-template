# an overall idea
ask an LLM for the base rate of the event as an initial estimate. Then ask AskNews to surface relevant news stories, and then ask the LLM how that changes the probability.
If there's a bias in output estimates, could translate from the produced probability probability to actual probability, which could be trained on a bunch of questions.

# evlauating performance between models
Since we're trying to evaulate performance on events that haven't happened yet, we don't yet have a ground truth.  
in the previous bot forecasting tournaments the bots do worse than humans, so we could use the median of the human predictions are our ground truth. Then, when we make changes to our model we have a way to evaluate whether the change is an improvement or not.

# brainstorm of things we could try
* how does perplexity do? andrew has API credits from his subscription
* check out AskNews for news stories (free?)
* metaculus provides free credits from anthropic and openai?
* create a tree of branching dependent questions? So like, if the main question is "who will be Japanese prime minister on Jan 1, 2026", then a dependent question might be like "will Japan be in recession on that date?" Then it could recursively think through questions that get farther and farther away from the main question