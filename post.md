*(This post was originally written by Lex on December 21, 2022. It has been reposted here for better pseudonymity, and slightly edited for clarity.)*

***

I’m reading [this article](https://gwern.net/doc/statistics/bayes/hope-function/1994-falk) (actually an excerpt from a book) which is about how people think about a particular probability problem. The problem goes like this:

> Imagine you’re looking for your favorite shirt. You think it’s probably in your dresser (80% probability that it’s in the dresser, 20% probability it’s somewhere else). Your dresser has **8** drawers, and you have no idea which drawer it might be in (equal probability that it’s in any individual drawer). After you’ve checked **3** of the drawers without finding the shirt, how has the probability that the shirt is in the dresser at all changed? How has the probability that you’ll find the shirt in the next drawer you check changed? 

Another equivalent formulation of the problem goes like this:

> Imagine you’re waiting at a bus stop. You think this bus is probably running at this time of night, but it might not be (80% probability it’s running, 20% probability it’s not). If the bus is running, it comes every **40** minutes, but you have no idea when in those 40 minutes it’s supposed to arrive. After you’ve waited **15** minutes without the bus arriving, how has the probability that the bus is running at all changed? How has the probability that the bus will arrive in the next 5 minutes changed? 

(If it’s difficult to see the equivalence, imagine 40 minutes as 8 “bins” of 5 minutes, and that you can “check a bin” by waiting through it to see if a bus comes.)

I think that most people, if they aren’t thinking of this as a math problem and aren’t asked to give an exact numerical answer, will have a pretty reasonable grasp of the situation. As you search through the drawers and repeatedly come up empty, you start to think that maybe the shirt isn’t in the dresser after all, but at the same time, you’re not just going to stop searching the dresser halfway through.

***

I’ve purposefully chosen the values of the numbers to make it easy to think about the problem. There are 8 drawers in the dresser, and a 80% probability the shirt’s in the dresser at all, so before you start searching, you can see that there’s a 10% probability the shirt will be in any given drawer. You can slice the remaining 20% probability (that the shirt is somewhere else) into 2 “drawers” that each have the same probability of holding the shirt as a real drawer (initially, 10%).

So, after 3 drawers have come up empty, there are 7 total “drawers” left: 5 remaining in the dresser and 2 “drawers” somewhere else. So the probability that the shirt is in the dresser is 5 out of 7, or about 71%. Meanwhile, the probability that the shirt is in the next drawer is 1 out of 7, or about 14%.

You can even make a chart of the way those probabilities change as you search through the drawers:

![A chart showing that as the number of drawers checked increases from 0 to 7, the probability of the shirt being in the dresser decreases as follows: 80%, 78%, 75%, 71%, 67%, 60%, 50%, 33%. The probability of the shirt being in the next drawer increases as follows: 10%, 11%, 13%, 14%, 17%, 20%, 25%, 33%.](https://64.media.tumblr.com/203e8afa7c7231c44c113c767d111fb4/ba81d151568b9a70-4d/s1280x1920/8b7c4350918f396648fcb46ec3cce2af0a397f5e.png)

Or a graph:

![A graph of the same information: as the number of drawers checked increases from 0 to 7, the probability of the shirt being in the dresser decreases as follows: 80%, 78%, 75%, 71%, 67%, 60%, 50%, 33%. The probability of the shirt being in the next drawer increases as follows: 10%, 11%, 13%, 14%, 17%, 20%, 25%, 33%.](https://64.media.tumblr.com/012bb5f970ca35df62f6c1807884e270/ba81d151568b9a70-fc/s1280x1920/9b8e7708fd227e04e2ea1fe7b60ed08f1e4a77d9.png)

And if you think about it, of course those probabilities have to converge when there’s only one drawer left to search: the point when, if it’s in the dresser at all, it’s got to be in the next drawer.

If you fiddle with the numbers (the probability that it’s in the dresser at all, the number of drawers in the dresser), you get graphs that look slightly different, but the key point doesn’t change: as you progress through the dresser, the chances of finding your shirt in the dresser at all decrease, but the chances of finding it in the next drawer increase.

Hence our intuitive behavior: we keep checking until we run out of drawers, even as our suspicion is mounting that the shirt was never in the dresser to begin with.

You can also use Bayes’ rule to get the same numbers: treating “the shirt is in the dresser” and “the shirt is in drawer #n” as hypotheses, and each checked drawer as a piece of evidence, and calculating it that way.

***

All that said.

The thing I’m really interested in is the wildly incorrect answers people gave, not when they were actually asked to search a dresser, but when they were asked to think about this problem and put numbers to their answers. Only one in five respondents gave the correct directions for the blue line and the red line, never mind the exact probabilities. And some of the reasoning people used was … kind of buckwild. A good handful of people seemed to be following logic along the lines of “There’s a chance of the shirt being in the drawer and a chance of it not being in there, therefore I don’t know one way or the other, therefore the chances are 50:50.”

Lest you think I’m exaggerating, here’s one respondent’s explanation of their reasoning (they were answering the version about waiting for the bus):

> “It doesn’t matter that the bus didn’t arrive in the last 5 minutes. There is always a 50% chance it will come an a 50% chance it will not come.”

And another person’s:

> “There is no ↑ in probability it will come because there’s only 5 min left—there’s still a 50:50 chance it will either come or its doesn’t.”

Again, all this despite the fact that (it seems to me) most people have a pretty good grasp of the situation when they’re not asked to explicitly describe their decisions or their reasoning.

This kind of thing is what I mean when I say, “most of human cognition is opaque to us”. People are so bad at logical reasoning, even when their gut-level reasoning would take them most of the way there!

It does matter, knowing these things on an explicit, logical level (for example, if you want to share your knowledge with someone who doesn’t share your intuitive understanding!). And of course, these people probably would have given more mathematically correct answers if they’d had more of a background in math and probability. But it's also probably easier to think rationally if you're able to make more of a connection between the processes happening in your head on an intuitive level and what the explicit, linguistic part of your brain has access to.

I like things like differentiating between belief and alief, putting value on knowing what your gut-level intuition is doing even when you don’t endorse or agree with it. Emotions and intuition are logical processes that are frustratingly hidden from conscious observation … but they are logical processes. 
