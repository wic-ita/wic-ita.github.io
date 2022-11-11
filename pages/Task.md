---
layout: page
title: Tasks
permalink: /task/
order: 2
feature-img: "assets/img/pexels-pixabay-373543.jpg"
---

<p align="justify">
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


<h2>Evaluation</h2>
We will provide rankings for each sub-task and test set: 
<ul>
<li> Sub-task 1 Monolingual</li>
<li> Sub-task 1 Cross-lingual</li>
<li> Sub-task 2 Monolingual</li>
<li> Sub-task 2 Cross-lingual</li>
</ul>

<h3> Sub-task 1: Binary Classification </h3>
Systems' predictions will be evaluated against the gold truth using the F1-Score.

<h3> Sub-task 1: Binary Classification </h3>
Systems' predictions will be evaluated against the gold truth using Spearman Correlation.

<h3> Baselines </h3>
<p align="justify">
For the Sub-task 2 we provide the same baseline proposed by Raganato et al. (2020) (<i>Baseline 2</i>). The baseline exploits models based on the BERT architecture (Devlin et al., 2019) for encoding the target sub-words. The encoded representations are concatenated and fed into a logistic classifier. In cases where the target word is split into multiple sub-tokens, the first sub-token is considered. 
We set the learning rate to 1e-5 and weight decay to 0. The best checkpoint over the ten epochs is selected using the development data.
Differently from Raganato et al. (2020), we train the baseline to minimise the difference between the model prediction and the gold score computing the mean squared error. We use as pre-trained model XLM-RoBERTa (Conneau et al., 2020).
<br>
The binary baseline (<i>Baseline 1</i>) for Sub-task 1, applies the threshold &delta; = 2. to the predictions of the <i>Baseline 1</i> to obtain discrete labels.
</p>

<h2> References </h2>
<p>
Alessandro Raganato, Tommaso Pasini, Jose Camacho-Collados, and Mohammad Taher Pilehvar. 2020. XL-WiC: A Multilingual Benchmark for Evaluating Semantic Contextualization. In Bonnie Webber, Trevor Cohn, Yulan He, and Yang Liu, editors, Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing, EMNLP 2020, Online, November 16-20, 2020, pages 7193–7206. Association for Computational Linguistics.
</p>

<p>
Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2019. BERT: Pre-training of deep bidirectional transformers for language understanding. In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), pages 4171–4186, Minneapolis, Minnesota, June. Association for Computational Linguistics.
</p>

<p>
Alexis Conneau, Kartikay Khandelwal, Naman Goyal, Vishrav Chaudhary, Guillaume Wenzek, Francisco Guzman, Edouard Grave, Myle Ott, Luke Zettlemoyer, and Veselin Stoyanov. 2020. Unsupervised Cross-lingual Representation Learning at Scale. In Dan Jurafsky, Joyce Chai, Natalie Schluter, and Joel R. Tetreault, editors, Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics, ACL 2020, Online, July 5-10, 2020, pages 8440–8451. Association for Computational Linguistics.
</p>

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
