---
title: Get to Know HTCondor Core Developer Cole Bollig

author: Malia Bicoy

publish_on:
  - htcondor
  - osg
  - chtc
  
type: news

canonical_url: "https://chtc.cs.wisc.edu/cole-story.html"

image:
  path: "<https://raw.githubusercontent.com/CHTC/Articles/main/images/cole_beads.jpeg"
  alt: HTCondor core developer Cole Bollig
  
excerpt: Learn about HTCondor core developer Cole Bollig!

---
<figure class="figure float-end" style="margin-center: 1em">
  <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/cole_beads.jpeg' height="474" width="700" class="figure-img img-fluid rounded" alt="Cole wearing a snazzy pink shirt.">
</figure>

**What kind of work do you do for CHTC?**

I’m one of the core developers for the HTCondor Software Suite (HTCSS). 
It’s a lot of coding, development and bug fixes. I also participate in 
meetings for various collaborations like the LIGO organization and FermiLab. 
The bulk of my work, however, is developing the HTCondor software. I have a 
specific focus on DAGMan, as I’m the quote-on-quote “DAGMan expert”.

**How would you define DAGMan?**

DAGMan is a HTCSS tool, which assists users in automatically managing workflows 
of HTCondor jobs. In the complex, modern world of computation, it makes sense to 
break complex workloads into smaller organized steps where a user has a job that 
requires the output of another as input. Theoretically, a user could sit on a 
computer, submit the first job, and wait for said job to finish before running 
the next job in the process to achieve a bigger task like sequencing genomes or 
analyzing gravitational waves, but why not let HTCondor take care of that? Enter 
DAGMan, DAGMan allows a user to describe the steps/jobs in a workflow as nodes and 
create execution dependencies between them via edges so a job is not executed until 
all of the other nodes it depends on complete successfully. Describing these nodes and 
edges is what creates the technical computer science jargony concept of the directed 
acyclic graph (DAG) the tool manages. Meaning DAGMan is a DAG Manager. While the base 
concept of DAGMan is to automatically manage a workflow for the user, DAGMan is also 
equipped with many useful features to assist the user in their research.

**Why did you want to join the CHTC team?**

I graduated college and had been applying to a lot of places. This position seemed 
well-fitting because it had a C++ focus, which I prefer to program with. The job 
was also affiliated with UW-Madison — a trusted place — and I fit the requirements. 
I was really ecstatic to even get an interview, to be honest. Getting a job in the 
computer science field can be a bit rough as a fresh graduate. I will say, after 
two years of working here, it’s been great. I’m all for CHTC.

<figure class="figure float-end" style="margin-center: 1em">
  <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/cole_tree.jpeg' height="405" width="400" class="figure-img img-fluid rounded" alt="Cole posing with some trees.">
</figure>

**What’s your favorite part about working at CHTC?**

I don’t know if I could single it down to one thing. For one, it’s a really cool group 
of people that I work with. Whether it’s directly on the team at CHTC or indirectly 
through an organization, they’re all awesome and do great things. It’s a very nurturing 
environment. As for HTCondor, it’s crazy to think about distributed high throughput computing 
software as a nerd myself. I’m very appreciative to work on something so cool and nerdy. The 
top aspect I enjoy, however, would probably be the gratification I get from the work we do. 
As a software engineer I could be working at Facebook or Google to create a new obscure feature 
that a few people interact with and feed the pockets of Mark Zuckerburg. Instead, I’m helping 
the scientific community. It is very gratifying to know that me clicking away at my keyboard 
all day is actually directly impacting science.

**What is the most challenging part of your job?**

The unknown. We’re actively developing the software. We don’t know where things are going 
to be tomorrow. We can plan as best as we can, but it’s a lot of learning as we go. Another 
challenging part is the code is a bit archaic at parts. It’s challenging to figure out what 
the code is doing and how it can improve. Even in the improvement sense, we don’t know what 
the research of tomorrow will need until it’s today.

**What do you think is the most exciting development happening right now?**

For me personally, it’s delving into the DAGMan code. I am the expert. It was pretty 
stable when I got here, but I keep looking at the code and thinking about new ways it 
can be improved or bringing it up to more modern standards. Another focus is DAGMan 
handling various authentication methods — especially tokens — based technology. It’s a 
bit of an issue right now, but over the next year or so, I hope we can iron out the details.

**I heard through the grapevine you go by “Dag Boy” here at CHTC, what’s the story behind the name?**

The name comes from my fellow core developer [Greg Thain](https://chtc.cs.wisc.edu/people.html). 
My first day here, one of my previous office neighbors came over and said, “Did anyone mention 
I’m leaving and you're taking over all my responsibilities?” Which I, of course, had no idea was 
happening, but he quickly got me up to date with the basics of DAGMan. I was young, and newly in 
charge of DAGMan — I couldn’t have been an expert by that point. Greg started calling me “Dag Boy” 
because I still had to grow up, and it stuck.

**What social event with work friends have you enjoyed the most?**

There’s a lot. We have a HTC week every year, for one. I get to directly interact with users and 
admins of the HTCondor software. On a smaller scale, we have Condor Fun Day. It’s just CHTC people 
hanging out, cooking food, and drinking a little. There’s also daily things. Some of us go to Big 10 
for lunch every Tuesday. They have three dollar sloppy joes. On Fridays at lunch, we have a little 
group that plays Sheepshead in the conference room. There is never truly a dull day.

**HTC24 will be coming up this summer. Can you tell me about that and what you like or don’t like about it?**

A dislike is that it’s a lot of setup. Putting together a conference that people from all 
over the country come to is never easy. At the end of the day — end of the week actually — 
it’s a great experience. The effort is truly worth it. Meeting all those people and doing all 
the social stuff afterwards is great. Last year, a group of us went out kayaking and 
paddleboarding on Lake Wingra. We just got to socialize and have fun. You can learn a lot too. 
It’s not just about the social aspect, there’s also the technical aspect. We get to tell our 
users about all the cool stuff we made, and they get to tell us about all the cool stuff they 
did with our cool stuff. It’s a nice cycle.

**I hear you are involved in the CHTC Fellows Program. What is that about?**

It’s a new thing we’re trying out this year, and we hope to continue it in future years. 
It’s a step up from a standard internship. We took the setup from the Google Summer of Code. 
We’re trying to get students who want to learn in our environment and develop specific projects 
that they want to work on. It’s a chance for them to get experience in a distributed high 
throughput computing environment, and we can test features out that we might not otherwise 
have had time for.

**What’s changed since you began working for CHTC?**

The biggest change — other than moving to another building in the future (does happy dance) — 
is the code. We’re actively adding new features, but my favorite pastime is helping to update 
HTCondor to modern C++ standards. The code has been around a long time and some parts predate 
the C++ standard library. We’ve been slowly updating HTCondor throughout the millions of 
lines of code.

<figure class="figure float-end" style="margin-center: 1em">
  <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/cole_pose.jpeg' height="263" width="800" class="figure-img img-fluid rounded" alt="Cole at the Terrace.">
</figure>

**You received a Bachelor’s in Media Arts and Game Development from UW-Whitewater, do you create or play video games in your spare time? Tell me a little about that.**

Yes, I am a gamer. I have three Xboxes, a Game Boy Color and a NES. 
I grew up with a bunch of other game systems that no longer exist in my hands — 
which is very unfortunate. Retro games cost so much now. Anyway, my discovery of 
computer science in high school plus me being a gamer is what put me towards the 
career path of game development originally. I went to UW-Whitewater and got a degree 
with an overly complicated name. It was Media Arts and Game Development with a technical 
emphasis — a mouthful. Then I ended up here, and I’m not disappointed. It’s a great place 
to work. I do wish I would find some motivation to do game development, because I have 
all of these ideas stuck in my head. I should make them come to fruition, but in the 
meantime I’ll just play some more video games.

**A video game that is on your list these days.**

The main video game I’ve been playing recently is Minecraft, which is a masterpiece in 
my opinion. There are a few of us on the team here that will occasionally talk about 
Minecraft. It’s a fun time, talking about the technical details. The other series I’ve 
been playing is the Borderlands series. I’m a very big fan, and I have invested a lot 
of time into it. A lot of time.

**Favorite things to do in Madison on the weekends.**

I come from the outskirts of Cross Plains, but whenever I come into Madison I enjoy going 
to the Terrace. I also like to just roam around the isthmus. I’ve recently gotten into 
going to concerts as well. Luckily we have a couple decent concert places around here, and 
they get some fun artists. One of the best things about Madison, though, is it’s a stone's 
throw away from a good hike. It’s not a very far drive. I’m also a big food advocate, 
and Madison has good food.

<figure class="figure float-end" style="margin-center: 1em">
  <img src='https://raw.githubusercontent.com/CHTC/Articles/main/images/cole_math.jpg' height="500" width="322" class="figure-img img-fluid rounded" alt="Cole wearing a NASA costume.">
</figure>

**Do you know any good programming puns?**

Really bashing my brain with this one. That was the pun by the way. The team loves it when 
I make bad puns. I have more. If you want to eat data, you can either do it bit by bit or 
in one big byte! This one is also good: there are 10 types of people in the world. Those who 
understand binary and those who don’t. I could keep going.

**What would you tell your younger self when you first started here at CHTC?**

That’s a difficult question because I am so young. One of my favorite pastimes is making my 
coworkers feel old, but don’t tell them I said that. Anyway, one piece of advice I’d give to my 
younger self would be that you will always keep learning. Whether that means learning to become a
better developer, figuring out new technologies to apply to the code-base, or even discovering weird 
obscure things. You never truly stop learning. I feel like pushing that towards my younger self would 
probably be good for him.

**Is there something you wish to add?**

I’m actually applying to UW-Madison’s professional masters program for computer science, which would 
be pretty cool to get into.