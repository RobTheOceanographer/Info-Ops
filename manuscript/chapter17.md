## Chapter 17

Since we're going to be talking a lot about reports, diagrams, exercises, flows, and all sorts of things that can exist in various forms, I'm going to suggest a heuristic that we apply to the rest of our discussion.

![](images/diagrams-for-navigation.png)

That is, if it's a picture of something, whether it's a UML diagram, the Analysis Survey, a sketch of a new porch, a database model, or a snapshot you made with your phone of a wireframe workshop you had this morning? It's only purpose is for navigation, to find your way back to where you were before. If it's a physical item -- and we use the word "cards" here liberally -- it's for working together to update our mental model.

So if there ever was such a thing as a "generic, abstract business discussion", it'd go something like this: Diagrams are shown to establish context. Historical narratives are presented to remind those in the room of the things in the diagrams. Some kind of work is done using physical pieces that came from the diagrams and narratives. Discussion, netogiation, questions asked, answered, and put on the MQL). Progress is made (or not). Somebody snapshots the physical representation of the mental model. Later on the "pretty" version of the shared mental model is uploaded to a tool. Repeat and rinse.

There are ton of physical-based dicussion techniques. I'm a fan of Legos and Playdough myself, but there are a bunch more: model-storming, wireframes, role-playing, VR and AR-facilitated games, and so forth. You don't have to use cards. But cards don't hurt, either. You can certainly bring cards and put them out on the table or a wall and refer to them as use whatever other tools you'd like. It all has to go back in the model at some point, anyway. Both the beauty and the curse of Structured Analysis is that there is a place for everything.

### Analysis Paralysis 

While we're covering some ground rules to use throughout the rest of the book, we should also cover the bear in the room.

Wait, there's a bear in the room? RUN! RUN FROM THE BEAR!

(much later) Sorry about that. There was no actual bear.

What I mean is this simple question: How do I know when to stop analysis? After all, I read all of these super cool books that told me the problem with analysis is that it never ends. People use the term "Analysis Paralysis". That sounds awful!

First, the easy answer. 

Set up your work so that you are promising to do something valuable to the person that pays you every so often, like every day or every week. "Hey boss, every Friday I'm going to show you what I've made for you. You're going to love it and be happy you paid me that twenty bucks!"

That simple statement solves many problems. If you show up Friday without anything valuable, your customer should not pay you. If you only make little diagrams and play games, and your customer continues to pay you for that, then both of you are very nice people who are kind and sweet and don't know what you are doing. You seem to like each other, so go in peace. Just don't ever work for me.

Efforts exist to produce **value**, whether you are in a business, a club, a charity, or working on a personal project, if you're not producing value there's nothing to judge you by. So -- commit to doing something that a reasonable outside person would find valuable on a regular basis. There's nothing like a hanging in the morning to focus the mind.

Sidebar: nothing we've done should take that much time. Good analysis make take a long while, but *only when it is difficult to establish a shared mental model*. People can't show up for meetings but want the right of approval. People agree in the room but need alignment with their direct reports before they can commit. There's a disagreement over scope with antoher group in this same area. Good analysis can't take a long time. People finding stuff out and making decisions can take a long time, but that's true no matter what.

And if you're waiting on answers or external agreement, be prepared to wait. At the risk of sounding pedantic, it's either important or it's not. If we don't know whether this is being done by our group or the other one, if we don't have permission to provide anything of value, it's a dead stop. Otherwise it wasn't important for analysis in the first place.

The most common failure mode for junior analysts is mixing up the buckets and confusing *any* question with important questions. So I've seen analysis teams hung up for weeks on whether this button display should allow A, B, and C or just A and B. Dudes! That's a System Structure Realized question. Why are you working down in the weeds so far? Your job starts with Business Behavior Abstract. Ideally you'd scope out some Master Model work, *then start working*. That's kinda the idea. And you never, make structure an issue in analysis. (I should make a poster that says this. Sometimes I walk into team rooms where the backlog has items on it like "Customer Table". I die a little inside each time I see this.)

So, working at the appropriate level and in the appropriate bucket, you should have paths A, B, and C available to the behavior, *set when the system is coded or configured*, i.e., when the System Realized stuff happens. Which ain't you.

It is very rare not to get agreement at the Business Abstract level, and when it happens, it means you have chartering and organizational support problems, not analysis problems.

I don't want to fill this book up with a bunch of humblebrag war stories, but if you will allow me, I want to show you that I have serious experience in this area. I'm not simply throwing out slogans.

Many years ago I was working in Silicon Valley with a team of CEOs building out products. These weren't startup CEOs, these were *real* CEOs. There was a Fortune 50 company that wanted to form an incubator. Each of these CEOs had managed very large companies are were on a kind of sabbatical in SV seeing if they could build and launch a product. (The products were things that the various sub-companies had made but hadn't marketed)

Technically, there shouldn't have been much coding or detailed work, only setting various demos up and working with potential customers. How hard could it be? The entire floor was full of millionaires, all of which were highly praised by their various industries. They all believed in Agile and Lean and all of the other buzzwords.

Should be a piece of cake, right?

Nope.

The problem was like always: shared mental models. Everybody was a genius in a little box, like you'd buy down at Target (There's a genius-in-a-box section just beside the Turbo-Man dolls.) No amount of smarts, process, and attention-to-detail can take the place of a shared mental model.

We we had work to do. We formed up into small teams. Each team was required to stay in the same room with one another.

The CEOs hated this. And why not? They'd spent their life going for that corner office! Their last several years, they had dozens of direct-reports who were senior managers. They were responsible for organizations of thousands. Sit in a room with a bunch of low-level schmucks, including this oddball Markham dude from the hills of Virginia? My first team leader told me "I'm making million-dollar deals here with this product. I don't have time for this group."

But when I looked at the work, I had offshore groups that were clueless about why they were doing what they were doing, a CTO that was basically acting as a McDonald's customer, giving out to-do lists to everybody once a day, an attached tech team that tried to stay out of the crossfire, and a customer that was wondering where the actual product was.

And, let's not forget. The product didn't work. (Although the demo was freakin' awesome!)

So there was that.

We needed a shared mental model, just like every other business. Or we would die. Just like every other business. Once we gained and kept the model, the rest would fall into place. This wasn't a difficult thing, but if you put enough smart people on a project, it can get damned-near impossible.

To try to establish momentum, he and I met with *his* boss, which was kind of a CEO-of-CEOs. It was established that yes, you need to listen to Daniel.

Next morning he comes into the room. We do a little bit of work for 20 or 30 minutes, then he announces that he has to leave.

"Ok. We'll just be here doing nothing until you come back."

That got his attention!

He, I, and the team worked through all of our problems. I still stay in touch with them and consider them friends. They tell me that when I was out there, they finally realized how it was always supposed to work.[^17:4]

[^17-4]: The project still had bad problems, and I left after the initial engagement even though they wanted me to stay, but the problems were because of a lot of outside stuff we couldn't control, one of which was the very CEO-of-CEOs that called me out there in the first place! 

Sure, we had a few hours or maybe even a few days of analysis to do. But we didn't have analysis paralysis. We had a project that wasn't set up to succeed. (Chartering projects is coming up in the next section) We had work to do, real, valuable work. Without a shared mental model, we could certainly have a lot of activity and spend a lot of money, but we couldn't get the job done. So we stopped.

Turns out, "make something people want" along with regular accountability and teamwork does wonders for analysis paralysis. And without those things, it doesn't matter what you do as far as analysis anyway.

### Test-Driven Analysis (TDA)

But I have been falling down on my job! We've been several dozen pages and you don't have any new complicated-sounding terms or buzzwords to put on your status reports. So here's one: Test-Driven Analysis.

TDA says that all analysis work, initial customer conversations, screen discussions during app development, user experience and bug discussions -- all of it -- is geared to either creating or passing a test. We just need to be explicit about what those tests are.

Another way of stating the "easy answer" above is that the Behavior Bucket, as it is continues to develop, describes a test of future system behavior that represents our values (as expressed in the supplementals and behavior flows). Making those tests pass, either manually or through creating some kind of automated system, is the goal of any effort.

Doesn't that sound much better than "Git 'er done"?

We'll be expanding on that concept throughout the rest of the book.

### The Detail Is In The Files 

![.amout files are where all the details are](images/chapter17-mus-stargaze.png)

Much like Beethoven was able to use music theory and notation to create various works, Structured Analysis uses the same tagging system and the same Master Models to create all sorts of valuable things. EasyAM tries to stick with this concept. The standard output format uses the same syntax as the input format. And duplication is fine, even encouraged. If you mention the Behavior "Pet Cat" in seven different places, it's still the same behavior.

This lets us take all the tagged information and output it in a bunch of places, even though there is overlap. So, for instance, if you look at the Master User Story item "Stargaze" .amout file from our deck project, it mentions family, friend, and chair from the Master Domain Model. If you go to the .amout for those items, you'll find they mention "Stargaze" Repetition is fine.

You can generate a bunch of analysis notes over several months! If this happens, and there are several of you on the team, you have a few choices for how to organize things.

You might just make One Big Honking File, then keep it updated. This is how I got started. It works, but it is a pain. It's also why I wrote EasyAM, to handle all of that sorting and collating for me.

You might want to continue in the same fashion we have with our deck project, labeling each file by date, author, and title. That's the way I work now, at least at the beginning. Then I modify things a bit.

After the project kickoff, especially on a technology project, we need to start making stuff, so people get out their protractors, pocket protectors, slide rules, and programming environments.

EasyAM is a programming language. Just like any other. It should be treated the same.

So once we start setting up a "real" environment, with IDEs, compilers, build tools, and so on, EasyAM bolts right in. We set up an "Analysis" folder alongside the other project folders (at the top of the directory structure, of course, where else would it go?). We add it to source control, trigger it in our local builds, and put it in the CI/CD pipeline alongside everything else. (We'll be talking about that later)

In order to keep things as clean as possible, each time I make notes I create a file as before with the date-based naming convention. During the compile process, however, I rename that to use an .amin-old extension instead of a .amin extension. Then I rename all the .amout files to .amin files. In this way, EasyAM always keeps everything sorted, and when I want to know everything there is to know about something I just go to the file that has its name.

There are a zillion ways of doing this, which is kinda the point. As Dr. McCoy from the old Star Trek might say if he had my job, I'm a writer, not a DevOps genius! You'll probably come up with your own system. If you've found something cool, let me know! I'd love to share it with the rest of the community.

### EasyAM Language Guide

Interested in all the tags you can use in EasyAM? Here they are:

![EasyAM cheat sheet](images/chapter17-easyam-reference.png)

You can find the latest version of this on GitHub in the same place you found the EasyAM compiler.

### Changes

We have been cooking these last few chapters. We've covered setting up and using the EasyAM analysis compiler, we've used in on an actual project, we've talked about several different kinds of reports it creates and the beginnings of how to integrate it into simple projects. We talked about how to use it unobtrusively when there's conflict.

From there we talked about how to navigate your way around an entire abstraction level at once using the Analysis Canvas. We talked about some rules of thumb we're going to use throughout the rest of the book: "diagrams for navigation, cards for manipulation" and Test-Driven Analysis. It's going to be really cool to watch those two rules-of-thumb play out as we increase the difficultly level.

What about our deck project? What would happen if our customer, who has just built a shrine downtown in honor of the great work we've done, asks us to build a backyard playground? Do we start doing analysis work from the beginning all over again?

We do not. Same people, same mental model. Instead, we start with a survey of the new behaviors involved and then ask him if the supplementals still apply. The vast majority of the analysis model, which exists in all of our heads, continues to hum along just fine. In fact, because we've already synchronized, as long as we're careful to mind our knitting, the backyard playground project will be just as kick-ass as the deck was, maybe even more so.

What if we changed the team? What if a new guy joined? What if we had to use a subcontractor to do the work? What if there was a completely new kind of job, say our customer likes us so much he wants us to help him in house-hunting?

You ask a lot of questions, you know that?

Yes, these are excellent questions and we're going to answer all of them. Just not right now. Right now it's enough to do a simple EasyAM example.

The first question, however is so important we can't go any further without dealing with it: what to do when the people stay the same but the business situation changes? When new stuff comes into a team and it needs to adapt, it's easy to fall back into order-taking mode. After all, all these things are new now! Why don't you just tell me what you want me to do and I'll go do it.

Resist that urge.

In technology, we call getting organized around upcoming work and new information "Backlog Grooming", and it's the topic of the next chapter.
