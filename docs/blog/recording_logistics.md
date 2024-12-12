---
layout: blog_page
title: Why it's hard to get classes recorded
permalink: /blog/recording-logistics/
---

date: 2024-12-12 \\
last edited: 2024-12-12 \\
author: ashay athalye

---

## Intro

Putting hundreds of classes online requires getting hundreds of classes recorded. I used to think that this should be fairly easy, but it's turned out to be non-trivial. Looking back, this was to be expected: logistics is hard.

[MIT OpenCourseWare](https://ocw.mit.edu/)'s standard method to record a class would be to hire [MIT Video Productions](https://mvp.mit.edu/) (MVP) to record the class.[^1] MVP's rate is something like $10,000-$20,000 per course (a standard full-semester lecture-based course at MIT may have ~24 1.5-hour lectures, or ~36 1-hour lectures). If we want to scale, we need a different strategy to record classes.

## A minimal setup

Consider this minimal setup:
- put someone's smartphone on a stand (plenty of cheap phone stands you can buy on Amazon) somewhere in the classroom, pointed at the instructor
- start a recording on the phone at the beginning of class, and stop it at the end of class
- have the instructor start a zoom recording on their laptop at the start of class

In doing so:
- audio is recorded through the phone's mic and the laptop's mic
- the classroom projector screen, if used, is captured on the phone video and also through zoom via the laptop screen share
- the chalkboard/instructor is captured on the phone video

With this setup, neither the audio nor video is great, but they are sufficient to edit together a recording of the class that's tolerable. Rather than have nothing, if I really wanted to learn something and couldn't learn it anywhere else, I'd be happy to watch the video that results from this setup. In fact, smartphone cameras are so good these days, the recording would probably be much better than tolerable. If we were to use a good microphone, the recording would be good, even.

When I talk to people about how to get classes recorded, many people propose this kind of minimal setup. "It's so easy to do this, everyone has a smartphone these days, just put it on a stand and record." 

## Why it’s hard to get classes recorded

<b>There are two reasons it isn't actually so easy</b>:

`(1) It's just more complicated than you think to get something supposedly simple to work reliably across a distribution of scenarios.`

`(2) You need someone to perform the setup, and the people we have available in the classroom can't be trusted to do it properly.`

Expanding on 1:
- Placing the phone such that everything we'd like to be in view, is in view, takes some care. Ever given a stranger your phone to take a picture of you? Most of the time the picture turns out bad.[^2]
- If the ideal phone position isn't in the first row of seats, how do you make sure students don't sit in front of the phone?
- What if a student knocks the phone over?
- How do you make sure the phone is sufficiently charged to stay on the whole time?
- How do you make sure the phone camera refocuses properly if it ever gets out of focus? It might change focus when students walk across the classroom.
- How do you make sure the phone camera exposes properly if it every changes its exposure? It might change exposure when the projector screen toggles on/off.
- Who in the classroom will volunteer their phone?
- Does their phone have enough storage space for the recording? If the recording is done at max resolution, it'll be big: a 1080p video at 30fps for 1.5 hours is ~11.7GB.
- How do you get the recording off their phone? Do you ask them to submit it somewhere?
- ...

Expanding on 2:

We can’t be in every classroom, so we rely on one or more of the instructors, TAs, and/or students to do the setup. However, their focus is elsewhere. Their primary motivation to be in the classroom is, rightly, not to do a setup task. Even if we pay them, keep the setup short, and provide clear instructions (and a walkthrough the first few times), finding and training someone to do the setup properly is challenging. 

More generally, there are three reasons why it's hard to get classes recorded: \\
`(1) Things are more complicated than you think.` \\
`(2) People are unreliable.` \\
`(3) Technology is unreliable.`

<b>Put more positively, we have to handle tricky logistics, minimize setup, provide clear instructions, motivate people, and improve basic infrastructure to get things to work reliably.</b>

I'll end with a concrete example of difficulties we faced in recording a particular class this fall semester that illustrates each of (1), (2), and (3).

## A concrete example
A course we wanted to record lectures for this fall was in one of [IS&T's autocapture rooms](https://ist.mit.edu/lecture-capture). Knowing that their provided microphone can often have problems (and it's so unfortunate when we lose audio for a lecture, because it's a lot to ask the instructor to give the lecture again), I decided on the following strategy to reliably record the lectures:

- Record via IS&T's autocapture system (video of classroom + audio)
- Record via zoom on the instructor's laptop (backup audio, backup capture of projector screen via laptop screen share)
- Record via portable audio recorder (Sony ICD-PX470) (backup audio)

[Here](https://docs.google.com/document/d/16vF_MX7bxhcjGaXRgk-oBxtmUeE5uw-GhoREdBth_EA/edit?usp=sharing) are the steps I provided the instructors and taped onto the table the instructor would put their laptop on. The steps take 30 seconds at the start of class (joining a zoom meeting, starting the audio recorder, putting on the lapel mic), and 30 seconds at the end of class (ending a zoom meeting, stopping the audio recorder, taking off the lapel mic). I went to class the first few times to help walk them through the steps.

Despite instructions that were easy to follow, reminders about what to do, and a very patient and cooperative teaching staff:
- In 15 out of 23 lectures, audio was missing in the IS&T recording (cause unknown)
- In 2 out of 23 lectures, the portable audio recorder wasn't started
- In 23 out of 23 lectures, the zoom microphone was not umuted

We ended the semester with 2 lectures that did not have audio from any of our three audio sources. Unfortunately, we won't be able to rerecord those lectures until next fall. 

Should I consider even more sources of backup audio next time?[^3]

## Conclusion

Recording classes should be very easy, but it can be hard to achieve at scale. 

Teaching staff already have a lot to worry about. Is it reasonable to expect them to be able to help with recording setup? Next time, should I also recruit some students in the class to help? My experience hiring students to do lecture scribing work tells me otherwise -- they can also be unreliable. 

My main takeaway from trying to get classes recorded the past few years is that if you want to get something done reliably, you need someone on the ground who's main responsibility it is to get that thing done. Maybe we can't avoid hiring people specifically to handle recording logistics. But that seems like such a waste of resources when the recording setup, especially in autocapture rooms, requires following just a handful of steps. 

MIT instructors often handle extensive setup tasks on their own, especially for lab classes. While open education is already more present in MIT’s culture and values compared to other universities, it is still limited in scope. By making it an even more central part of the culture, we could make recording setup a key responsibility of teaching staff, allowing us to cost-effectively scale to recording hundreds of classes.

## Footnotes:

[^1]: In recent years, many classes have been recorded on zoom or in rooms that have some level of automatic recording technology, so the majority of OCW's course publications this past year may not feature recordings done by MVP. 
[^2]: E.g. it's not framed well, your feet are half cut off rather than fully included or excluded, etc.
[^3]: Joking, but not entirely...
