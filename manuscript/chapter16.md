## Chapter 16

![The MQL puts all of our questions in one spot](images/chapter16-easyam-1.png)

Ok, here we go! Off to work now!

(Looks around)

So how does any of this Structured Analysis, EasyAM stuff do anything useful? Can we push a button and a deck come out of the printer?

Yes, actually you can. Just keep pushing the button. It'll come out eventually. Hang in there!

The work of analysis is creating a shared mental model. The good stuff is in our heads, not in a drawing in a tool somewhere. You could throw away everything we've done so far and probably a good job of building a deck. Likewise, you could run away to Paris in the Springtime, a new contractor could come in, and botch the whole thing up -- even if he had all of these notes. (Yes, I'm going to keep pointing that out because some folks will dive right into the "real" part of the book without knowing what the heck they're doing.)

So whatever work we've done? It's invisible. Like an invisible friend, only better.

Structure is derivative. Once enough Behavior and Supplemental information is in place, the structure "pops out"

In our case, we've playing with physical models that represent structure all along, ever since we printed out that diagram with the movable furniture pieces. We haven't had a meeting where there wasn't some physical stuff people could manipulate to play with structural ideas.

The analysis has done its job both the customer and us have a rock-solid shared mental model on how this deck is going to look and work. If required by building code, we'll draw up some blueprints and get a sign-off. Heck if we've been updating our online model as we go, that's probably already done. Otherwise we'll move on.

### Links

But wait! We forgot the links between items, how the supplementals impact the behaviors, how the behaviors use the domain model items. Hey, if we're going to learn all this crap we had better be using some of it!

Hurriedly, we go back and add all of that. We create a new file, "2018-05-07 dbm Linkages.amin" and put all of that in there. We do it with our customer there (Remember, we never, ever, ever add or change the model by ourselves. Cleaning up is fine, writing questions and notes is fine. Anything else? We all have to work on it together.)

We thought there would be no surprises, but nope. As soon as we started doing the work, we learned new stuff. Dang analysis. So here's how we add linkages in EasyAM:
```
MASTER BACKLOG
  ALL
  Cookout food
    AFFECTEDBY
      Easy-to-use
      Looks nice to the neighbors
      Reminds me of nature
    USES Food, Table, Chair, Gas grill, Family, Friend, Cabinet
  Nap in the summertime
    AFFECTEDBY
      Easy-to-use
      Must comfortably accomodate two large people side-by-side
      Must be impervious to weather for ten years
      Reminds me of nature
    USES Hammock, Recliner
  Entertain friends
    AFFECTEDBY
      Easy-to-use
      Looks nice to the neighbors
      Handle up to five people
    USES Table, Chair, Family, Friend, Hobby
```

We just re-list the item, then, for behaviors, we type "AFFECTEDBY" and a list of supplementals that affect it. Likewise, we type "USES" and a list of domain objects. All of this is exactly the material we went over in the last section, only typed into a text file.

We can describe the relationship either way. A behavior is AFFECTEDBY a supplemental, or a supplemental AFFECTS a behavior. Here we see how that works.

```
MASTER SUPPLEMENTAL MODEL
  Meets local building codes
    AFFECTS ALL
  Easy-to-use
```

Also note that since we're using "ALL", EasyAM knows what that means. We tell it that "Meets local building codes AFFECTS ALL", then all behavior will have that associate with it.

For a refresher, here are the linkages and keywords

<behavior> AFFECTEDBY <supplemental>

<behavior> USES <structure> 

<supplemental> AFFECTS <behavior> 

<structure> USEDBY <behavior> 

<one structure item> HASA <another structure item> or 

<one structure item> ISOWNEDBY <another structure item>

EasyAM doesn't care. Put the relationships in any way that makes sense to you. You can repeat the same stuff over and over again. It'll just skip it. Note, though, it automagically tries to figure out what you mean, so you misspell something, you end up creating a new thing with a misspelling. Then you have to chase that down, just like any other programming language.

Also note that you can only join to structure *through* behavior. Supplementals can't join to structure. That makes sense because without an associated behavior, supplementals don't have any meaning, therefore joining the two up doesn't make sense.

Our links are in place! Yay! You're probably still wondering how this helps at all, aren't you? I know you. And I'm watching you there in the back. 

I'll show you.

### Starting work

We have a structural model of everything we need and an EasyAM model loaded up with the basic model information. The next day we come to work with our cards and physical model and start doing deck-building stuff. I'm guessing it would involve footers. Builders seem to be crazy about footers. Never hear much about headers.

After a day or two, we've got footers in place and we're starting on the steps. The customer comes by.

"How's it going?"

"Great! Let me show you!"

You get out your cards and give a tour of how the work is progressing.

![The Cookout Food behavior card with full title, associated supplementals, and domain links](images/chapter16-easyam-2.png)

You walk over to where the grill will be. What you're doing here is walking through the analysis you've already done together and pointing out how the derived structure fits into all the constraints. There should be no surprises!

To the customer, however, it just looks like you are smokin' hot at knowing what your job is.

"Over here is where the grill will be, like we discussed. Your grill fits right in here and should no problem feeding up to five people, maybe twice that. (glances at card again). Nothing complicated here. You know, "Big Bubba" (his pet name for his grill) is going to look sitting there. The dark color will sit mostly behind the rail, looking like a shadow from the treeline. I don't think the building inspector will have any problem here."

Then you walk him through the flow.

"So you reach into the refrigerated cabinet, to the left beside the grill, grab your burger and dogs and fry 'em up. When they're ready, you turn around, walk six feet and put them on the table. If a couple of friends want to help you cook, there's plenty of room."

That's the really detailed way of doing it. The laziest way, and what I would probably do, is just stand there and point at the deck going through the behavior list -- but I would use structure terms. Remember: you want behavior, you talk about structure (or supplementals)

"Over there is where the steps will go (enter and leave). The grill goes here. (Cookout food). Hot tub's there. Hammocks right beside it. The table is big enough for all of your games, and there's plenty open space, easily enough for you and your friends to stargaze."

That covers the status of the project in two minutes.

Every day or so, you repeat and rinse. Point to System Realized Structure stuff, talk about how it's changed in the last day, what problems you're having, and what your plans are for tomorrow. Be sure to cover all the behavior as you do so.

At the end, you could some kind of formal walkthough or hand-off, but why would you? You've made sure there's no gap in understanding between you or the customer, and you both know where everything is and more importantly, *why things are made the way they are.* So there's nothing to approve. Go out and get a beer or something.

But let's say the first day, as you're pointing at stuff, when you point at where the stairs go, the customer says something like "That's not going to be wide enough at all"

What do you do? Do you ask exactly wide they should be?

Maybe. I'd ask "Why?" Because I'm really interested how the customer and I have such different ideas about this. Changing the deck is easy. Continuing to live on different planets is painful. The misalignment problem is much more important than the mistake.

He might say something like "Well, I need my three heavyset friends to be able to walk up the steps at one time."

You take a look at your card; not because you're trying to determine exactly what was said. Analysis isn't specs, remember, but because you want to remind you and him about the conversations, figure out what happened.

![The Enter and leave behavior card](images/chapter16-easyam-3.png)

"Yeah, I'm looking here. I've got that the steps (reading) 'must comfortably accommodate two large people side by side'. We talked about that the first couple of days, didn't we?"

You've pointed out the supplemental linkage and asked if he remembers the discussion. Let's say he doesn't. So then you pull out the 'two large people' supplemental card.

![The two large people supplemental card](images/chapter16-easyam-4.png)

Now you're looking at all of the touch-points regarding this supplemental. Your "conversation library", aka formal, written analysis model, is starting to save your butt.

"Yeah, ok. We talked about this last Thursday, right? When we talked about taking naps in the summer, you mentioned that you wanted your two family members to be able to use the hammocks. We talked again about them using the hot tub and telescope. Remember I showed you these notes about how ten feet would be enough?"

Whatever happens now is fine. Maybe you missed something. Maybe you didn't. In either case, you're able to pick up a model card, look at what's joined to it, then read those notes and questions, reminding both of you about all the great times you had back in the day. The written model has done its job.

What you will find is that the more you use EasyAM in a reasonable and constrained fashion, the quicker the model becomes smarter than you are. That is, it remembers a ton of stuff that everybody else forgets. And it has enough linkages and annotations that with a little bit of reading, you can find yourself back in the same spot you were a month ago discussing a topic with as much (usually more) context than you had back then.

If this drags on longer than a few minutes, you can run another set of cards, get out the modeling toys, and have a bit of continued analysis, just like you did before you started. (For the record, I have never had this happen. Usually just taking a few minutes and poking through a few cards, we're good to go.)

This is way cool. The more you see this happen in your practice, whatever you're using it for, the more it will seem like magic. Compare that to the usual way of trying to "capture requirements" Yuck.

10/10 highly recommended. Would do again.

### To-Dos, WORKS

For each item, we've talked about adding questions, notes, even diagrams. But there are other things you might want to stick on your items.

**TODO** The name covers it. Put stuff in you want to be reminded to do later

**WORK** If you want to capture work you've done on the item, say for billing purposes, this is the tag to use. (This isn't a work-tracking system. It might be relevant to future conversations to say something like "WORK: I spent all last week trying to determine if those giraffes could swim! Giraffes can't swim!" We'll know to tread gently the next time we talk about giraffes.)

There are three other ones, **DEFECT**|**BUG**, **DATA**, and **CODE**. They do a bunch of stuff. We'll cover those later in automation.

Here's our Stargaze behavior with a couple of these added:

```
MASTER BACKLOG
  Stargaze
    AFFECTEDBY
      Easy-to-use
      Must comfortably accommodate two large people side-by-side
      Handle up to five people
    USES Family, Friend, Chair
    DEFECT Outside security light prevents good stargazing
    WORKS Spent six hours on the phone with an astronomer from Hershey. There's no fixing the light problem
    TODOS Call the city to see if the light can be moved  
```

And here's our new Stargaze card.

![The Stargaze behavior card after adding a bug, a work, and a to-do. (Nothing changed)](images/chapter16-easyam-4.png)

Wait! There's nothing there.

Correct. That's because these model cards are for a single purpose. They're not for keeping track of everything. Once you know the full title, open questions, notes, and linkages, you should have enough context to either do whatever your work is -- or dive deeper somewhere else.

This is a key part of all the automation we'll be doing: delivering the right amount, but also the minimal amount of information needed for whatever the job is. There is a place you can go to see everything about an item -- but it's not a place that you would use to do any work. Remember: the tool, even if it's a bunch of cards, is not the work.

### The Analysis Canvas 

This gets us to a bit of a thorny problem that I've been struggling with for years: how do you handle and display all of the items at any level of the Analysis Pyramid (Business Abstract, Business Realized, System Abstract, System Realized)? The purpose of our tagging system is to create a "Library for Conversations", and the tags give us all that we would ever need to organize and sort stuff, but where's the little map of the library? All big libraries have little maps you can look at to get yourself into the right spot. Where's that?

Diagrams are the only answer. Whether it's a floorplan or a roadmap, diagrams help get you quickly oriented and pointed in the right direction. So let's make a "map" to show how our three buckets work together on our deck project.

![This shows us the people we're trying to help and how we're trying to help them](images/Chapter 16 UC Model.jpg)

Our version of the Use-Case model isn't a bad place to start. It's simple. It kinda shows us why we're here. But it doesn't really show what we're doing. We could add in Activity Diagrams for all of our behaviors, but then we're really just talking about *what we do*, that is, the desired behavior of the target system [^16-2]

[^16-2]: Of course, there are always the temporal indicators: was, as-is, and to-be. Most of the time I'm going to skip those and just talk about the to-be case.

Well heck, how about our Supplemental Model?

![](images/Chapter 16 Deck Master Supplemental Model.jpg)

That's even worse. It's good stuff. It just doesn't tell us how to get anywhere. It doesn't orient our mind to dive into a discussion quickly.

Ok. So how about the Domain Model?

![](images/Chapter 16 Deck Domain Model.jpg)

Same thing. It's not that these diagrams are bad, they just don't help orient us. These diagrams are about *how items in each bucket relate to other items in the same bucket.* Useful for looking at an entire bucket at a time, just not an Analysis Level.

So let's throw all three items into a diagram, like so.

![](images/Chapter 16 Deck Overview1.jpg)

Better. It certainly looks more impressive! Lots of boxes of different shapes and lines. We could probably even do something with the font, maybe add in a drop-shadow.

So --- not so much.

It's the linkages that matter. When you are orienting yourself around an item, say a behavior, the use-case diagram is where to start. Find the bubble. Find the stick figures with lines to the bubble. Now you know the test and who you're changing the behavior to make happy. But what about the supplementals that affect the behavior? The words used in describing the behavior. You could go to those models, find out things about how supplements work with one another, or how the important words we use are related to one another. But you still don't have the links. It's the links where the magic happens.

Ok, dang it. Let's draw the lines in! I've got a drawing tool, dang it, and I'm not afraid to use it!

![](images/Chapter 16 Deck Overview2.jpg)

Ooof. That's a mess. Although if we had a plotter and generated a wall-sized diagram, it might work. It's just not very useful for carrying around with you or putting on a cubicle or team wall.

When I first started using Structured Analysis, I kept everything in diagrams and used a UML modeling tool to handle linkages. (UML modeling tools are different from the kinds of drawing/diagramming tools most people use. With a tool made specifically for UML, you should be able to re-use the same thing in multiple places. The tool keeps track of all the links behind the scenes.)

This wasn't bad, but it led to lots of meetings where I was futzing around with the tool trying to find the context instead of actually participating in the meetings. At times, I'm sad to say, I ended up working in the UML tool while everybody watched.

This was as exciting as watching paint peel. The only thing that kept me from going down the full path to perdition was my insistence that I would only update the model with the entire team in the room. As a group, we simply wouldn't put up with a bunch of diagramming using a projector, so I kept things simple simply because the team would have shot me if I had pushed things too far.

After that, I tried just printing the detail pages of everything on a certain level and sticking them on the wall. When I add the diagrams for the three buckets shown above, it works. Takes up a lot of space, but it works.

Over the past couple of years, as I have taught Structured Analysis to teams all over the place, I have been developing **one chart to rule them all**, my idea of a single diagram to get you oriented and working as quickly as possible.

![Behold, the **Analysis Canvas!**](images/AnalysisCanvasInfoGraphic.png)

Eventually EasyAM will output something like this, once the industry has banged it around enough that we know it makes sense. For now, if you're interested in creating your own Analysis Survey, there are instructions in the appendix. (It's not that hard to do, but plan on it taking a few hours)

The key thing that I expect to hold with all revisions of the survey is the overall plan for how to read it, which is called out in the boxes. 

Behavior should generally stay to the left, since that's what scopes projects. Supplementals stay to the right because they control the quality of what we do. Structure is in the middle because it's the tension between behavior and supplementals that determine and validate structure.

For any level, there are the things "outside" or "above" it. That should be at the top. There are the things that go inside our minds as we created a shared mental model. That should go in the middle. There are the interconnections between the buckets where the magic of Structured Analysis happens. Finally there are "downstream" impacts, other groups, machines, teams, and people that are impacted every time our mental model changes. That should go at the bottom.

This is something I've made up. It's good enough for now. It's far too busy for a standard-sized piece of paper, but it should work on a printer that prints tabloid or A2-sized paper. It needs improvement, but you should be able to pick anything that you're talking about, walk to a printout of the Analysis Survey on the wall, and within 10-30 seconds know all of the other things that touch on it and the things it touches on. And that should be true for anybody in the team. (This is what I would consider to be the acceptance criteria for the diagram) I'm looking forward to seeing it evolve over the next few years!

We have built a deck and our customer loves it. Now let's talk about lessons learned and how we can take the analysis work we've done so far on the deck and continue to use it. 