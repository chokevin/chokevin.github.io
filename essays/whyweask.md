---
layout: essay
type: essay
title: Why We Ask Questions the Smart Way
date: 2017-09-03
labels:
  - Problem Solving
  - Research
---

<img class="ui small right floated spaced image" src="../images/idea.jpg">

Programmers aren't walking encyclopedias. There will never be a time where we will understand everything about the system we are creating. Sometimes we can get extremely close to understanding a specific system. Some people dedicate so much of their life to understanding a subject that they write papers and books about a niche topic. No matter how much knowledge a person accrues, there will always be some unanswered question that lingers in their mind. For an engineer who is trying to figure out their financial situation, to a banker who is trying to make an automated Python script the amount of questions a person will come across is boundless.

While the amount of questions that a person may have could very well be unlimited, there's a good chance that 99% of those questions have been thought by another person in the world. There's about 6 billion people in the world with more than 1 billion people who can connect to the internet. With those odds there is a high possibility that a question on opening excel sheets in Python or mortgage rates for first time home owners has been asked in some form on a forum on the internet. So how can we go about collecting information about questions that haven't been answered before?

Now before we even begin to talk about questions that haven't been answered before, we should talk about questions that have been asked before. All answer hunting should begin with a good Google search. Thoroughly research the question to see if anyone else has encountered the problem. Especially when you are learning a new topic there is a high possibility that the question has been asked before. Sometimes the question needs to be reworded in different ways to see if a similar question has been asked in a different way. Anyway on to asking questions.

There is an article written by Eric Raymond that is titled How to Ask Questions The Smart Way. Theres some quote out there thats written <i> There are no such thing as dumb questions </i> except there are such dumb questions. They just are not phrased effectively. By having a ill-phrased question it will cause people to either misinterpret or ignore the question.

An example of a ineffective question is the following from StackOverflow.
<blockquote> Thread Title: Why method needs to call inside another method only? </blockquote>
<blockquote cite="https://stackoverflow.com/questions/46047798/why-method-needs-to-call-inside-another-method-only"> <i>
I have come across scenario where I am getting an error but unable to understand. Here is code: ( Assume I have created Grocerylist class with addgroceryitem method). I am new to Java so this question may sound stupid if it is basic logic but please to suggest for this. </i>
</blockquote>

This is an ineffective way to phrase a question because of three things. The first one being that the title of the question is vague and impossible to interpret by other programmers. Is this person talking about a specific case or is he talking about generally? At first glance it is impossible to tell. Another issue is that he draws attention to his inexperience and the potential stupidity of his question. According to Raymond, there is no need to call attention to lack of experience. The question should be asked in a clear, detailed manner in which a user conveys the exact problem they are having to another user.

This ineffective method of asking questions correlates directly to the quality of answers that are given. Most people on the thread respond with wide sweeping generalizations that don't specifically answer the question. One user wrote <i> This is the way java works, you cannot add non-declaration code (sorry i don't know the correct term) inside the class, that code should be inside methods. <i> While this answer may seem obvious to someone who already knows the answer to the above question, to the thread creator he may be more confused than when he wrote the question.

An example of a smart question is given below.

<blockquote> Thread Title: Does Java JIT cheat when running JDK code? </blockquote>

<blockquote cite="https://stackoverflow.com/questions/45912510/does-java-jit-cheat-when-running-jdk-code"> <i>
I was benchmarking some code, and I could not get it to run as fast as with java.math.BigInteger, even when using the exact same algorithm. So I copied java.math.BigInteger source into my own package and tried this:. When I run this (jdk 1.8.0_144-b01 on MacOS) it outputs: . When I run it with the import line uncommented:. It's almost three times as fast when using the JDK version of BigInteger versus my version, even if it's using the exact same code.
I've examined the bytecode with javap, and compared compiler output when running with options: and both versions seem to generate the same code. So is hotspot using some precomputed optimisations that I can't use in my code? I always understood that they don't. What explains this difference? </i>
</blockquote>

The code blocks were left out for conciseness, but this shows a quality question asked in the right forum. It was posted on StackOverflow which is the forum for programming questions. It also asks a question that has not been asked before. The answer is probably detailed in the JDK documentation; however, is not easily understandable or accessible to a programmer who is looking for a quick answer. The extent of the problem is documented thoroughly. The user shows an example of the problem and outlines exactly where the differences lie. This makes it simple for another user to answer his exact question which makes for a great learning experience for everyone. One mistake on this user's part is that he fails to check his question for spelling errors which deters users when reading.

The conciseness and the exactness of the answers that follow this smart question show the effectiveness of asking questions the smart way. It was also written only two hours after the question was posted.

<blockquote><i>
Yes, HotSpot JVM is kind of "cheating", because it has a special version of some BigInteger methods that you won't find in Java code. These methods are called JVM intrinsics.
</i></blockquote>
<i>
<blockquote><i>
In particular, BigInteger.multiplyToLen is instrinsic method in HotSpot. There is a special hand-coded assembly implementation in JVM source base, but only for x86-64 architecture.
</i></blockquote>
<blockquote><i>
You may disable this instrinsic with -XX:-UseMultiplyToLenIntrinsic option to force JVM to use pure Java implementation. In this case the performance will be similar to the performance of your copied code.
</i></blockquote>
<blockquote><i>
P.S. Here is a list of other HotSpot intrinsic methods.
</i></blockquote>

It provides an insightful answer to the posed question and is met with hundreds of approvals. The response points out why the user is seeing the following behavior in his question. All within a timely manner.

There is so much to learn in programming that hackers need to emphasize smart questions to get quick answers. If we continue to write smart questions, the quality of information on the web becomes richer, and programmers will be able to develop much quicker. The wealth of knowledge will keep growing every day.
