So, about entity, there's a lot to do.
We want an entity to have: a number of component, a list of component identifier+length:the component.

The big question is, does we make the component size compile time known?
If yes, that make things easier I think, that basically prevent component from extending, and make managing them internally easier.
But then, there's no adaption in size from the component.
Is that really bad? Maybe. Not for my Os.

The only problem is rust, which does not like this kind of structure, and I wonder if I should switch to C for this kind of operation.

What I want to be able to do:
I'll have a structure that reference all entity that have a specific component within them.
That's should be okay to do.
Then, we want to gather all specific component from some entity.

If we make them fix sized, that allow us to sort components within an entity..
That's good.


Okay, we make them size fixed, and then we have an architect that store in a sorted list which component it stores, and take reference to them.
Then, components are just data, packed.

When we want to get 






