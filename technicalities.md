# Technicalities {#technicalities}

Despite the general aversion to systematization without reason, there are some processes that are simply unavoidable. The following are the few things that you must know and follow for a good X-Team experience.

## Journaling {#journaling}

There comes a time in every person’s life, when they think to themselves, “I should write a book.” And while writing a book is something that takes forever, there is something else that I have in mind. No, it’s not a blog either \(though if you write one, Ben will be happy to give it a look and push it online\).

What I’m talking about is writing a journal. No, not one you start with “Dear Diary...” It’s much closer to \`Captain's log, stardate 2017-09-10\`. And I promise, it’s not about me just wanting to put more work on your shoulders. It’s actually about, well, this:

[https://www.youtube.com/watch?v=dnzE9ip5U04](https://www.youtube.com/watch?v=dnzE9ip5U04)

And, before you ask, no, I am not calling you a slacker.

See, there are two distinct objectives when writing these X-Journals.  
The **first one is for the team you work with at the partner** to be able to see at any time, what you’re working on, how you’re progressing, etc. There might be daily or weekly standups, but nothing communicates competence like a journal of achievements you can always point to or which they can always check, when in doubt. This is the journal you may or may not already be writing. It is pretty much a summary of your daily work, and it should be primarily accessible by the **team that works with you on the project**. It should include things like what tickets you worked on, what problems you ran into and how you solved them, what you learned that day...

The **second one is for us, Unleashers \(Ben, Jacek, Karol\) and your account manager \(the guy that told you what project you’ll be working on\)** here at X-Team. This journal is a copy of the first one **with additional reflections** on any and all characteristics of the project you’re working on — to reflect on project health, so to speak.

* Is there a ton of issues that aren’t being tackled and your suggestions are being ignored? Put it here.
* Is the client’s communication erratic or hard to follow? Are the goalposts being moved all the time? Put it here.
* Does the client not provide you with what you need to be able to do your job? For Flying Spaghetti Monster’s sake, PUT IT HERE!

**Basically, this second journal is here so we know what is going on and can step in and help solve problems before they evolve to their final form.**

And if you are worried about how “complaining” is going to come across — None of us Unleashers have ever seen or heard of anyone getting in trouble for expressing objective criticism. Obviously, it has to be professionally done — like putting it in this journal and/or messaging us and/or your account manager directly, but you will definitely not be penalized for it. If anything, “comparing notes” from several X-Teamers on a project could be helpful in potentially improving the work environment for everyone.

### Step I/III {#journaling-i}

So, now that you’ve read all this, if you’re not keeping an X-Team journal yet, I would like you to create a private channel like e.g. \#journal-john,invite the unleashers\(Ben, Jacek, Karol\)and your account manager\(that can be either: Brad, Jake, Josh, or Luke\), and create the first, Hello World! post, which should include a simple introduction of yourself, with things like:

* What are your usual working hours \(and timezone\)?
* What is your preferred work environment? Beaches, mountain cabins, cafes, your own comfy bed...
* What does a normal day for you involve \(no need to share anything personal you feel uncomfortable sharing\)

_PROTIP : If you need an example journal take a look at \#samuel-pepys-journal_

### Step II/III {#journaling-ii}

It’s time to share with you a new journaling technique called TIL \(Today I Learned\). Through the years we’ve established that there’s nothing that builds trust with partners like some good old transparency and sharing of knowledge. That’s why we want you to implement this technique in your daily routine. Here’s your second assignment and, as usual, let Ben, Jacek, or Karol know once you’re done.

#### TIL

##### What is a TIL?

TIL \(Today I Learned\) posts can be really short. They show one thing you learned while working on the project.

Sometimes, it's something very specific to the project, like a significant requirement that you found while digging through some docs. Another time, it's more general info that you discovered or remembered along the way, like a debugging technique or a handy bash trick.

##### How to write a TIL

Start looking for those little "learning moments" in your day and quickly jot down some notes in your journal \(the client journal that also gets copied for us\). Remember, keep it quick & raw. If others read it and have questions, they can ask for more info.

Try to keep it down to a couple of sentences and maybe a code snippet or screenshot.

**Exercise: **Try making a couple of TIL posts during your working day.

##### Why do we often avoid this?

It's easy to fall into the trap of thinking"I won't share that TIL, because everybody probably knows it already, and I will seem dumb!”Or“What if I'm wrong and there's actually a better way to do it??"

As a wise commander once pointed out, _"It's a trap!"_

Just do it, and everyone will thank you later.

##### Why should we do this?

Let me address those 2 fears:

_"Everybody probably knows it already"_

Who cares :\) Maybe they do, but maybe they don't. Only someone very arrogant will think badly of you at this point. That's their problem, not yours.

_"What if I'm wrong and there's actually a better way to do it?"_

Again, don't let this stop you. If somebody else knows a better way, this may be your golden opportunity to learn it! They might have been avoiding sharing this knowledge for the very same reason described above! This is your chance to break the cycle.

##### Example by Josh

The other day I was reviewing pull requests on a github project, I and remembered a handy way to review them locally. I wrote it as a quick "TIL" entry, and since there's no sensitive businesss info there I also posted it to twitter:[https://twitter.com/joshwnj/status/855215578042073088](https://twitter.com/joshwnj/status/855215578042073088)

In a couple of days it had 13 retweets and 9 likes. That's nothing groundbreaking, but if there's a handful of people that found it useful, it's totally worth the 2 minutes it took him to do it.

### Step III/III {#journaling-iii}

It’s time to share with you another great journaling technique about reflections. Once you gather some entries in your journal, they are a great resource to reflect upon and make improvements.

#### Reflections

Having done hundreds of code reviews, we've found reflections to be a very helpful process to learn about good programming techniques. Sometimes, we review some code, and instinct tells us it is "good" or "bad".

The next step is to try and articulate why. Is it just written in a style that goes with or against our personal preference? Or is there some deeper reason?

I encourage you to use code reviews as an opportunity to write new journal entries. Writing "reflection" entries is similar to TIL, but rather than learning something new the focus is on describing something you observed and why you liked / disliked it.

#### Reflect on your own code

It's helpful to write reflections on your own code as well.

We don't always have time to complete everything to the level of perfection we hoped, so this is an opportunity to add more context to any rough edges you may have had to leave behind.

* Think about future maintainers of the code, or other people doing similar activities in future. Are there things they'll need to keep in mind, or things that will make their job easier?

* If you were to implement this feature again in future, are there things you would do differently?

* Any known tradeoffs or pros/cons of the approach you took, especially if it has impact on other parts of the system.

* Finally, did you observe the golden rule of coding? I.e., _“Always write code assuming the next person that’ll work with it is a violent psychopath that knows where you live.”_

## Invoicing & Time Off {#invoicing}

First, our invoicing period is **two weeks**, which means that, every two weeks, you will have the opportunity to submit your invoice with the total number of hours worked, reimbursement requests and other things, explained below. You will receive a notification about the beginning of the invoicing period per email and also on your google calendar for your X-Team account. If you do not receive any such notification by the 3rd Friday of your joining a project, contact Mike \(@mikerhoads\) and he’ll help you out.

Once you receive the invoice period notification, go to [https://xteamdevs.appspot.com/](https://xteamdevs.appspot.com/). There, you will find your payment profile, which you’ll have to fill out the first time you’re there. On top, you have the options to _**Request Time Off **\_and _**Submit Invoice**_. The former is self-explanatory, so let me just add that you should always, if at all possible, _**request time off at least 1 month in advance**\_, preferably more.

The Submit Invoice button is the more important one at this point. When you click it, you’ll go through a 6-stage process.

1. **Announcements**  
  Here you will find some company announcements like the begin of XOutpost registrations, the Lit Beacons — when we are looking for specific profiles you could get a referral bonus for, etc.

2. **Basics**  
   Invoice date, option to upload a PDF invoice \(you will still have to fill out everything\), and notes.

3. **Hours worked**  
   A list of projects you can invoice the company for and the agreed hourly rate. Enter the number of hours you worked in that period.

4. **Reimbursements**  
  Here you can put in for any reimbursements you may wish to claim. Some examples would be Unleash Budget reimbursements, GameClub reimbursements, FitQuest reimbursements, referral bounties etc. This would also include reimbursements for education, conferences + related expenses, certain project specific software that’s required etc. If unsure, whether something fits, ping [@ben](https://x-team.slack.com/messages/D23Q0MCQ6).

5. **Survey**  
   Here you’ll find a few questions on how things are going for you in X-Team. There are no right or wrong answers here, just be honest, so we can help make things better if something is suboptimal or feel content that we’re doing a good job if everything’s fine.

6. **Banking info**  
  Here you get a last chance to fix any mistakes in the recipient details for your salary. Double-check everything, hit Finish, and wait for the money to show up in your account. As a general guide on the transaction speed - barring public holidays, the money usually arrives in my EU bank account by Friday after the invoicing period.

And this is really all there is to it. If you’re experiencing any kind of problems with your payments, just talk to Mike \(@mikerhoads\) and he’ll help you out.

## Unleash Budget {#unleash-budget}

You didn't think we'd forget about this, did you? This jewel is the equivalent of 2500 USD per calendar year, which are there to keep your skills current, your body fit, your mind sane, and your entertainment desires tickled. There are several categories of expenses you can use your Unleash Budget for:

* \#photography-club — up to $50/month toward photography equipment
* \#productivity-quest — up to $20/month on any productivity app
* \#game-club — up to $20 on any game/month
* \#fit-quest — gym membership
* \#courses — any paid course
* \#conferences — ticket, travel, and/or lodging for any paid conference \(including \#unleashconf\)
* Health & Wellbeing — anything that helps you relax and recharge your batteries

Unsure of whether something you want to get fits in to one of these categories? Chances are it does, just shoot a quick ping to [@ben](https://x-team.slack.com/messages/D23Q0MCQ6) to find out.

