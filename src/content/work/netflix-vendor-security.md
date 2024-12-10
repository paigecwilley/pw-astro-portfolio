---
title: Netflix vendor security
publishDate: 2020-03-04 00:00:00
img: /assets/netflix_wordmark.jpg
img_alt: netflix workmark logo
description: |
  A tool to assess vendor security for every Netflix tool or partner - from THX to catering.
tags:
  - NextJS
  - Apollo GraphQL
  - TypeORM
  - Typescript
---

## Mountains of evolving data in one place
A tool for receiving, viewing, and editing a lot of data. Includes a Google Forms-style survey builder (pictured).

As this is an internal Netflix tool, I can't say a ton about it. Here's what I can tell you: Netflix needed a tool for receiving, viewing, and editing A LOT of data. They also needed a custom survey builder tool that did everything Google Forms does and then some. I built the front-end for this project and queried all the data from the database our backend engineer built using a Graphql server. I built countless tables and grids for displaying data and just as many inputs for altering data (so many mutations!)

### Duplicating Google Forms

The Netflix team on this project needed a way to create surveys similar to Google Forms to send but integrated into the tool and able to handle additional data points. This had a lot of fun features like dragging and dropping of sections and questions, figuring out how to add and remove questions and sections anywhere, and handling multiple kinds of inputs.

### A comment section that's not scary

Part of the project required a 'feedback' and 'comment' section on one page. This part of the project intimidated me initially from both a ui and a mutation standpoint. Some of this feature's unique challenges included creating a 'recursive ui', making sure a list of 'infinite' comments showed up 'like in Facebook', adding @ mentions to other users, and debouncing.

### A diff engine for at-a-glance assessments 

This is the part of the project I'm most proud of. Netflix wanted to compare similar sets of data over time. If the data for October was different from September, I highlighted how it was different by showing both October and September’s data and highlighting in the October data what had changed, been removed, or been added from the September data (the colored outlines in the image). This involved comparing large sets of data to each other and manipulating the data in such a way that we could still see everything we needed.
