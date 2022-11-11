---
layout: page
title: Data
permalink: /data/
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
