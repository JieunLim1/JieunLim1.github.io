---
title: 'Blog Post number 1'
date: 2023-08-08
permalink: /posts/2012/08/blog-post-1/
tags:
  - cool posts
  - category1
  - category2
---
# Heading
To Help You Survive in College
---
# Open-Sourcing Q&A Generator machine with GPT!

# TL;DR

This is an application that is developed for people, especially for students who would like to test themselves by reviewing materials. It creates problems based on the context that is provided by the user (it may be a note from lectures or a weblink from Notion). 
What makes it special is that it not simply creates problems but creates various questions that do not repeat as the user wants. It also checks the answer written by the user and provides feedback that guides the user to the points that could be improved.
DO NOT CRAM BEFORE THE TEST DAY!

There exist AI question-generating machines that simply create one question out of time. Or there exist machines that output the same question again and again as long as the text is the same. But what if it creates a test paper with various questions that are categorized by the subjects? This is where Q&A Generator machine comes in. 

![IMG_0364](https://github.com/JieunLim1/JieunLim1.github.io/assets/136796436/92afcbe8-66a5-42ac-a4ca-31bc5554210d)
![IMG_0366](https://github.com/JieunLim1/JieunLim1.github.io/assets/136796436/83614522-653b-429f-8a61-4a8546725142)

The system consists of two blocks(not obviously), which are the question generator and response (answer key matching) blocks. 
The first block is responsible for creating questions as many as the user orders according to the given context. The context could be a text or weblink for notes in Notion, which makes college students much more convenient as it reduces their task to copy and paste lecture notes. The system requires the machine to generate different questions from each other to make sure that the test paper covers the full content of the context. 

As shown in the figure, each chain has a corresponding memory object. It saves the context, generated questions, user’s responses, and results with its own ID value. When one loop in a block is done, it sends the data back to the beginning of the next loop so that it does not duplicate making the same questions again.  

The final block, or marking chain, is in charge of marking the user’s response based on the "Model Answer", or an answer provided when generating the question". After, it saves the results on its system so that it makes the next version of reviewing material collected by previous incorrect questions. 
To add on, while reviewing, the most significant thing is to know what to study and make up the gap in knowledge. The machine notices the answer but also "Things to improve" in order to assist the full review process.

To jump into the memory part, this is how the relational information is saved. 
![image](https://github.com/JieunLim1/JieunLim1.github.io/assets/136796436/c5ac44db-0b93-4f0b-b498-4b7ead2d6899)
The image shows the ERD ( Entity Relational Diagram ). 

* Data Normalization
  The benefit of normalization, or splitting the tables into separate tables, is to reduce the duplication of unnecessary columns and anomalies (a phenomenon that could occur while adding, editing, and deleting the data).
  Another special function of this application is that it creates a paper that collects all the incorrect questions the user gets from a certain subject. This is an example of using the join function that joins the split data.
  
