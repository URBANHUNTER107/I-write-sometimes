# I Joined a YC Startup and Spent My First Two Days Not Writing Code. Nobody Warned Me.

okay so i need to vent about something that's been sitting in my head for months.

when i got the internship offer — YC-backed startup, DevRel role, actually exciting work — i was pumped. like genuinely couldn't sleep the night before i started. i had ideas. things i wanted to build, communities i wanted to talk to, content i had already been drafting in my head.

day one. i open my laptop. and the first slack message i get is a setup doc.

forty-three steps long.

i'm not exaggerating. i counted. install this version of node, not the latest one, this specific one from three versions ago. configure these environment variables. make sure your GPU driver is *exactly* this version otherwise the pipeline silently breaks and you'll spend an afternoon wondering why your outputs look wrong.

i didn't write a single meaningful line of code for almost two days.

and the wildest part? nobody thought this was weird. it was just the thing. the thing you do when you join. the price of admission. one of the engineers even said to me "oh yeah two days is actually pretty fast, it took me a week when i joined."

a week.

---

## we've tricked ourselves into thinking this is normal

here's something i genuinely don't understand about our industry.

we will spend thousands of dollars on SaaS tools to save developers fifteen minutes a week. we will debate endlessly about tabs vs spaces and which testing framework is better and whether microservices are overengineered. but we will also just... casually accept that every single new developer — junior, senior, intern, contributor — has to sacrifice days of their life just to get to the starting line.

and it's not even the same starting line for everyone.

you want to learn Blender? cool, does your machine have a GPU? no? well you can try the CPU renderer, it'll just take forty minutes to render a frame, good luck staying motivated.

you want to run a machine learning model locally? sure, let's just check — does your CUDA version match PyTorch which matches your Python which matches the specific version of a dependency that one guy in Ohio last updated in 2021? no? welcome to dependency hell, population: everyone.

you want to contribute to open source? awesome. clone the repo. step one: it won't build. step two: google the error. step three: the Stack Overflow answer is from 2019 and half the commands don't exist anymore. step four: close the tab and never come back.

we talk a lot about "lowering barriers to entry." we do bootcamps and YouTube tutorials and free courses. but then we hand someone a laptop and a forty-three step setup doc and act surprised when they bounce.

the problem was never the concepts. it was always the configuration.

---

## the moment that broke my brain a little

so part of my job is going to college events — hackathons, tech fests, workshops — and showing developers what InfinityOS can do. it's a platform that runs GPU-heavy tools like Blender and Android Studio and DaVinci Resolve inside a browser. no install. no drivers. just a tab.

there was this one event in Pune. student walks up, i show him Blender running in a browser tab. and he just... stops. stares at the screen for like five full seconds. then quietly goes:

*"wait. this is actually running?"*

i've thought about that reaction a lot since then.

he wasn't impressed by a feature. he wasn't excited about some clever UI thing. he was surprised that the part he'd been conditioned to dread — the setup, the friction, the "okay let's see if this even works on your machine" moment — just didn't exist.

that's how deep the conditioning goes. when setup disappears, it feels like a trick.

i've had that same conversation maybe forty times now across Pune and Bangalore. always the same beat: the pause, the slight suspicion, the "okay but is it slow though?" (it's not, that's always the follow-up assumption). and then the slow realization that no, you can actually just... start.

every single time, what they're reacting to isn't the product. it's the absence of the thing they expected to suffer through.

---

## here's the part most people miss

the usual take on cloud dev environments is "it's more convenient" or "it's good for teams." and yeah, both true. but i think there's a more interesting argument that doesn't get made enough.

it's a trust problem.

think about how developer adoption actually works. someone hears about your tool. they get curious. they go to the docs. step one says install X. step two says configure Y. step three assumes you already have Z running somewhere.

each one of those steps is a place where you lose them. not because your product is bad — because the *road to your product* is full of speed bumps that have nothing to do with your product.

i think about this constantly from a DevRel angle. the whole job is closing the gap between "i heard about this thing" and "i'm actually getting value from this thing." every minute of setup is a minute where interest decays. the curious person becomes the frustrated person becomes the person who closes the tab and doesn't come back.

when an environment just works, you move the aha moment from day three to minute two. that's not a convenience improvement. that's a fundamentally different conversion rate. that's the difference between people who try your thing and people who stick around.

---

## the matrix thing (i promise this is going somewhere)

you know that scene where Neo learns kung fu by plugging in a chip and just waking up knowing it? "i know kung fu."

obviously that's not what's happening here. you can't download skill. a cloud environment doesn't make you a better developer.

but here's the thing i think people conflate when they push back on this stuff: nobody is saying make the learning easy. the argument is make the *starting* easy. those are completely different.

Neo still had to fight Morpheus. he still had to do the work. he just didn't spend three days beforehand trying to find a USB drive with the right OS image.

removing setup friction doesn't make you soft. it just means the difficulty you face is the actual problem you're trying to solve, not the arbitrary tax you pay before you're allowed to touch it.

nobody becomes a worse engineer because they didn't have to compile their own kernel. i promise.

---

## okay but is this real or is it just docker 2.0

fair. i'm asking myself this too.

because we have been here before. Docker was going to fix environment problems forever — and it did help, while also inventing about twenty new ways for things to silently break. Vagrant was going to be the answer. there's a whole graveyard of tools that promised to end setup hell and instead just moved it somewhere slightly harder to find.

so yeah, cloud dev environments could go the same way. the concerns are real: latency matters for certain workloads, vendor lock-in is a genuine risk, "what if your internet is bad" is a real question for a lot of developers outside SF, and the cost model at scale is still being figured out.

i get all of that.

but here's what feels different this time. every previous solution asked developers to manage their environment more skillfully. cloud environments are asking a different question entirely: what if you didn't manage it at all? what if it just existed, ready, the moment you needed it?

that's not an incremental improvement. that's a different premise. and i think it's the right one.

---

## the thing that actually gets me though

i'm from Varanasi. not a tech hub. not the kind of city that gets featured in startup news. just a city with a lot of students who are genuinely curious and genuinely capable and working on mid-range laptops with 8GB of RAM and no GPU.

i know what it feels like to hit the hardware wall. to want to learn something, try to set it up, and get told by your own machine that you're not allowed.

and i know what that does to someone who's just starting out. you don't think "oh this tool has high system requirements." you think "maybe i'm just not ready for this yet." you think the problem is you.

it's not.

the problem is that most developer tooling was designed by and for people who have good machines in good environments with fast internet. everyone else is just working around assumptions that were never meant for them.

when i think about what cloud dev environments could actually mean — not in a pitch deck way, in a real way — it's this. the student in Varanasi and the student at IIT and the engineer in San Francisco should all hit the same starting line. the barrier should be the problem, not the machine.

whether that actually happens depends on pricing, accessibility, whether these companies stay independent or get acquired and go enterprise-only. i don't know how it plays out. but the direction is correct.

---

## so where does this leave us

i think we're in that weird early phase where the technology is real but the habits haven't caught up yet.

most developers still default to local setup. not because it's better — it usually isn't — but because it's familiar. there's a specific kind of comfort in having your environment on your own disk even if that comfort costs you two days every time you start something new. breaking that habit is a culture problem, not a product problem. and culture moves slow.

but what i've noticed is this: once someone actually experiences an environment that just works — no error messages, no version conflicts, no "did you try reinstalling?" — they don't really want to go back. the muscle memory shifts.

the hard part isn't building the product. it's getting people to the moment where they actually feel it.

which is, now that i think about it, exactly what Developer Relations exists to do.

so i guess i'm working on the right thing.

---

*Mohd Farhan Abbas — second year CSE at DY Patil International University. DevRel intern at ProjectX (YC P26), working on InfinityOS. i also do data analysis and SQL stuff and occasionally contribute to open source.*

*[GitHub](https://github.com/) · [LinkedIn](https://linkedin.com/) · [Twitter/X](https://x.com/)*
