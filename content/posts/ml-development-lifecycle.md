---
title: "Building ML Products that work"
date: "2026-01-04"
summary: "A system that has worked well for me for large, ambiguous ML project undertakings."
description: "How to work on ambiguous ML projects"
toc: true
readTime: true
autonumber: true
math: true
tags: ["machine learning", "project", "product strategy"]
showTags: true
hideBackToTop: false
hidePagination: false
draft: false
---

Some of the best work I have seen come out of the teams I have lead involved some spark of curiosity: a hypothesis about how to make things better for users. Over many such projects, I have found that a systematic approach is invaluable for turning such ideas into reality. The system is there not to impede or create friction but to provide a framework for exploration. This is especially critical for Machine Learning Engineers because while we are given a million parameters to play with to refine our objective functions, the path to success is filled with ambiguity and dead ends. A systematic approach to such work prevents burn out and keeps the creativity engine fueled.

## Hypothesis-Driven Model Development

The cornerstone of successful ML projects is a hypothesis-driven approach. Each project begins with a question: “If we improve certain parts of the ML system, can we solve a consumer problem and impact key metrics?” To answer this, we follow a sequence of well-defined steps:

1. **Hypothesis Generation**
   - Identify the problem: Frame the specific user issue or business challenge as a consumer problem.
   - Link the problem to metrics: Define measurable offline, input, and output metrics.
   - Develop a chain of hypotheses: Establish a logical flow of cause and effect, where each hypothesis can be validated incrementally.

2. **Feasibility Study**
   - Conduct exploratory data analysis (EDA): Assess data availability, quality, and relevance.
   - Review existing solutions: Learn from industry practices and academic literature.
   - Investigate systems: Understand infrastructure limitations and opportunities for integration.
   - Scope the project: Draft a detailed roadmap with milestones.

3. **Implementation**
   - Build offline models: Develop pipelines, train models, and enhance retrieval/ranking systems.
   - Iterate on system-level components: Integrate metadata ingestion, retrieval, ranking, and reranking pipelines.

4. **Evaluation**
   - Offline metrics: Validate using metrics like Precision, Recall, and NDCG.
   - Online metrics: Use A/B tests to measure impact on key business outcomes like customer spend and order rates.

5. **Productionization**
   - Deploy models: Integrate solutions into production systems, ensuring robustness and scalability.
   - Monitor results: Analyze real-time performance and identify areas for further improvement.

## The Power of Hypotheses

A hypothesis is more than an educated guess; it’s a roadmap for experimentation. By breaking down a big idea into smaller, testable hypotheses, you ensure that every step is rooted in data and aligned with business goals.

### Example: Improving Subtotals with Personalized Recommendations

**Good Hypotheses Chain:**
- **Hypothesis:** Showing higher-priced items in categories users prefer will nudge them toward higher subtotals.
- **Implementation:** Enhance the ranking system with features like price sensitivity and historical purchase weights.
- **Evaluation:** Measure the average price of top recommendations and ensure user engagement remains stable.

**Bad Hypotheses Chain:**
- **Hypothesis:** Boosting higher-priced items will increase subtotals.
- **Implementation:** Apply a blanket rule to prioritize expensive items.
- **Evaluation:** Skip intermediate validation, assuming the solution will work.

The first approach validates assumptions incrementally, reducing risks and ensuring outcomes align with user needs.

## Key Phases in the ML Development Life Cycle

### **Hypothesis Generation**
Start by observing user behaviors, analyzing product metrics, and identifying opportunities. Frame your problem as a series of questions linked to measurable outcomes.

### **Feasibility Study**
Explore the data and system infrastructure to determine the viability of your solution. For instance, if your hypothesis involves user purchase behavior, ensure you have the necessary data on spending patterns and item categories.

### **Implementation**
Develop both system-level and model-level components:

- **System-Level Components:** Enhance ingestion pipelines, retrieval algorithms, ranking models, and reranking systems.
- **Model-Level Components:** Focus on training data, feature engineering, labels, objectives, and architecture.

### **Evaluation**
Evaluate your solution rigorously:

- **Offline Metrics:** Validate model quality with historical data.
- **Online Metrics:** Use A/B tests to assess real-world impact.

### **Productionization**
Deploy your solution, monitor its performance, and iterate based on user feedback and live metrics.

## Lessons Learned

1. **Collaboration is Key:** ML projects thrive on cross-functional collaboration. Bring together product managers, engineers, analysts, and stakeholders early and often.
2. **Data Drives Decisions:** Let data guide your hypotheses, implementation, and evaluation.
3. **Iterate Relentlessly:** Hypotheses often evolve. Be ready to pivot based on findings.

## Conclusion

Personalization is both an art and a science. By following a hypothesis-driven framework, you can tackle complex problems methodically, align your team’s efforts, and deliver measurable impact. Whether you’re optimizing recommendations, improving engagement, or driving revenue, this approach will help you navigate the challenges of ML development with confidence.

