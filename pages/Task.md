---
layout: page
title: Tasks
permalink: /task/
order: 2
feature-img: "assets/img/pexels-pixabay-373543.jpg"
---

<p>
The general goal of the WiC-ITA task is to establish if a word w occurring in two different sentences s<sub>1</sub> and s<sub>2</sub> has the same meaning or not.
In particular, our task is composed of two sub-tasks: the binary classification (Sub-task 1) and the ranking (Sub-task 2).
</p>


<h2>Sub-task 1: Binary Classification</h2>
<p align="justify">
Sub-task 1 is structured as follow:
Given a word <i>w</i> occurring in two different sentences s<sub>1</sub> and s<sub>2</sub>, the system has to assign a binary label to the sentence pair determining whether <i>w</i> maintains the same meaning or not.
The labeling system for this sub-task is:
 <ul>
  <li>0: the word <i>w</i> has not the same meaning in the two sentences s<sub>1</sub> and s<sub>2</sub>;</li>
  <li>1: the word <i>w</i> has the same meaning in the two sentences s<sub>1</sub> and s<sub>2</sub></li>
</ul> 

An example of output for Sub-task 1:
</p>
<img src="/assets/img/example2.png" alt="example2">




<h2>Sub-task 2: Ranking</h2>
<p align="justify">
Sub-task 2 is structured as follow:
Given a word <i>w</i> occurring in two different sentences s<sub>1</sub> and s<sub>2</sub>, the system has to assign a score to the sentence pair determining with which degree <i>w</i> has the same meaning in the two sentences. 
The scoring system for this sub-task is a continuous value where <i>score</i> &#8712; [1,4].
An higher score corresponds to an higher degree of semantic similarity.
<br>
An example of output for Sub-task 2:
</p>
<img src="/assets/img/example.png" alt="example">

