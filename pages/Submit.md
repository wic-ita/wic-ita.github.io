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
                <a class="clear" aria-label="Submit Results" title="Submit Results" href="/submit/">
                     Submit Results 
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



Each participant can submit at utmost <b>three</b> runs. For each run, a short description of the system and the list of data and resources used must be submitted by filling out the form at (You have to log in with a Gmail account):

<center>
    <a>https://forms.gle/2U5sJnpwFJF7F8Pg6</a>
</center>

The form requires to provide the following information:
<ul>
    <li> Name of the team </li>
    <li> Name of the run </li>
    <li> Zipped file containing at least two files (<i>description.txt</i>, <i>binary.jsonl</i> <b>or/and</b> <i>ranking.jsonl</i> <b>or/and</b> <i>binary\_eng.jsonl</i> <b>or/and</b> <i>ranking\_eng.jsonl</i>). The run can refer to only one of the two subtasks. </li>
</ul>

The \textit{binary.jsonl} is a JSON Lines text file containing for each row a Json line with the example ID and the predicted label (as in Listing \ref{lst:ex1}).

The \textit{binary\_eng.jsonl} is a JSON Lines text file containing for each row a JSON with the example ID and the predicted label (as in Listing \ref{lst:ex4}).


The \textit{ranking.jsonl} is a JSON Lines text file containing for each row a JSON with the example ID and the predicted score (as in Listing \ref{lst:ex2}).


The \textit{ranking\_eng.jsonl} is a JSON Lines text file containing for each row a JSON with the example ID and the predicted score (as in Listing \ref{lst:ex3}).


<b>The <i>description.txt</i> file contains information about the submission, such as the model used, the parameters, and other relevant stuff. Please, be sure to properly include in the description all the information necessary to track the submitted system.</b>

An example of submission is available at:
<center>
<a>https://github.com/wic-ita/data/blob/main/xlm_finetuned.zip</a>
<center>

Please, contact us if you experience any issues with the submission at <a>wicita.evalita@gmail.com</a>.
