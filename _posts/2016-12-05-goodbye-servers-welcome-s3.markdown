---
author: Karun Japhet
comments: true
title: Goodbye servers, welcome s3
slug: goodbye-servers-welcome-s3
date: 2016-12-05T02:04:56+05:30
layout: post
categories:
- Events
tags:
- news
- serverless
---

If you're a dev and you self host your blog, I'd love to hear why. Why do you self host blogs? For most simple blogs, esIn this day and age, migration to a static site like [Jekyll](https://wordpress.org/plugins/jekyll-exporter/) or [Octopress](https://jason.pureconcepts.net/2013/01/migrating-wordpress-octopress/) is pretty easy. I did this [a while back](https://blog.karun.me/blog/2015/11/28/movement-to-cybershark/). This can be followed up by asking [Amazon S3](https://davidwalsh.name/hosting-website-amazon-s3) to host your website. You can even [get cloudflare to front the SSL for free](https://blog.karun.me/blog/2015/02/01/forced-https-on-your-website-with-cloudflare/).

Why? S3 is free for the first year. Even post that period, my bills have been <$0.05 which is a **99.843% reduction in cost**.

## Continuous delivery

![HTTPs blog on S3]({{ site.url }}/images/uploads/https-blog-on-s3.jpg)

[Snap CI](https://snap-ci.com/) is will integrate with your publically accessible GitHub repositories for free and trigger builds on commit! Connect to your github repository and get it to compile your markdown into html. [Deploying to S3](https://docs.snap-ci.com/deployments/aws-deployments/aws-s3-deployments/) is a piece of cake. Congratulations on having continuous delivery for your blog!

[Cloudflare provides the free SSL](https://blog.karun.me/blog/2015/02/01/forced-https-on-your-website-with-cloudflare/) and Amazon S3 provides the [near free hosting](https://aws.amazon.com/s3/pricing/). A few cents a month to host your entire website is a good deal!

I've been on S3 for a year now and I couldn't be happier!
