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

## Is there such thing as a stupid question?

I’ve had instructors address a whole class and say, “There’s no such thing as a stupid question.” I now know that is in fact not true because I’ve challenged the statement and received the appropriate dumb-stricken, annoyed look. There are definitely stupid questions, and along with that, usually unhelpful answers. Though we all might be guilty of being callous and making people victim to our poorly formed questions, there are steps we can take to ask smarter questions that hopefully don’t illicit the dreaded “rtfm” or “stfw” response.

## What’s a smart question?

Stack Overflow, a question and answer site for programmers, is a great resource for anyone who may have issues with code or who may simply want to learn new or different methods of doing something. There I found examples of good questions and bad questions, which could probably be improved.

In the following example, we examine the components of a decent question. In this case, the asker is trying to figure out a way to get the date of the previous month in Python.

```
Q: python date of the previous month

I am trying to get the date of the previous month with python. Here is what i've tried:

str( time.strftime('%Y') ) + str( int(time.strftime('%m'))-1 )

However, this way is bad for 2 reasons: First it returns 20122 for the February of 2012 (instead of 201202) 
and secondly it will return 0 instead of 12 on January.

I have solved this trouble in bash with:

echo $(date -d"3 month ago" "+%G%m%d")

I think that if bash has a built-in way for this purpose, then python, much more equipped, should provide something 
better than forcing writing one's own script to achieve this goal. Of course i could do something like:

if int(time.strftime('%m')) == 1:
    return '12'
else:
    if int(time.strftime('%m')) < 10:
        return '0'+str(time.strftime('%m')-1)
    else:
        return str(time.strftime('%m') -1)
        
I have not tested this code and i don't want to use it anyway (unless I can't find any other way:/)

Thanks for your help!
```

While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## The foolproof way to get ignored.

While there are decent questions that benefit everyone, there are those one can ask to create an entirely different effect. In the following example, a user asks how he would, in short, create a desktop application with Facebook.

```
Q: Facebook Desktop Notifier

I am a beginner programmer that have never used anything other than what's included in a language.

I am trying to create a desktop application that notifies me anytime I get an update onfacebook. 
How should go about doing this? Thanks in advance.

edit Sorry I was not clear. Is there any way to make a DESKTOP application with facebook?
```

A simple “yes” would have answered the question, but we know that’s not the sort of answer he or she is looking for. Fortunately, someone kindly responded with a link to Facebook’s developer website. The asker should have done more research on his or her potential project. Then further down the road, he or she could have asked more specific and detailed questions that wouldn’t require a thousand-paged response for a sufficient answer.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.

## Are There Smart Questions, or Just Foolish People?

Whether you’re in a room filled with 300+ students or in office hours with your professor, asking any question can be a daunting task. Asking questions may seem intuitively easy; however, it is a lot easier than it sounds. Everyone is afraid of looking or sounding stupid, but asking smart questions is a great way to avoid that. Asking smart questions is an important skill, not only for software engineers, but for everyone. Smart questions lead you to what you’re looking for more efficiently and is less confusing for everyone. For software engineers, they are usually in teams; and by asking smart questions, everyone is on the same page and everyone is able to help each other. Smart questions allow for productive conversations and allow for more proficiency. Smart questions also allow for smart replies/answers.

## “Sorry, what was the question?”

The question posted onto Stack Overflow titled “How to get console inside jsfiddle” has very sparse information. The two sentences asked were just a restatement of the title and how this person recently saw the console embedded into jsfiddle and wanted to replicate it. No picture or example of what they saw. In fact, a person in the reply had to get clarification of what this person meant. This is not really a smart question as multiple people had to ask for clarification, which was inefficient for everyone. The replies to the question weren’t any good either. The top answer was short but not concise, and did not show any example code, gif, or video, only links. This lazy question reflected poorly on everyone as it was a long process for something trivial. 

## Give A Round of Applause for the Smart Question! 

Another question posted onto Stack Overflow titled “How do I loop through or enumerate a Javascript object?” is already starting better off than the lazy question. The smart question had only ONE sentence, but it was concise and straightforward. They asked how to loop through an object’s elements and get their keys and values. They even provided example code in their question that wasn’t a link. Questions do not need to be lengthy to be smart but understandable. Smart questions are almost like emails in the sense that they are short but relay all of the important information to someone. The smart question also allowed for even smarter replies/answers. The top answer had embedded code examples about how to enumerate through a Javascript object and explained how and why. The top answer even gave multiple ways of solving the question each with explanations. Asking smart questions produces not only correct answers but also something that can be useful to someone years down the road. 

## So...Any Questions?
Asking smart questions creates efficient communication and is less of a hassle for everyone involved. Lazy questions do not elicit reliable answers and do not get anyone anywhere. Putting in a little more thought and taking the time to form smart questions is the best way to find what you are looking for. Smart questions also help others around you as they may also have the same or similar questions. It's more efficient and produces something of value, rather than everyone being lost and having no idea what is going on. 
