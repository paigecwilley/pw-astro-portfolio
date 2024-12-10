---
title: Netflix Jobs site
publishDate: 2019-12-01 00:00:00
img: /assets/netflix_wordmark.jpg
img_alt: Netflix wordmark logo
description: |
  Architected several iterations of a jobs site to support discovery and application for career opportunities at Netflix.
tags:
  - NextJS
  - Apollo GraphQL
  - Contentful
---

Netflix came to Underbelly with a plan in 2017: Create a better hiring experience for candidates and Netflix.

For V2, Netflix wanted to highlight their diversity and inclusion initiatives and make it easier to hire for their various office locations.

 Working with a designer, I created the blog (including the Contentful model), moved the site from using a REST API to Graphql to query all content from Contentful, and updated designs or added features to every page.

### A new way to display media

Creating this grid was my favorite part of this project. Based on the designs, each row could have one, two, or three items and each item could be any number of content or media elements with its own constraints and requirements. Architecting this from both a content-modeling standpoint in Contentful and then creating and rendering all the components for that content was a lot of fun for me and a very interesting exercise!


### Moving to GraphQL

V1 of this project originally used the Contentful REST API. I started work on V2 using that API. Partway through the project, I decided the complexities of working with the more complex content could benefit from using GraphQL. I moved all the content-based pages over to Apollo GraphL,, and it definitely made iterating on the new design faster and cleaner.

### A home for content

V1 of the the jobs site didn't have a blog. For V2, Netflix knew they wanted to highlight the many experiences and people at Netflix with a blog. I created the content model for the blog in Contentful and created this page from the designs.