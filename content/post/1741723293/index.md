---
date: 2025-03-11 20:01:33+0000
draft: false
title: 'RAG: Not a Silver Bullet?'
categories: ['Micro']
slug: 1741723293
math: true
---

## A Few Ideas About RAG

As I keep pouring in efforts to build [LiveAPI](https://hexmos.com/liveapi/), I get new ideas on how to make it better from time to time.

There is a constant feeling that maybe we should have some sort of Chatbot on top of the structured API information we generate at scale.

People say:

"Nobody reads documentation these days"

"I don't think anyone will read docs anymore"

"Nobody cares about documentation. Code is documentation"

And so on.

What they also sort of imply is that - we just want to ask a Chatbot or be surfaced with the relevant information automagically in the right place at the right time.

## We may build a Chatbot - at some point in the future

But for now - this post will be about one of the approaches to building Chatbots that seems to be making noise across places like Hacker News - called "RAG"

RAG stands for Retrieval Augmented Generation

The LLM in its primordial state is like our long-term memory or impressions. It sort of has a vague recollection of facts, ideas and sentiments. But it has to be grounded with something more concrete - before a specific answer can be given.

RAG is about - helping the LLM remember better, while also helping it transform current or specific information into the framework of its answers.

## RAG Flaws - Still too literal

I've heard from multiple quarters - with those having comparatively deeper knowledge on the topic that RAGs often underperform.

"Just tag your docs with keywords - don't bother with RAG"

I've heard the above opinion expressed multiple times.

Consider the following case mentioned on an [HN Thread](https://news.ycombinator.com/item?id=42174829).

There's a textual records of various activities performed day to day by a bunch of people.

Now we are curious - "Guess the occupation of person X"

The augmentation happens purely based on the keywords present in this question.

Imagine now person X has been going to various chemistry conferences, etc but her occupation is not mentioned anywhere.

Pure RAG approaches most probably will fail here because they cannot connect "attends chemistry conference" to "occupation" - because the keywords are sort of different

## What is the way around?

For things like above - we fall back to the old search and information retrieval mechanisms.

We build a semantic graph - putting related nodes together.

We do PageRank, or similar alternatives.

We essentially do search first.

The LLM layer is mostly good for "summarizing" the findings.

So - the role of something like RAG becomes much more limited, or sometimes even irrelevant.

Many AI apps may end up with Search followed by Summarization.
