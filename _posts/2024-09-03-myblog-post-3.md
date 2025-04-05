---
title: 'Re;Magic'
date: 2024-09-10
permalink: /posts/jieun-blog-post-3/
tags:
  - video editing
  - subtitles
  - react
---

# Editing Made Easy, Magic Made Real 
---

# All in one with Re;Magic!

---

# TL;DR

**Re;Magic** is a web-based tool that automates the process of syncing YouTube video scenes with subtitle files using JSON input. Designed for content creators, educators, and students, it eliminates the need for manual timestamp adjustments.  
If the system detects mismatched captions, the user can easily **edit the timeline** through an intuitive interface. In the end, Re;Magic exports the finalized subtitle file as a **.vtt**, ready to be used on YouTube or other platforms.

Ever spent hours adjusting subtitles to match your video timeline? That’s where **Re;Magic** comes in—it saves time and makes the editing process smarter and cleaner. 🧠⚙️

---

## Why did we build this?

We noticed that a lot of video editors, especially those working with lectures or content for accessibility, waste hours trying to match captions with fast-moving scenes. JSON-formatted captions are great for structure but frustrating to edit manually. So, we asked ourselves:

**"What if we could build a smart tool that aligns it all for you?"**

And that’s how Re;Magic was born.

---

## How does it work?

The system takes two inputs:
- A **YouTube video URL**
- A **JSON-formatted file** with subtitle content and estimated timestamps

It then parses the video and attempts to match subtitles to scenes using the given data. If the initial match is off, the user can **manually fine-tune** the timestamps using a timeline editor—just like in a basic video editing app.

After adjustments are done, Re;Magic generates a **.vtt file** that can be uploaded directly to platforms that support captioning.

---

## Features

**Auto-Matching**  
Automatically matches subtitles with the video timeline using JSON metadata.

**Manual Editing**  
Fix any mismatches with ease.

**VTT File Export**  
Exports clean subtitle files in `.vtt` format for easy upload.

**Simple UI**  
Built with **React** for a responsive and lightweight experience.

---

## Screenshot Preview

<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/2459dce1-6844-41a2-8c72-58078ecf549e" />
<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/e3481870-43a0-43fa-bf5e-4012fb86ca3f" />
<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/83a3635a-a84c-4d54-a15c-0b3137975656" />
<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/df29a9dd-9b86-4a94-b869-c6328423e075" />
<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/4cd3327f-7d6f-4731-9a4b-d8aef1b6477f" />
<img width="1470" alt="Image" src="https://github.com/user-attachments/assets/8d3997f4-274b-485c-b9f7-0eb5422fcae3" />

---

## Challenges & Learnings

One challenge I faced was ensuring **accurate syncing** when the JSON timestamps were vague or inconsistent. To address this, we included frame-based scrubbing and implemented buffer ranges around scene boundaries.

We also learned how important **user control** is—even with automation, giving users manual override capabilities made the tool more trustworthy and flexible.

---

## What’s next?

We’re looking into:
- Supporting **multiple languages** in captions
- ONLY require Youtube url link as an input
- video editing functions (adding and trimming)  
- Adding **.srt export** options  
- Improving auto-matching accuracy with **scene detection AI**

---

## Tech Stack

**Front-end:** React  
**Data Handling:** JavaScript, JSON  
**Export Format:** WebVTT (`.vtt`)

---

If you're tired of dragging timestamps manually or want to make your video content more accessible without the stress—**Re;Magic is for you.**  
Let the magic match it for you. 

