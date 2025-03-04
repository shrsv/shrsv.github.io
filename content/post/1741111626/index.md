
---
date: 2025-03-04 18:07:06+0000
draft: false
title: 'LiveAPI Rebuilt: A Scalable and Reliable API Documentation Tool'
categories: ['Micro']
slug: 1741111626
math: true
---

Hi there! I'm Shrijith Venkatrama, founder of Hexmos. Right now, I’m building [LiveAPI](https://hexmos.com/liveapi), a tool designed to make generating API documentation from your code incredibly easy.

Over the past few months, we’ve been hard at work refining LiveAPI to be more robust, scalable, and user-friendly. Here’s a look at what we’ve been up to.

## What We Did in November and December

Towards the end of last year, we ramped up our outreach efforts, connecting with engineering leaders, CTOs, technical freelancers, and experienced developers. Many of them were generous enough to try out LiveAPI and provide us with invaluable feedback.

We closely observed how users onboarded, interacted with, and benefited from LiveAPI. What became clear was that while the concept was strong, the product needed significant improvements before it could truly serve the needs of professional developers. With that realization, we dedicated the past three months to making fundamental enhancements.

## Identifying Key Issues

Through our interactions and testing, we uncovered several major pain points:

-   **Handling Large Codebases**: Many users experienced failures when processing large repositories, making the tool impractical for sizable projects.

-   **Challenges with Multi-Project Repos**: Codebases structured as monorepos or with multiple subprojects often encountered errors.

-   **Pricing Concerns**: Users expressed a preference for API-count-based pricing rather than a repository-based model.

-   **Lack of Framework Support**: Several critical frameworks were missing from our compatibility list, limiting adoption.

-   **Accuracy Issues**: Due to size limitations, the accuracy of generated documentation was sometimes inconsistent.

-   **Unstable LLM API Calls**: Intermittent failures occurred when making LLM-based API calls, and we lacked a robust retry mechanism.

-   **Uninspiring Documentation Design**: The generated documentation needed a more polished, professional, and visually appealing design.


## Re-Architecting LiveAPI: The Solution

Initially, we thought we could address these issues with incremental fixes. However, as we dug deeper, it became clear that a more fundamental overhaul was necessary. Over the past three months, we completely re-architected LiveAPI’s backend to build a more stable and scalable system.

-   **Event-Driven Architecture**: We transitioned to a fully event-driven approach, ensuring better scalability and responsiveness.

-   **Redis-Powered Queues and Streams**: We adopted Redis to efficiently manage queues, data structures, events, and streams, significantly improving performance.

-   **Reliable LLM Interactions**: We developed new mechanisms to enhance the reliability of LLM-based API calls, minimizing failures and improving consistency.

-   **Scalability for Large Repos**: We tackled repository size limitations, enabling us to generate documentation for 150-200 APIs per project with ease. This number is expected to grow further as our optimizations continue.

-   **Future-Proof Infrastructure**: The event-driven architecture allows us to scale dynamically based on demand, ensuring a seamless experience for users.

-   **Enhanced Documentation Design**: Improving the documentation layout and visual appeal required a steep learning curve for our team, but the result is a much more engaging and professional output.


## The New and Improved LiveAPI: What’s Next?

With these changes in place, LiveAPI now offers:

-   **Higher Reliability**: Automated document generation is now far more stable and dependable.

-   **Better Support for Large Repositories**: Even complex, multi-project repos can be processed with ease.

-   **Visually Appealing Documentation**: The new design makes API documentation more readable and professional.

-   **Improved Accuracy**: The enhancements result in more precise and complete API documentation.

-   **Support 60+ Frameworks**: We now support the top 15 languages and around 60 frameworks within them


We’re incredibly excited about these improvements and can’t wait to share them with our users. Stay tuned for the official release of the new LiveAPI, and if you haven’t tried it yet, now’s a great time to check it out!
