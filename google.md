# Everything I know about getting a job at Google

Amanda House ([amhouse.github.io](https://amhouse.github.io))

2020 November 15

---

## Why

Before the pandemic, when it was possible to do so, I very occasionally socialized. Maybe a few times a year. At every party, regardless how far I went from the Bay Area, I met aspiring software engineers. These people ranged from current computer science students, to people making a later in life career change, to, memorably, a 10 year old. I've handed out enough cards and entered my contact info into enough phones to get messages from people I had met once, their friends, their friends' friends, ... Even now, I get a steady stream of emails asking for advice.

I'm not writing this because I'm somehow more of an expert than any other Google engineer is, but because I've written versions of this over and over again. And one of my favorite ways to answer questions at work is to send back a link to documentation that I wrote. (I absolutely love writing documentation.) So, next time I get an email asking for advice, I'll have this.

## Roadmap

We'll go through what you could do to get a job at Google, in roughly reverse chronological order. Obviously you would need to follow the steps in forward chronological order, but people seem to have more concrete questions about the immediate steps than all the work that leads up to it, so I've found that people follow better when I reverse the order.

## Getting the interview

The best way to make sure you get an interview is to first get your foot in the door somehow. I have absolutely no idea how applications and resumes get filtered. (I'm not saying that because I'm not allowed to, I am just severely allergic to "process" and anything that isn't doing my job well, so I really just don't know.) But I have heard many, many stories about great applicants getting auto-rejections. I do not know the rhyme or reason to them, but I do know that you can greatly increase your chances of getting that first call through a few avenues:

Referrals. The world runs on connections. Getting a referral from someone who does the job that you want to do is a great way to stand out in a pile of applications. I have no stats nor educated guess on what the exact difference is for follow-ups with or without a referral, but I wouldn't be surprised if it's orders of magnitude better with.

College career fairs. Many people I've worked with love hiring interns and new grads. They can be full of passion and extremely moldable. You'll see big tech companies recruit heavily at strong CS programs, and not just the Ivies/MIT/Stanford—last I checked, pushes for diversity have taken college recruiting all through the Midwest. This is another good way to get that first interview; you get a chance to not only submit your resume, but have a face to face chat with a recruiter or SWE. If they like you and your application, it's also likely that you can get a same day (or same couple of days) interview. NOTE: I have no idea how this has adapted during the Covid era. If you're a current student, you could check with your program if any virtual recruiting is happening.

Coding challenges. I have no direct experience with this one, but I have encountered people who searched some CS/SWE things on Google and unlocked an Easter egg coding challenge that actually turned into a full slate of interviews and an offer. So if you've put in the work to prepare well, and you get lucky with timing, this may be a way to get that first call back.

## Preparing for interviews

Interviews are not perfect. I am not here to advocate for or against them. From what I've seen, what exactly interviews measure for, their biases, and their effectiveness, are topics of intense debate online. You can easily find these arguments elsewhere. So for the purposes of this guide, I am going to completely sidestep that discussion and simply present what I did to prepare for interviews.

Reading the infamous Cracking the Coding Interview is an absolute must. This book tells you everything you need to know about the mechanics of interviews. I'm not even going to try to summarize the key points of the book, because at this point I suspect I've forgotten more of it than I remember. So just read it; it's assumed background for the rest of this write-up.

Instead of trying to rehash CtCI, what I can do is provide my particular flavor of interview prep. In general, I think of interview prep in 3 dimensions:

- Data structures and algorithms. Strong fundamentals here will be key to figuring out the solution of each problem.

- Implementation. Fluency in your chosen programming language will smooth over the entire interview experience. You don't have to be able to write perfect code with no errors outside of an IDE, but you shouldn't struggle with the basics either.

- "All the other stuff" that goes into an interview. It's not enough to figure out the solution and code it flawlessly; interviewers are looking for your thought process and communication skills. There's a checklist of things to cover.

Now, the details:

For "all the other stuff": Interviewers want you to talk out loud so they know where you're at and what you're thinking. So when you first get the problem, do your brainstorming out loud. Talk out a solution, and when you think you've got it, do a sweep for edge cases. Ask your interviewer about assumptions you want to make, or if there's enough ambiguity, ask them how you should handle those cases. When you've got a full grasp of the possible inputs and solutions, start implementing. Don't talk about your code in so much detail that you're explaining, say, what a for loop is, but do explain each chunk of code grouped together as a logical step. When you think you're done, do not announce that you're finished! Tell your interviewer that you're now going to run through your code to check for any bugs—and do that. It's so much better to find a flaw yourself, than it is for your interviewer to have to tell you there's a bug in some part of your code. Then offer a complexity analysis of your solution. Expect all interviewers to care about time complexity, and be prepared for any interviewer to follow up with a question about the space complexity. Only then should you say that you're done—and, if your solution is worse than O(n), you should offer to now optimize it, unless the interviewer has a follow up part in mind.

On data structures and algorithms: Everyone and their mother has a list of topics to study for interview prep. I'll provide my list for the sake of this guide being "complete," but just be aware that this is by no means comprehensive nor authoritative. It's just what I covered before interviews to feel prepared enough.

- Arrays
- Strings
- Sets, maps, and hashing functions
- Linked lists
- Queues, BFS
- Stacks, DFS
- Trees
    - Binary
    - Traversal orders
    - Binary search
    - Etc. There are so many trees. Study as many as you can until you feel sick when you think about trees.
- Recursion
    - Memoization
    - DP
- Searches
    - Particularly binary
- Sorts
    - Particularly merge and quick
- Heaps
- Concurrency
    - Threads (vs processes)
    - Semaphores (vs mutexes)
- Graphs
    - Shortest path algorithms. Pick your favorite to know how to implement (e.g., Dijkstra's)
    - Topological sorting
    - MSTs, if you're not already sick of graphs by this point
- Big O for all of the above

For all of the topics above, I review:

- The concept of the data structure or algorithm (Wikipedia, university lecture notes posted online, or any other reasonable resource)
- How to implement the ds/alg yourself
- Then, whether your preferred language has a library for that ds/alg
- For data structures, how to use them / the operations of them
- The applications of the ds/alg in the context of interview problems. So, examples of problems and solutions using that ds/alg.

On implementation: You should pick a programming language to use for your interviews that strikes the right balance of your expertise in it, and how appropriate it is for interviews. E.g., I used Java constantly through college and almost exclusively at work, but I had also become familiar with Python at the end of college and now use it in my spare time / for personal side projects. So I chose to use Python, because the thought of fighting with Java's verbosity during a high pressure situation seemed terrible.

As I mentioned above, no one expects you to be able to code flawlessly on a whiteboard or on a laptop but without an IDE. The point of practicing using your chosen language isn't to make zero mistakes during the interview, but to be fluent enough that you're not tripping yourself up after you've done the hard part of identifying a solution.

My approach to rapidly increasing my Python fluency was to: Choose a variety of practice problems (roughly in order of the list above). Then when I did, say, a stack problem, I kept notes in a text file on how to initialize, push, and pop with the stack. I would do the same for various for loop syntaxes when I used a new one while practicing, or to keep track of how to iterate through key, value pairs of a map, and so on. Basically, if you had to look it up to use it, make a note of it. Then use spaced repetition to memorize the contents of your text file, and enjoy flying through the implementation part of your interview.

One last note: Practice, practice, practice. I've sort of talked about it all throughout this section without explicitly addressing it. You could use CtCI; it's an enormous book full of problems. I do recommend something like LeetCode or HackerRank instead, though. The main advantage is that, when you test your solution, you don't have to be the one to think of dozens of test cases nor manage the infra to define and run your code against those tests.

## Computer science fundamentals

If the "preparing for interviews" section seems daunting, all I can say is that getting a solid computer science education is the single best thing you can do to prepare.

You'll never truly master something the first time you learn it. The process goes something like: become aware the concept exists, get the basics down, and practice it a bit. Time goes on, you forget much of it. But then you are reminded of it, regain some of that initial knowledge, make a few more connections and insights than you had the last time, and practice it more. And so on. Each time you encounter that concept, you'll master a bit more and it'll get a bit easier.

A great CS education will do this to you over 4 years. Then you'll leave, you'll think you've forgotten it all, and then you'll sit down to prepare for interviews and go, "Oh, I remember this. This isn't so bad."

I cannot emphasize this enough. My CS degree seemed unnecessarily grueling at the time, and even while I was there, I thought I forgot everything from the last semester by the time the new one rolled around. But then, my experience with interviews went something like this:

<img src="https://amhouse.github.io/blog/media/interviews.png" width="300"/>

NOTE: I cannot speak to whether bootcamps are sufficient, as I have no direct experience with them nor people who graduated from them. I will say that my opinion from hearing about them is that they will do very little to help with the topics above. I do, however, acknowledge that a 4 year degree in CS is infeasible for many people, and I would never be opposed to alternative methods of learning. My viewpoint simply comes from my experience and one way to get a strong foundation in CS.

Good luck!

---

### Contact

[amhouse.notify@gmail.com](mailto:amhouse.notify@gmail.com?subject=Google)

Comments welcome!

### Blog home

[https://amhouse.github.io/blog](https://amhouse.github.io/blog)

Please do share this blog with anyone who might find it interesting.
