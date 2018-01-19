# Good Teamplay

There are innumerable theories on what makes for good teamplay. Our years of experience in running a completely remote team, however, has equipped us with a certain introspection into this question. Thus, we have distilled the question into three main categories.

## Always Acknowledge {#acknowledge}

When you speak with someone face to face, you say something, and they nod. We use these non-verbal signals to show someone that their message has been received.

So how do we signal when we communicate over text?

### Repeat back in your own words

The most obvious way to show someone you've received their message is to use more text. Say "Got it", or "I understand", or something along those lines. This is fine for simple things. However, when there is a more complicated request a much better way is to rewrite the request in your own words.  This goes beyond just saying that you've understood something, and *proves* that you have. Example:

> **Alice:** hi @Bob, when you deploy the latest version you'll need to migrate the database.

> **Bob:** Got it, thanks. I'll migrate the db immediately after the deploy has completed

This technique of "repeating back" also enriches communication by helping to expose gaps. Notice how when Bob repeated back his understanding of Alice's request, he used the words "immediately after"? This might prompt Alice to add a little more detail to the instruction, like:

> **Alice:** thanks! But remember, you can't do it immediately after because you'll need to give some time for everything to sync after the deploy. Usually takes about 10 minutes, so check that it's completed first and then go ahead with the migration.

Conversations like this are the seeds of great documentation. For bonus points, Bob can offer to add some process notes to the wiki. Good on you Bob!

### Signaling in a group

The example above of rewriting things in your own words is good for one-on-one communication but is too noisy for a group. Even verbal acknowledgment is too noisy if you have several people all saying "Ok" after every message. Because of this, many group conversations lack a consistent form of acknowledgment. This is a shame, because if Bob says:

> **Bob:** hey everyone, I've added a wiki page with steps to follow when you need to do a database migration after a deploy: https://...

it's important for Bob & Alice to know that people have seen it.

Slack makes it so easy via emoji reactions to do low-noise acknowledgment in group conversations, so we should do this as much as possible. It doesn't even matter so much which emoji you use, it's really just about giving a signal that you have received the message. However, a general rule is to only use "positive" emojis. Obviously, a sad face, or even :thinking-face: is going to be a confusing signal. Thumbs-up is always a good way to start, but a bit of variety also helps to add personality.

## Conventions {#conventions}

Everyone in your team has had different experience in the past, and has learned to do things in different ways.  Agreeing on conventions must not be a theoretical exercise of deciding which way is "The Best", but a pragmatic approach to get everyone working in harmony.

### Start small

If you sat down and wrote out a list of conventions you've followed in the past, I bet we'd be here all day. You could cover everything from spaces VS tabs, to how git branches are named, to how we report bugs discovered in production.

Instead, just pick one and see if you can implement it in your team.

### What makes a good convention?

Before you propose a convention to your team, consider how it lines up with the following qualities.

Good conventions are Documented, Reasoned, Automated and Team-owned.

* **Documented**  
  Make sure you have a place to document the details of the convention that is available to all of the team.


* **Reasoned**  
  Where possible, give some rationale for why you are proposing this convention. However, avoid general statements like "Spaces are better than tabs because …". It's better to give reasons that relate specifically to the nature of the project in question.  And sometimes it's also fine to say that there is no compelling reason, apart from choosing something for the sake of consistency.


* **Automated**  
   It's not always possible to automate a convention. However, when you can, it's a huge win. Using a code linter in conjunction with CI or git hooks is great because it avoids so many "please fix your code" conversations.  Moreover, an automated code-formatter like prettier or gofmt means that everyone can produce consistent code without having to remember a bunch of (often) arbitrary rules.


* **Team-owned**  
  It's important that everyone feels they have some buy-in to the conventions your team takes on.  If you notice that someone seems unhappy with one of the conventions, try to discuss and find out how things could be improved. Always remember that the purpose of the conventions is to serve the team, not the other way around. So if one of your team members is experiencing frustration which can't easily be resolved, it might be better to discontinue the convention.

## Setting Expectations {#expectations}

How many times have you said something like: _"I fixed the bug, it should be working now."_

What's the problem with that? Fixing bugs is good right? The issue with the statement above is that it is vastly open to interpretation. The other person is likely to understand something very different than what we mean.

For example, if I say, _"I fixed the bug, it should be working now,"_ it might be interpreted as:

1. _"I've tested it, and can prove that it is working now"_

1. _"I changed something that should, in theory, fix the bug, but I don't actually know"_

When we think we are saying **B**, but the client thinks we are saying **A**, this is a recipe for massive frustration.  Every time a client hears a promise that a bug has been fixed, but continues to see a bug, they gain frustration, and we lose trust.

### Being Clear

Part of the challenge here comes from the necessity to fight against our own habits. So it's always good to stop and analyze your own words, and ask the question *"How might someone possibly misinterpret me here?"*

Beyond that, there are a few ways we can enrich our communication to set clear expectations.  Here are some suggestions.  When describing some work you've done, whether fixing a bug or implementing a feature:

1. **Be specific about what someone will see when they use the new version**.  
  E.g.:

    *Previously, when clicking the Login button the app would crash.*

    *With this update, when clicking the Login button the login form appears.*

1. **Be specific about how a reviewer can reproduce the same behavior** that you described in step 1.  

    * Are the changes deployed to a certain host?

    * Do they need to review the changes locally?

    * Are there any other steps to take before the changes can be reviewed?

    *This update can be reviewed here: https://staging…*.

    OR

    *This update can be reviewed locally. Remember to re-install dependencies and run database migrations.*

1. **Be specific about how far you've reviewed the changes yourself.**  
   Ideally, you'll always be reviewing your own work, but if for some reason you can't, it's much better to be honest than to cross your fingers and hope it works.  Also remember to include details about where you reviewed the changes. Reviewing locally is not the same as reviewing on staging.

    *I've reviewed the behavior as described above, on my local host.  I've been through the main user path, but if anyone is able to help cover edge-cases I would appreciate the help.*

1. **Provide proof.**  
  This might mean some quick screenshots, or even a short screencast, for more complicated scenarios.

All of these techniques support each other. Providing proof and describing the work in your own words help to set the reviewers expectations of what they will see when they review your work. Detailing steps to reproduce helps to avoid environment-related inconsistencies. Moreover, being clear about the level of testing you've already done will influence how surprised or frustrated a reviewer will be if they happen to notice something incorrect.

You are encouraged to use your own judgment about how much or little to apply these techniques, based on the nature of the work you are doing and the team structure.  But in any case, think about how to incorporate these four qualities into your handover notes, whenever you submit some work for review.
