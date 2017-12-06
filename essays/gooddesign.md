---
layout: essay
type: essay
title: Good Design
date: 2017-12-05
labels:
  - Design Patterns
---

When working at my internship this past summer, my manager had imparted on me one software engineering idiom that has kept with me. He had just moved over to Amazon one week after I started my internship. The manager that held the responsibility of getting me through my 12-week internship at different company working on a technology stack completely different to his expertise had just started a week before I did. That's five business days. Doesn't instill much confidence in a person. At least I didn't feel confident about him.

Yet this guy was quite the software engineer. He had spent a majority of his career across the street at Microsoft working on kernel development for the Window's OS. His last coding stint was working with some of Microsoft's smartest guys contributing code to a codebase that reaches millions of people. During his time as a manager he also helped mentor interns into successful projects.

He was a smart guy and a more than qualified software engineer in low level software, but here we are in a project involving social media. Amazon Spark was the next new social media platform for the e-commerce giant and I had been given a project in Java and React. My manager wrote all his code in C++ in his past job. A lot of his experience just doesn't add up to what we had to do. I was a little nervous since this internship would base whether I would get a return offer for the next summer.

When we had our first one-on-one it was like he could tell that I was lacking a little confidence in myself and in him. We were talking about my time at Amazon where he took a step back and talked a little more broadly. He mentioned design patterns. At the time I had no idea what a design pattern was. I had just picked up the book Clean Code where I started to learn the basics of writing clean code, but I had never heard terms such as observer, singleton, or factory before.

What he told me that has stuck with me is that the language or project scope really doesn't matter. To him the only thing that matters is whether you can see the proper design patterns reflected in the codebase. the My nervousness quickly went away after we had our first one-on-one. I began looking up design patterns and was quickly caught up on these design patterns which are simple to understand but make code much more structured and readable.

One example of a design pattern that is used heavily in client-based models in the Singleton. When accessing something such as an API client from the backend we would only require one continuous connection with the API server. However, without the singleton model, there is a possibility that each parallel client that accesses our backend would create a new connection to the server. This is unnecessary so we limit the connection to a Singleton where the client declaration only happens once. This helps reduce the amount of connections that are created when scaling upwards and improves the readability of the code.

In industry, I had experienced design patterns frequently when reading code in large codebases. Interfaces, factories, you name it. All of them are important in understanding how a new codebase works when you are tasked with writing or maintaining code you have never seen before. However, with mastery of design patterns anyone is able to quickly understand and work to improve the code.
