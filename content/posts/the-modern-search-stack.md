---
title: "The Modern Search Stack and How it May Evolve"
date: "2024-11-20"
summary: "Information Retrieval is "
description: "An LSM Tree overview and Java implementation."
toc: true
readTime: true
autonumber: true
math: true
tags: ["machine learning", "project", "product strategy"]
showTags: true
hideBackToTop: false
hidePagination: false
draft: true
---

## LLM for Free Form Search
Large Language Models (LLMs) are transforming free-form search by enabling conversational and contextually aware experiences. Emerging tools such as SearchGPT and AI-powered overviews are setting a new standard for intuitive search experiences. For example, Perplexity AI combines advanced language modeling with search results, while Amazon Rufus leverages LLMs to enhance query understanding and relevance.

- SearchGPT
- AI Overviews
- Perplexity AI
- Amazon Rufus

https://searchengineland.com/searchgpt-what-you-need-to-know-446455
https://dl.acm.org/doi/10.1145/3534965


## Transformer Based Ranking
Transformers have significantly advanced the capabilities of search ranking models. With innovations such as BERT and RankFormer, search engines can now interpret nuanced queries and return highly relevant results. These models power search systems at companies like Google and Amazon, improving both accuracy and user satisfaction.

- BERT
- RankFormer
https://blog.google/products/search/how-ai-powers-great-search-results/ 
https://www.amazon.science/blog/leveraging-transformers-to-improve-product-retrieval-results 


## Continous Learning for Your Next Search
Modern users demand experiences tailored to their preferences and history. Continuous learning frameworks, such as Instagram Explore’s recommendation system, incorporate behavioral data, contextual signals, and user feedback to deliver results that feel uniquely personalized. These systems use reinforcement learning and multi-task learning to optimize relevance, engagement, and conversion rates.

- Instagram Explore Recommendation
- Video Recommendation

Modern users demand experiences tailored to their preferences and history. Personalization frameworks incorporate behavioral data, contextual signals, and user feedback to deliver results that feel uniquely tailored. These frameworks often rely on reinforcement learning and multi-task learning to optimize for multiple objectives, such as relevance, click-through rate, and conversion rate.

## Embedding Based Retrieval / Generative Query and Document Understanding
Traditional search systems relied heavily on term frequency-inverse document frequency (TF-IDF) and BM25 algorithms. While effective for their time, they lacked the nuance to understand semantic relationships. Enter neural ranking models, which leverage transformer architectures like BERT and GPT to understand context and intent at an unparalleled level. These models bring semantic relevance to the forefront, enabling more intuitive and satisfying search results.

Two-tower models have revolutionized how we match users and items in e-commerce, content platforms, and beyond. By learning separate embeddings for queries and documents (or users and items), these models enable fast and scalable retrieval, especially when paired with Approximate Nearest Neighbor (ANN) search techniques.

Vector search represents a paradigm shift in how information is indexed and retrieved. Instead of relying on tokenized text, it uses dense embeddings to capture the meaning and context of data. This is particularly useful for multimedia search, such as images, audio, and video, where traditional methods fall short.

- Paper: Query Understanding in the Age of LLMs https://arxiv.org/abs/2306.16004
- Paper: Query Intent Understanding with LLMs using Retrieval Augmentation and Multi-Stage Distillation https://aclanthology.org/2022.emnlp-industry.50.pdf
- https://medium.com/@siladityaghosh/unveiling-the-power-of-llm-frameworks-for-document-analysis-and-inquiry-8e6773fcb035
- https://medium.com/@addepto/how-to-use-llm-to-extract-information-from-documents-6395fcbc0291 

https://engineering.fb.com/2023/08/09/ml-applications/scaling-instagram-explore-recommendations-system/ 
https://newsroom.tiktok.com/en-us/how-tiktok-recommends-videos-for-you
https://blog.x.com/engineering/en_us/topics/infrastructure/2020/streaming-logging-pipeline-of-home-timeline-prediction-system 
https://arxiv.org/pdf/2006.11632
https://tech.instacart.com/optimizing-search-relevance-at-instacart-using-hybrid-retrieval-88cb579b959c
https://www.instacart.com/company/how-its-made/how-instacart-uses-embeddings-to-improve-search-relevance/
https://dl.acm.org/doi/10.1145/3534678.3539164
https://medium.com/better-ml/embedding-learning-for-retrieval-29af1c9a1e65

https://engineering.fb.com/2023/08/09/ml-applications/scaling-instagram-explore-recommendations-system/


Human in the Loop Active Learning for Ambiguous Queries
Human-in-the-loop systems, like Amazon’s Crowd Coachable Retriever, enhance search quality by incorporating crowd-sourced feedback. Google’s search quality rater guidelines similarly ensure that ambiguous queries yield useful results by leveraging human input.

- Amazon - Crowd Coachable Retriever https://www.amazon.science/publications/active-learning-with-crowd-sourcing-improves-information-retrieval
- Google search: How our quality raters make search results better https://support.google.com/websearch/answer/9281931?hl=en 
  - Search Quality Rater Guidelines: An Overview https://static.googleusercontent.com/media/guidelines.raterhub.com/en//searchqualityevaluatorguidelines.pdf

Graph Neural Networks
Graph Neural Networks (GNNs) are increasingly used to recommend related products, leveraging relational data between entities. Combined with real-time processing of user interactions, these models enable highly dynamic and context-aware search experiences.

https://www.amazon.science/blog/using-graph-neural-networks-to-recommend-related-products

Streaming User Interactions in Real time
https://blog.x.com/engineering/en_us/topics/infrastructure/2021/processing-billions-of-events-in-real-time-at-twitter-

Predictive Search - Query Suggestions
Predictive search systems, such as autocomplete and query suggestions, are being revolutionized by LLMs. These models go beyond simple word prediction, enabling smarter and more contextually aware user interactions.

https://www.algolia.com/blog/ai/predictive-search-and-autocomplete
LLMs as a smarter word predictor https://medium.com/@venkatesh.mymail/beyond-autocomplete-building-a-smarter-next-word-predictor-with-gpt-2-218bbc49775e
https://blog.personal.ai/autocomplete-ai-prompts-for-faster-recall-b34a7505b6b2

Reinforcement Learning for UI Module Layout
Optimizing UI layout dynamically can significantly enhance user experience. Reinforcement learning models, such as those used at Expedia and Amazon, adapt module layouts to maximize engagement and satisfaction.

https://medium.com/expedia-group-tech/multi-variate-web-optimisation-using-linear-contextual-bandits-567f563cb59
https://assets.amazon.science/92/9c/e2ab8a7640daabae51f87942a89a/a-map-of-bandits-for-ecommerce.pdf

Privacy Preserving Search
As privacy concerns grow, search systems are adopting privacy-preserving techniques to handle sensitive data securely. These methods include differential privacy and federated learning, ensuring user data remains protected while maintaining search relevance.

https://www.amazon.science/publications/privacy-preserving-active-learning-on-sensitive-data-for-user-intent-classification