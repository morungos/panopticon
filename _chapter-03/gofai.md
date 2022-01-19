---
title: "Good old fashioned artificial intelligence"
order: 60
---

Early work on artificial intelligence depended heavily on symbol manipulation.
For example, in language, each word would typically be a symbol, and we 
might use rules that look like:

    if 
        word[t] = 'artificial' and word[t+1] = 'intelligence'
    then
        ...

In this, the computer (obviously) doesn't actually know what words like
"artificial" and "intelligence" truly mean. But, that doesn't necessarily
matter. With a little care, we can create programs that mimic intelligent
behaviour very quickly.

A good example is Weizenbaum's ELIZA, the first chatbot, and a program
sufficiently engaging that it did manage to engage users into 
extended conversations of a kind. ELIZA used a set of rules and patterns,
much of which would echo back what people typed in. A typical dialogue 
with ELIZA would look like this:

> Woman: Men are all alike.  
> ELIZA: In what way?  
> Woman: They’re always bugging us about something or other.  
> ELIZA: Can you think of a specific example?  
> Woman: Well, my boyfriend made me come here.  
> ELIZA: Your boyfriend made you come here?  
> Woman: He says, I’m depressed much of the time.  
> ELIZA: I’m sorry to hear that you’re depressed.  
> Woman: It’s true, I am unhappy.  
> ELIZA: Do you think coming here will help you not to be unhappy?  

In ELIZA, this kind of behaviour is essentially built entirely from three
different kinds of rules.

1. Pattern rules, that detect phrases like "I am X", and generate an 
appropriate response, like "I am sorry to hear that you are X". As above, 
the computer doesn't understand what X is, so you could literally type, 
"I am an avocado sandwich" and ELIZA would likely respond, "I am sorry to
hear that you are an avocado sandwich".

2. Default rules, that nudge the conversation back on track when all else
fails, e.g., the "In what way?" in the example here.

But, Weizenbaum used a trick! ELIZA modelled a very specific type of
conversation, involving a client-centered, Rogerian, counsellor. Rogerian
therapy is very structured, and reflection is a key part of that structure. 
So this reflecting back of of dialogue is exactly what would likely happen
in a typical client-centered session, but it is not at all realistic of 
normal everyday conversation. In effect, there is a context to the whole
interaction which makes it work in this specific setting, but which makes it
very fragile.

Developing these kinds of applications took a lot of work, especially when we
start to look at human expertise. For example, imagine we are building a
program to detect faults in power stations. The same basic approach, using a
collection of specific and general rules, can work very effectively. But
identifying those rules can be extremely hard, especially as one of the more
intriguing parts of human expertise is that we often find it hard to articulate
our expertise. Imagine, for instance, having to tell somebody how to ride a
bicycle, or know when a pizza is cooked, or when an message is sarcastic. Even
in technology, which you might think of as a field driven by logic, people use
terms like "code smell" to refer to this *tacit* knowledge.

For a while, these systems were still worth building. Sometimes the payoffs
were so good that it was worth investing years of effort capturing the
expertise. And tools and methods were developed to ease the process. Eventually,
though, there was enough disillusionment that the second AI Winter set in, and,
for the most part, work on symbolic approaches to artificial intelligence became
less popular.

Having said that, it's important not to underestimate the impact of artificial
intelligence on modern technology. Many of the innovations that power modern
computing trace their history directly to artificial intelligence. For example:

1. Object-oriented programming came directly out of artificial intelligence
   work in the 1960s, through Alan Kay's involvement.

2. In many respects, modern language like Python and JavaScript are direct
   descendants, with slightly different syntax, of the Lisp family of 
   symbolic artificial intelligence languages.