---
layout: essay
type: essay
title: "Answer Me This!"
# All dates must be YYYY-MM-DD format!
date: 2024-01-25
published: true
labels:
  - Smart Questions
  - Reliable Answers
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/questions.jpeg">

## Are There Smart Questions, or Just Foolish People?

Whether you’re in a room filled with 300+ students or in office hours with your professor, asking any question can be a daunting task. Asking questions may seem intuitively easy; however, it is a lot easier than it sounds. Everyone is afraid of looking or sounding stupid, but asking smart questions is a great way to avoid that. Asking smart questions is an important skill, not only for software engineers, but for everyone. Smart questions lead you to what you’re looking for more efficiently and is less confusing for everyone. For software engineers, they are usually in teams; and by asking smart questions, everyone is on the same page and everyone is able to help each other. Smart questions allow for productive conversations and allow for more proficiency. Smart questions also allow for smart replies/answers.

## “Sorry, what was the question?”
```
Q: How can I get the console to show in a fiddle on JSfiddle.com?

I recently saw a fiddle that had the console embedded in the fiddle, anyone know how this can be done?

A: pretty simple one..

example

github

Just add the following URL to External Resources in jsfiddle, you will see console.log and console.error in the result screen.

https://cdn.jsdelivr.net/gh/eu81273/jsfiddle-console/console.js
```
The question posted onto Stack Overflow titled “How to get console inside jsfiddle” has very sparse information. The two sentences asked were just a restatement of the title and how this person recently saw the console embedded into jsfiddle and wanted to replicate it. No picture or example of what they saw. In fact, a person in the reply had to get clarification of what this person meant. This is not really a smart question as multiple people had to ask for clarification, which was inefficient for everyone. The replies to the question weren’t any good either. The top answer was short but not concise, and did not show any example code, gif, or video, only links. This lazy question reflected poorly on everyone as it was a long process for something trivial. 

## Give A Round of Applause for the Smart Question! 

```
Q:  I have a JavaScript object like the following:

var p = {
    "p1": "value1",
    "p2": "value2",
    "p3": "value3"
};

How do I loop through all of p's elements (p1, p2, p3...) and get their keys and values?

A: ou can use the for-in loop as shown by others. However, you also have to make sure that the key you get is an actual property of an object, and doesn't come from the prototype.

Here is the snippet:

var p = {
    "p1": "value1",
    "p2": "value2",
    "p3": "value3"
};

for (var key in p) {
    if (p.hasOwnProperty(key)) {
        console.log(key + " -> " + p[key]);
    }
}

For-of with Object.keys() alternative:

var p = {
    0: "value1",
    "b": "value2",
    key: "value3"
};

for (var key of Object.keys(p)) {
    console.log(key + " -> " + p[key])
}


Notice the use of for-of instead of for-in, if not used it will return undefined on named properties, and Object.keys() ensures the use of only the object's own properties without the whole prototype-chain properties

Using the new Object.entries() method:

Note: This method is not supported natively by Internet Explorer. You may consider using a Polyfill for older browsers.

const p = {
    "p1": "value1",
    "p2": "value2",
    "p3": "value3"
};

for (const [key, value] of Object.entries(p)) {
  console.log(`${key}: ${value}`);
}
```

Another question posted onto Stack Overflow titled “How do I loop through or enumerate a Javascript object?” is already starting better off than the lazy question. The smart question had only ONE sentence, but it was concise and straightforward. They asked how to loop through an object’s elements and get their keys and values. They even provided example code in their question that wasn’t a link. Questions do not need to be lengthy to be smart but understandable. Smart questions are almost like emails in the sense that they are short but relay all of the important information to someone. The smart question also allowed for even smarter replies/answers. The top answer had embedded code examples about how to enumerate through a Javascript object and explained how and why. The top answer even gave multiple ways of solving the question each with explanations. Asking smart questions produces not only correct answers but also something that can be useful to someone years down the road. 

## So...Any Questions?
Asking smart questions creates efficient communication and is less of a hassle for everyone involved. Lazy questions do not elicit reliable answers and do not get anyone anywhere. Putting in a little more thought and taking the time to form smart questions is the best way to find what you are looking for. Smart questions also help others around you as they may also have the same or similar questions. It's more efficient and produces something of value, rather than everyone being lost and having no idea what is going on. 
