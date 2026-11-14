---
title: "MAT 221: Statistics"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/SVU_M221
venue: "Southern Virginia University"
date: 2026-08-26
location: "Buena Vista, Virginia"
---

An introduction to probability and statistics: describing data, experimental design, regression, probability models, confidence intervals, hypothesis testing, and analysis of variance.

## About the course

This is the statistics course most SVU students take. It covers describing data, experimental design, probability and probability models, confidence intervals, hypothesis testing, chi-square tests, regression, and analysis of variance.

Two commitments shape the course. First, we do our computing in Excel or Google Sheets. Graphing calculators can do a great deal of statistics, but they are not what people use in the workforce, so students are tested on doing the analysis in a spreadsheet. Second, statistics does not live in a textbook. It lives in the news, in advertising, in published research, and in the arguments people make to persuade you of things, and the course keeps sending students out to meet it there.

My goal is not merely that students *know* the material but that they can *do* it: handed a data set and a question, they know how to proceed. That skill is built by doing, in the room, with help nearby. So the reading happens before class, and class time is spent working.

## How a lesson works

Every lesson runs on a **Lesson Guide**, a packet with two halves: a Pre-Reading half that students complete before class, and an In-Class half that we complete together.

### Before class: the Pre-Reading

Each guide opens with a numbered list of learning objectives for the day, tied to the sections of the textbook. Students then read those sections with the guide beside them. The Pre-Reading is structured note-taking, not busywork:

- **Key statements with blanks.** The main sentences of the chapter, with the important words left out for the student to supply while reading.
- **Definitions in your own words.** Each new term gets a space where the student explains it, not copies it.
- **The book's examples, worked.** The guide walks through the textbook's own examples, so students have already tried the central calculations once before we meet.
- **Checks for understanding.** Short "explain what this means" questions at the points where students most often go wrong.

The guide also lists optional video lectures that follow the same textbook and work in Excel, for students who want a second explanation.

After the reading, students take a short **Pre-Reading Quiz**. It is open book and open note, but not open AI. Both are due before class. Because the class discussion depends on everyone arriving prepared, no Lesson Guide score is ever dropped.

### In class: recall, a mini-lecture, and extension exercises

The In-Class half of the guide is mostly questions, with only a brief stretch of me talking. It has three parts, in the same order every day.

1. **Recall and Discourse.** We begin with the day's terms and concepts, and students describe each one in their own words, first from memory and then to each other. Pulling ideas back out of memory interrupts forgetting and strengthens retention; explaining them to someone else deepens understanding. Students should expect to be called on.
2. **Mini-Lecture.** About a page of what I add to the reading: clarifications, the mistakes I see most often, why the idea matters, and the Excel functions for the day with their syntax, such as `NORM.DIST` or `BINOM.DIST`. When we reach hypothesis testing, for example, this is where the courtroom analogy lives: the null hypothesis is "the defendant is innocent," and a verdict of "not guilty" does not declare anyone innocent.
3. **Extension Exercises.** This is where most of the class period goes. I choose three or four examples from the day's reading, usually ones students already worked in the Pre-Reading, and write a fresh exercise for each: the same ideas in a new setting, and only slightly harder. One thing changes at a time. The question is reversed, "exactly" becomes "at least," or a follow-up asks what happens if a condition fails. Each exercise is labeled with the textbook example it extends, so a student who is stuck knows exactly where to look. We work these together, and students put steps on the board, explain why they chose the method they chose, and say where they got stuck.

Reading a worked example and watching someone else solve a problem are not the same as solving it yourself. It is easy to leave a class feeling that everything made sense and then sit down in front of a blank spreadsheet and not know where to begin. The extension exercises are designed to close that gap while help is still in the room, and the participation grade rewards the work they require.

### After class

Students practice in an online homework system with immediate feedback, and submit **Written Work**, the handwritten reasoning behind selected homework problems. About once a week there is a short **Weekly Quiz**, written in the same spirit as the exams, as a low-stakes rehearsal.

Each unit ends with a **Celebration of Knowledge**. Do not let the name fool you: it is a midterm exam. But it is also a chance to see how far you have come.

## The units

### Unit 1: Describing data (Chapters 1–2)

The course begins with the language of statistics: populations and samples, parameters and statistics, types of data and levels of measurement, and how samples are drawn. We then look at how studies are designed. Students learn to tell an observational study from an experiment, to see why randomization and blinding matter, and to spot confounding variables and sources of bias.

The second half of the unit is about summarizing data. Students build and read frequency tables, stemplots, histograms, and box plots; compute percentiles, quartiles, the mean, median, and mode; and measure spread with the range, interquartile range, variance, and standard deviation. They learn which measure of center suits a skewed distribution, how z-scores and the Empirical Rule locate a value within a distribution, and how to recognize a graph that misleads.

The unit closes with an introduction to the In the Wild assignments, so students start applying these ideas to real claims right away.

### Unit 2: Probability and probability models (Chapters 3–7)

Unit 2 builds the machinery that inference depends on. It starts with the basics of probability: three ways of assigning a probability, the addition and multiplication rules, independence versus mutual exclusivity, and conditional probability. Two-way tables get special attention, including false positives and false negatives in medical testing.

From there we turn to random variables as models of real situations. Students compute expected values and standard deviations, then meet the named models one at a time: the binomial, geometric, and Poisson distributions for counts, and the uniform and exponential distributions for continuous measurements, where probability becomes area under a curve. For each model the questions are the same. What conditions make it fit? What are its parameters? How do we compute with it in Excel?

The unit then slows down for the normal distribution, with a full day of practice, and finishes with the Central Limit Theorem: why averages of samples behave predictably even when individual values do not. This is the idea on which the rest of the course rests.

### Unit 3: Statistical inference (Chapters 8–12)

Unit 3 is the heart of the course: using a sample to say something about a population. We begin with point estimates and confidence intervals for means and proportions, including when to use the t-distribution and how large a sample must be.

Hypothesis testing takes two days. Students learn to state null and alternative hypotheses, to understand Type I and Type II errors and the trade-off between them, to compute a test statistic and p-value, and to state a conclusion in plain language. We then extend the idea to comparing two groups (independent samples, paired samples, and two proportions), to chi-square tests for goodness of fit, independence, and homogeneity, and to correlation and linear regression.

In this unit, class time shifts toward theory and judgment. Students have worked examples in the reading and videos, so we spend more of our time on why the methods work, on effect size (Cohen's d) as distinct from statistical significance, on the meaning of the two kinds of error, and above all on choosing the right test for a given question.

### The final weeks: modeling, ANOVA, and the bootstrap

After the third Celebration, the course looks outward. We use regression for prediction, and discuss the risks of extrapolation and the influence of outliers. We study one-way analysis of variance for comparing several groups at once. The last new topic is bootstrapping, a general, computer-based approach to inference that goes beyond the textbook.

The semester ends with student project presentations and a comprehensive final exam. Where each Celebration looks at a single unit, the final asks students to hold the whole course at once: to look at a question and know which tool it calls for, and why.

## In the Wild

These assignments run through the whole semester and come in three kinds.

- **Statistics in the wild.** Students find statistics in a news article, an advertisement, or a published paper and analyze the claims being made. What was the population? What was the sample? Does the conclusion actually follow from the data?
- **Modeling a real situation.** Students describe something in the world that one of our probability models actually fits, estimate its parameters, use the model to make a prediction, and, where the data exist, check whether the prediction held up.
- **Small projects with real data.** Students locate or gather a real data set and analyze it with the methods of the course. These are small and deliberately imperfect. The data may be biased or messy, and that is part of the lesson.

Alongside these runs a standing hunt for **statistical malpractice**: a misapplied test, a misleading graph, a conclusion the data cannot support. The first student to find and document a genuine instance earns extra credit. The test is whether the thing actually misleads, not whether a rule was broken.

**Textbook:** [*Introductory Statistics*](https://openstax.org/details/books/introductory-statistics) from OpenStax, free online.

**Prerequisite:** MAT 114: Finite Mathematics or MAT 115: College Algebra.

## Syllabus (Fall 2026)

- [Course Policies](/files/teaching/files-SVU-M221/syllabus/M221-Course_Policies-Fa26.pdf)
- [Course Schedule](/files/teaching/files-SVU-M221/syllabus/M221-Schedule-Fa26.pdf)

## Helpful resources

- [Seeing Theory](https://seeing-theory.brown.edu/). A visual, interactive introduction to probability and statistics. Excellent for building intuition about sampling distributions and confidence intervals.
- [StatKey](https://www.lock5stat.com/StatKey/). Free in-browser tools for simulating sampling, bootstrap confidence intervals, and randomization tests.
- [Khan Academy: Statistics and Probability](https://www.khanacademy.org/math/statistics-probability). Extra explanations and practice problems for every unit.
- [My YouTube channel](https://www.youtube.com/@JaredMcBrideMath). Lesson videos I have recorded.

## Data sets

**ANOVA lesson**

- [Pulse Data](/files/teaching/files-SVU-M221/ANOVA_Pulse_Grouped.csv)
- [Arsenic Data](/files/teaching/files-SVU-M221/ANOVA_Arsenic.csv)
- [Speed Dating Data](/files/teaching/files-SVU-M221/ANOVA_Speed_Dating.csv)
- [NFL Weights Data](/files/teaching/files-SVU-M221/ANOVA_NFL.csv)
- [NFL Raw Data](/files/teaching/files-SVU-M221/NFL.csv)
- [Student Performance](/files/teaching/files-SVU-M221/StudentsPerformance.csv)

**Finale prep**

- [Course Evaluations](/files/teaching/files-SVU-M221/FinalePrep-CourseEvals.csv)
- [NBA](/files/teaching/files-SVU-M221/FinalePrep-NBA.csv)
- [Sub Shops](/files/teaching/files-SVU-M221/FinalePrep-SubShops.csv)
- [Word Counts](/files/teaching/files-SVU-M221/FinalePrep-WordCounts.csv)

**Finale**

- [Presidents](/files/teaching/files-SVU-M221/01-Presidents.csv)
- [NFL](/files/teaching/files-SVU-M221/02-NFL.csv)
- [Olympics](/files/teaching/files-SVU-M221/03-Olympics.csv)
- [Netflix](/files/teaching/files-SVU-M221/04-Netflix.csv)
- [Bears](/files/teaching/files-SVU-M221/05-Bears.csv)
- [Fast Food](/files/teaching/files-SVU-M221/06-FastFood.csv)
- [Premier League](/files/teaching/files-SVU-M221/07-PremierLeague.csv)
