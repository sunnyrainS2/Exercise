DECAF: Detecting and Characterizing Ad Fraud in Mobile Apps
====
Bin Liu, Ramesh Govindan

## The contributions of this paper are:
> 1. Present the design and implementation of a scalable system for automatically detecting ad placement fraud in mobile apps.
> 2. Characterize the prevalence of ad placement fraud and how these frauds correlate with app raings, app categories, and other factors.

## Background
  Advertising in mobile apps is plagued by various types of frauds. The frauds fall under two main categories: *Bot-driven frauds* and *Placement frauds*. Bot-driven frauds employ bot networks or paid users to initiate fakead impressions and clicks. Placement frauds manipulate visual layouts of ads to trigger ad impressions and unintentional clicks from real users.  
  Instead of analyzing server-side logs, the authors explore a qualitatively different approach: to detect fraudulent behavior by analyzing the structure of the app, an approach that can detect placement frauds more effectively and before an app is used.  
  This paper consider two categories of placement frauds: *Structural frauds*, relate to how the ad controls are placed and *Contextual frauds*, place ads in inappropriate contexts.

## Decaf Overview

## Optimizations for Coverage and Speed

## Evaluation

## Characterizing Ad Fraud
