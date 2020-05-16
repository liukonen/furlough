# Day 26

Monday Monday.


I had plans. Plans to learn the go language today... but that will have to wait, as I need to help my dad out with something.
It's ok though... why, because I spent the entire weekend programming rather than relaxing. Lame, right! However, I ran into some problems. 
From Last Friday, you'll know I converted my chatbot over to C#. Specifically the C# .Net Standard runtime. Worked fine on my mac. Runs fine on my one windows folding at home box (minus a hiccup I saw today)
What it doesn't do, is want to compile or run on my Linux machine using mono. Ok, Fine, I will make it a .net core application. That way I don't need the mono framework.
So my Saturday consists of converting my app to .net core, doing some test runs, setting up a new "beta" app for testing on a different slack workspace. Runs great on my mac. Runs great on Windows. Test it out on Linux, reports back fine and evens shows active. But when I ask it a question, I get the silent treatment. Gah! Sunday rolls around. I do some things, then get back to it. Ok... well I know it runs well on windows... if its compile or permissions, maybe a docker container will fix it. So I take my app, make a "quick" (still took me a while since I am learning) docker container, run it..... and.... still ignoring me.

My plan B for the app... run it on my windows box for now (which is also folding) until either I figure out how to get it running, OR the second option, I go back to Python, only not dependent on the RiveScript format. I found an Aiml library I can use, which should in theory run faster then RiveScript. I know my Bot runs great on python, and if I have connection issues they get thrown. the .net implementation I found is not telling me anything as far as errors go, or if my connection is junk.

So because of that, I'm probably going to start working on plan B, and later, when participating in DockerCon, maybe I know more and can fix the issues I'm running into with the container I made.

Also, today is a good day to keep it light, since tomorrow is [Dev around the sun](https://devaroundthesun.org/) 