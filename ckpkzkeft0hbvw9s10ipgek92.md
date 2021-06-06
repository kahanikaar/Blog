## Getting into GSoC'21 with CERN-HSF

With a lot of excitement, I hereby share that my proposal, ROOT Storage of Deep Learning models in TMVA, with CERN-HSF was accepted for Google Summer of Code 2021 and thus I will be working under the guidance of my mentors   [Lorenzo Moneta](https://www.linkedin.com/in/lorenzo-moneta-982b902/) (Senior Physicist at CERN) ,  [Anirudh Dagar](https://www.linkedin.com/in/anirudhdagar/) (Previous GSoC student developer at CERN), and  [Sitong An](https://www.linkedin.com/in/sitong-an-71533a94/) (Marie Curie Fellow at CERN)  from the TMVA team of the Root Project. 

![Screenshot from 2021-06-06 06-11-28.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1622940163443/B0hu_19Ap.png)

CERN-HSF (High Energy Physics Software Foundation) is an Umbrella organization for high-energy physics-related projects in GSoC. CERN (*Conseil Européen pour la Recherche Nucléaire*) is the European Organization for Nuclear Research that operates the largest particle physics laboratory and is known for the Large Hadron Collider, while the HEP Software Foundation facilitates cooperation and common efforts in High Energy Physics software and computing internationally.

The Root Framework is an open-source object-oriented library for data analysis developed by CERN, primarily written in C++, with bindings for Python and R, having functionalities of processing, analysis, visualizations and storage. TMVA (Toolkit for Multivariate Analysis), a submodule of ROOT,  provides a machine learning environment for the processing and evaluation of multivariate classification and regression techniques. My project involves developing the functionalities facilitating the storage of deep learning models which are trained in TMVA and converters for translating saved models trained in other frameworks like PyTorch and Keras, into the ROOT format following the ONNX standards for fast inference.

This is the first blog in the GSoC with CERN-HSF series documenting my work and experience over the period. Here I present my experience of the selection procedure I underwent for getting in.

### Table of Contents
- [Motivation](#motivation) 
- [Prequel](#prequel)
- [Adapting to learn](#adapting-to-learn)
- [Time of the year](#time-of-the-year)
- [Day to Results!](#day-to-results)



## Motivation 
Google Summer of Code is an initiative by Google for university students to participate in a 3-month long program towards contribution to open-source, where each student is paired with respective mentors working on a project under an open-source organization.

I was always a fan of Open-source and the idea behind developing software for the free use of everyone while providing the source code for collaborative development  fascinated me the most. It was back when I entered in college in my freshmen year,  I got to know more about "Open-Source Development" and "GSoC" and the mere curiosity to explore these,  actually took the first step towards this journey. The very active Programming Society of my college, working on various domains, having people of unique insights and interests lead by my seniors, introduced us to concepts of Git, how we can collaborate on developing open source software and of-course about popular programs like Google Summer of Code. I was amazed by the dynamism, involvement and dedication of my seniors while working on the renowned repositories of JuliaLang, OWASP, coala, etc. and thus got intrigued to contribute to this fascinating thing.  Eventually, I started contributing to open-source since my sophomore year and it has been a great experience since then, learning a lot by contributing to the spirit of free and open source software.

## Prequel
Before starting the story, let's have a trip to the past, shall we?

<p align="center">
<img align="center" src="https://media.giphy.com/media/BpGWitbFZflfSUYuZ9/giphy.gif" alt="drawing" width="500%" style="display: block; margin: 0 auto;" />
</p>
It was at the end of my sophomore year, in 2020, when I applied for GSoC for the first time. Owing to some unfortunate factors, firstly I started off late for the process which was the major setback. Eventually, I messed up discovering the organizations I should've applied based on my skills and domains I pursue. I lacked the aptitude to understand a large codebase properly and didn't research much for the projects, I shortlisted.

Somehow, I finalized to apply for two organizations and submitted the proposal. Finally,  it was the D-Day, 4th of May, 2020, when the results came, 

![Screenshot from 2021-06-06 14-42-46.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1622970821050/j7G_tEHOl.png)
it was unfortunately NOT MY DAY, the results were disappointing as my proposal got rejected in both the organizations I applied for.

It was something very upsetting, but soon I got back to work and decided to contact the mentors regarding the results. On the 6th of May, 2020, I wrote to the mentors for their feedback on my proposal and where is the scope of improvement, and I was lucky enough to receive a reply on the same.
 
- >![Screenshot from 2021-05-24 18-34-11.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1621861501042/s6XatAMYp.png)

- > 
![Screenshot from 2021-06-06 14-45-55.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1622971012553/yw0KFhDiq.png)

I geared up to analyze the feedback, focusing on where I lacked, how I could have been better and where improvement was seriously needed in my work. 

## Adapting to learn
Soon after the results, I sat down listing where can I improve myself and have a steady development on my learning. Due to the COVID-19 pandemic, all our college activities were suspended, thus we got a good amount of time to focus on developing technical skills, and exploring new domains. I started learning new languages and frameworks, developing projects and went through some cool courses, I always had that intriguing interest of developing ideas to real life problems and enjoyed participating in hackathons. Me along with few of my friends formed a group, named it Deluminators (*Potterheads ;)* and we participated in a lot of hackathons over the period. Hackathons were one of such events which actually inculcates the sheer skills of creative and critical thinking, collaborating on a team to develop something, and the spirit of always learning something in the process. I started exploring more about open-source (development, contributions and events), researching and exploring the fields which interests me. Having a systematic plan while aiming for a goal, and keeping a consistent approach towards my work, I was evolving. Artificial Intelligence in general and Machine Learning in particular are the fields which excites me the most, and I love learning and diving deep into the working of algorithms related to machine learning, and trying to comprehend what those black-box concepts actually mean and work in the background. Accepting one's own mistakes, further analyzing it and working towards correcting them are one of the bravest act anyone can do. While applying to GSoC in both 2020 and 2021, I did commit a lot of mistakes but did learn from them, which accounts for another detailed blog, sometime later perhaps.

## Time of the year
It was the month of February again! The wave of GSoC had already gained momentum. Frequent contributions to the popular organizations and repositories were seen, and even I was working on giving my best shot this year.
I started shortlisting the organizations where I should apply depending upon my skills and interests, maintaining daily logs and notes of work. After finalizing to apply for CERN-HSF this year, I started communicating with the mentors of various sub-orgs under the organization and explored more about the projects they planned to undertake this summer. The process of applying to CERN-HSF included performing a preliminary task for individual projects, and based on the submission, the mentors evaluated us and some selected people were called for further discussion about the project and for drawing up the proposal. 
After submitting the preliminary tasks for the project, I contacted the mentors to know more about the project and their views for the same, and further drafted an initial proposal and sent them for their review. After going through the proposal, they gave a positive feedback, and even asked me for some changes which may improve my plan and chances of selection. After careful work on the suggestions and review, I finalized the proposal which was then submitted on the 13th of April, 2021.

## Day to Results!
The tension inside was rapidly increasing as the day of result was fast approaching. I was uncertain whether I will be selected this time, considering how GSoC has became highly competitive and there can be another candidate with a better proposal or project which may lead to my rejection again. It was the 17th of May, 2021, when the results were scheduled to release, and I was super nervous the whole day. I wasn't even able to study for my semester exam scheduled on the following day. I remembered it was around 11.20PM, in the last year, when the results were declared, so I thought this time  they might be releasing it on a similar time as well. Nevertheless, I was repeatedly checking my mailbox for any updates regarding the same. 
At around 11:14PM, when I reloaded my mailbox, suddenly I saw the notification of an email, whose subject stated, **"GSoC 2021: Congratulations, your proposal with CERN-HSF has been accepted!"**, and I was overwhelmed with happiness. I literally cried reading through the content of the email.


![Screenshot from 2021-06-06 14-47-29.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1622971102679/a-MVtGVud.png)

Getting into GSoC was one of the dream goals I aimed for during my span of being a University student, and this was beyond expectations for getting an opportunity to work in one of the most exciting organizations in the planet. I was elated on finally achieving what I had dreamt for very long, it was one of the best moments of my life.

I sincerely hope to complete the project in the upcoming days with an utmost dedication. Regular blogs documenting my work and learning will be posted with the following being about the Community Bonding Period.

Looking forward to an exciting summer,  
  
Sanjiban.  
  
  
 
> 
Writing a technical blog for the first time was challenging but had some great help. Do read the following blogs, which inspired and helped me a lot in the process.
- ** [My journey to becoming a GSoC ’20 Student](https://medium.com/swlh/my-journey-to-becoming-a-gsoc-20-student-8c34a78e97ef) ** , by Rahul Saxena, my senior and a GSoC Student Developer with R-Project for 2020 and 2021.
- ** [Anirudh Dagar's GSoC Blog @ CERN-HSF](https://anirudhdagar.ml/gsoc/) **, by Anirudh Dagar, my mentor for the project and a GSoC Student Developer with CERN-HSF for 2020.
