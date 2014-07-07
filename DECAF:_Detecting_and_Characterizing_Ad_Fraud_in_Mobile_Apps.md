DECAF: Detecting and Characterizing Ad Fraud in Mobile Apps
====
Bin Liu, Ramesh Govindan

## The contributions of this paper are:
> 1. Present the design and implementation of a scalable system for automatically detecting ad placement fraud in mobile apps.
> 2. Characterize the prevalence of ad placement fraud and how these frauds correlate with app raings, app categories, and other factors.

## About Placement frauds
  Advertising in mobile apps is plagued by various types of frauds. The frauds fall under two main categories: *Bot-driven frauds* and *Placement frauds*.
> Bot-driven frauds employ bot networks or paid users to initiate fakead impressions and clicks.
> Placement frauds manipulate visual layouts of ads to trigger ad impressions and unintentional clicks from real users.

  Instead of analyzing server-side logs, the authors explore a qualitatively different approach: to detect fraudulent behavior by analyzing the structure of the app, an approach that can detect placement frauds more effectively and before an app is used.  
  This paper consider two categories of placement frauds: *Structural frauds*, relate to how the ad controls are placed and *Contextual frauds*, place ads in inappropriate contexts.

## Decaf Overview
  DECAF is designed to automatically discover various placement frauds scalably and effectively. DECAF performs dynamic checking in which it checks the implementation of an app by directly executing it in an emulator.  
  It employs an automation tool called a Monkey that can automatically execute it and navigate to various parts, together with optimizations to scan through a large number of visual elements within a limited time.  
  It includes a framework for efficiently detecting whether ads within an app violate an extensible set of rules that govern adplacement and display. At each state, DECAF invokes the fraud checker that has a set of detectors. The Extension of the fraud checker includes the following detectors: small ads, hidden ads, intrusive ads, many ads, and inappropriate context.

## Optimizations for Coverage and Speed
  In this section, the authors develop various techniques to address coverage and speed problem.
  
#### 1. Detecting Equivalent States
  To optimize coverage, DECAF uses a different notion of state equivalence. First, the equivalence should be decided based on fuzzy matching. Second, the equivalence function should be tunable. To compare if two states are equivalent, they compute cosine similarity and consiter them if the cosine similarity is above a threshold.
  
#### 2. Path Prioritization
  Many (especially tablet) apps contain too many states for a Monkey to explore within a limited time budget. To address this, DECAF uses a novel state equivalence prediction method to prioritize which paths to traverse in the UI graph for detecting structural fraud and a novel state importance assessment for detecting contextual fraud.
##### 1) State Equivalence Prediction
  To motivate state equivalence prediction, the authors consider two following points.
  Backward transitions can be expensive. Minimizing state traversal overhead using prediction.
##### 2) State Importance Assessment
  Using app usage for estimating state importance. Prioritizing state traversal using state importance.
#### 3. Page Load Completion Detection
  DECAF has no way of knowing when the page has loaded in order to check state equivalence. DECAF uses a simpler and app language-agnostic technique to monitors all I/O activities of the app process, and maintains their sum over a sliding window of time T. The method has the virtue of simplicity, but comes at a small cost of latency, given by sliding window length, to detect the page load.

#### 4. Fraud Checker Optimizations
Detecting too many ads.
Detecting hidden and intrusive ads.



## Evaluation
#### 1. State Equivalence Prediction
#### 2. Assessing State Importance
#### 3. Overall Speed and Throughput

## Characterizing Ad Fraud
#### Fraud by Type
#### Fraud by App Category
#### Frauds by rating
#### The propensity of publishers to commit fraud.
#### Takeaways
