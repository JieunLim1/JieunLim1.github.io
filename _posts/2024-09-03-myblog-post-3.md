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

**Re;Magic** is a web-based tool that automatically converts caption files in **JSON format** into standard **VTT subtitles**—with built-in editing support. Designed for content creators, educators, and accessibility advocates, it streamlines the entire process of syncing captions to video scenes.

Just upload your JSON file and a YouTube link. Re;Magic will align the captions automatically. If anything is off, you can adjust the timestamps visually using our editor—no technical knowledge required.  
Once finalized, download the `.vtt` file and upload it wherever captions are supported.

Save time. Stay accurate. Keep control.

---

## Why did we build this?

We noticed that many editors—especially those working on educational or accessibility content—waste time manually aligning captions frame by frame. JSON is a common format for structured caption data, but most platforms only accept `.vtt` or `.srt`.

Re;Magic bridges that gap by **automating the conversion**, and providing an **intuitive UI** to review and adjust the results before export.

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
<img width="1470" alt="ImageTest" src="https://github.com/JieunLim1/Magic-front/blob/main/public/3.png?raw=true">
<img width="1470" alt="Image" src="https://github.com/JieunLim1/Magic-front/blob/main/public/4.png?raw=true" />
<img width="1470" alt="Image" src="https://github.com/JieunLim1/Magic-front/blob/main/public/5.png?raw=true" />


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

