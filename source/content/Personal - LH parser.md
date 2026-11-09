!! This is personal, and you can read it, but it has nothing to do with anything here !!

Stands for Lost-Hazard.

This is a special kind of parser, of which I hasn't seen any. It works by asking you to define priority on the different reduction you want to perform, and then just greedily reduce whatever it can, bottom-up.

Here's an example of a kind of grammar:
```grammar
100.E -> n
100.E -> E*E
10.E -> E+E
```

Rules with higher priority are meant to be parsed first.
This allow more simpler rules, we do not have to ensure that priority would be respected by increasing the number of rules.

# Implementation
Of course, a naive approche would be to just go through the code, again and again, and each time reduce the lower one found.
This way is really optimised.

- First thing we wanna do is, whenever we encounter a reduction, and that it has the highest priority, we can immediately reduce it, we are sure that there is no higher priority reduction that would fit (see ambiguity).
- Also, going through the whole list of lexeme every time take a lot of time, we can store not only the highest priority reduction, but all of them, in a priority queue. Then, we only have to go to highest scoring reduction, remove all appearance of this lexeme in other reductions (which is not the easiest part), reduce it, and append back to the queue the new reduction that appear possible.
- Once this done, we can be even more greedy on our first implementation process. If we keep track of which reduction score is higher, we know that if any reduction encountered is this number, we can immediately reduce. (Don't forget that new reduction might have a higher scoring value that our previous max, but this also mean we can immediately reduce the new one too).
- There's also a lot of optimisation on the first pass, using Boyer-Moore algorithm might help.
- We also want to be able to easily add all possible reduction for a situation.

For now on, that's all I've got.

# Ambiguity
There's a lot to say, but not so much time left to me.






# Grammar:
regexp:
```grammar
1000.E -> l
1000.E -> -
1000.E -> E*
1000.E -> (E)
100.E -> EE
10.E -> E|E
1.S -> E
```

the grammar itself:
See the itself implementation of https://en.wikipedia.org/wiki/Extended_Backus%E2%80%93Naur_form.
I'll make something like this, I think.
Okay, let's split the grammar between lexer and parser side:
Each non-terminal would either have only non-terminal rule, or only terminal rule.
Those with terminal rules would be put into the lexer.
Okay, the same way, we have something that describe regular expression, and with priority/
We transform those terminal rules into regex, and then we traverse the string, matching always the longest regex possible.






