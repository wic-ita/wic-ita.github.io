---
layout: page
title: Submit your results
permalink: /submit/
order: 3
feature-img: "assets/img/pexels-pixabay-159751.jpg"
---


<script>
const ul = document.getElementsByTagName("nav")[0].getElementsByTagName("ul")[0];
ul.innerHTML = `
            <li>
                <a class="clear" aria-label="Home" title="Home" href="/index.html">
                     Home 
                </a>
            </li>
            <li class="separator"> | </li>
            <li>
                <a class="clear" aria-label="Tasks" title="Tasks" href="/task/">
                     Tasks 
                </a>
            </li>
            <li class="separator"> | </li>
            <li>
                <a class="clear" aria-label="Data" title="Data" href="/data/">
                     Data 
                </a>
            </li>
            <li class="separator"> | </li>
            <li>
                <a class="clear" aria-label="Important Dates" title="Important Dates" href="/dates/">
                     Important Dates 
                </a>
            </li>
            <li class="separator"> | </li>
            <li>
                <a class="clear" aria-label="Organizers" title="Organizers" href="/organizers/">
                     Organizers 
                </a>
            </li>
            <li class="separator"> | </li>
        <li class="separator"> | </li>
            <li>
            	<a id="theme-toggle" title="Home " aria-label="Home" onclick="themeToggle()">
            		<i class="fas fa-adjust" aria-hidden="true"></i>
            	</a>
            </li>
`;
</script>



We provide all datasets in the JSON Lines text format containing one example for each line. 

Datasets are available at <a href="https://github.com/wic-ita/data">https://github.com/wic-ita/data</a>


<h1>Subtask 1: Binary Classification</h1>
We provide two datasets for model development:
<ul>
	<li>The <i>train.jsonl</i> which consists of 2,805 training examples. This dataset should be employed to train the model</li>
	<li>The <i>dev.jsonl</i> which consists of 500 training examples. This dataset should be employed to evaluate the model in the training phase, e.g., tune hyper-parameters </li>
</ul>

The training dataset (<i>train.jsonl</i>) is highly unbalanced, consisting of about 71.27% of positive and 28.73% of negative examples. At the same time, we provide a balanced development set (<i>development.jsonl</i>) consisting of 50% positive and 50% of negative examples.
Further, the dev set includes 250 examples where the target word is out of the vocabulary, i.e., the target word never appears in the training set.
For each In-Vocabulary target word of the development set, at least one positive and one negative example are provided in the training set.



<h1>Subtask 2: Ranking</h1>
We provide four datasets for model development:
The <i>train_agr.jsonl</i> which consists of 2,805 training examples for which the two annotators agree
The <i>train_dis.jsonl</i> which consists of 1,015 training examples for which the two annotators disagree
The <i>train.jsonl</i> which consists of 3,820 training examples. This dataset is the union of the <i>train_agr.jsonl</i> and <i>train_dis.jsonl</i> datasets
The <i>dev.jsonl</i> which consists of 500 training examples


Both <i>train\_agr.jsonl</i> and <i>dev.jsonl</i> contain the same examples of the training and development set of Subtask 1. 
