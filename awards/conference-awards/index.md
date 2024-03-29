---
layout: ieeevr-default
title: "Conference Award Winners"
---

<style>
    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.9em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
    }

    .styled-table thead tr {
        background-color: #fec10d;
        color: #ffffff;
        text-align: left;
    }

    .styled-table th,
    .styled-table td {
        padding: 12px 15px;
    }

    .styled-table tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table tbody tr:nth-of-type(even) {
        background-color: #fffbed;
    }

    .styled-table tbody tr:last-of-type {
        border-bottom: 2px solid #fec10d;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #fec10d;
    }

    /* Collapsible */
    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 0.8rem;
        text-align: left;
        padding: 0rem;
        color: #fec10d;
        background: #ffffff;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        /*color: #FFF;*/
    }

    .lbl-toggle::before {
        content: ' ';
        display: inline-block;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        border-left: 5px solid currentColor;
        vertical-align: middle;
        margin-right: .7rem;
        transform: translateY(-2px);
        transition: transform .2s ease-out;
    }

    .toggle:checked+.lbl-toggle::before {
        transform: rotate(90deg) translateX(-3px);
    }

    .collapsible-content {
        max-height: 0px;
        overflow: hidden;
        transition: max-height .25s ease-in-out;
    }

    .toggle:checked+.lbl-toggle+.collapsible-content {
        max-height: 1500px;
    }

    .toggle:checked+.lbl-toggle {
        border-bottom-right-radius: 0;
        border-bottom-left-radius: 0;
    }

    .collapsible-content .content-inner {
        background: white;
        /* rgba(0, 105, 255, .2);*/
        border-bottom: 1px solid white;
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }



    /* video container */
    .video-container {
        overflow: hidden;
        position: relative;
        width: 100%;
    }

    .video-container::after {
        padding-top: 56.25%;
        /* 75% if 4:3*/
        display: block;
        content: '';
    }

    .video-container iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    /* Thumbnails box */
    .box {
        border-radius: 5px;
        padding: 20px;
    }

    .box:nth-child(even) {
        color: red;
    }

    .wrapper {
        display: grid;
        /* border: 1px solid #000; */
        grid-gap: 10px;
        grid-template-columns: repeat(auto-fill, 150px 30%);
    }

    .styled-table2 {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
        width: 50%;
        margin-left: auto;
        margin-right: auto;


    }

    .styled-table2 thead tr {
        background-color: #fec10d;
        color: #ffffff;
        text-align: left;
    }

    .styled-table2 th,
    .styled-table2 td {
        padding: 12px 15px;
        width: 50%;
    }

    .styled-table2 tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table2 tbody tr:nth-of-type(even) {
        background-color: #f3f3f3;
    }

    .styled-table2 tbody tr:last-of-type {
        border-bottom: 2px solid #fec10d;
    }

    .styled-table2 tbody tr.active-row {
        font-weight: bold;
        color: #fec10d;
    }

    img {
        display: block;
        margin-left: auto;
        margin-right: auto;
    }

    /*
    div {
        text-align: justify;
        text-justify: inter-word;
    }
    */

</style>


<h1>IEEE VR 2022 Conference Awards</h1>

<!--
<p> Awards presented at the annual IEEE VR 2021 are in two categories:</p>
<ul>
    <li>Awards sponsored by the Visualization and Graphics Technical Committee of the IEEE Computer
Society, and</li>
    <li>Awards sponsored by the conference itself.</li>
</ul>
-->
<!--
<p>
    Award winners are selected by various means including people’s choice voting, invited judges, and
formal selection committees.
</p>
-->    

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Journal Papers</th>
    </tr>
    <tr>
        <td><strong><a href="#journal-best">TVCG - Best Journal Papers</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#journal-honorable">TVCG - Honorable Mentions</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#journal-nominees">TVCG - Best Journal - Nominees</a></strong></td>
    </tr>
</table>

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Conference Papers</th>
    </tr>
    <tr>
        <td><strong><a href="#conference-best">Best Conference Papers</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#conference-honorable">Honorable Mentions</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#conference-nominees">Nominees</a></strong></td>
    </tr>
    
</table>

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Posters</th>
    </tr>
    <tr>
        <td><strong><a href="#best-poster">Best Posters</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#poster-honorable">Honorable Mentions</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#poster-nominees">Nominees</a></strong></td>
    </tr>
    
</table>

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Demos</th>
    </tr>
    <tr>
        <td><strong><a href="#demo-best">Best Demo</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#demo-honorable">Honorable Mentions</a></strong></td>
    </tr>
    
</table>

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>3DUI Contest</th>
    </tr>
    <tr>
        <td><strong><a href="#3dui-best">Best 3DUI Contest Entry</a></strong></td>
    </tr>
    <tr>
        <td><strong><a href="#3dui-nominees">Best 3DUI Contest Entry Nominees</a></strong></td>
    </tr>
</table>

<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Doctoral Consortium</th>
    </tr>
    <tr>
        <td><strong><a href="#DC-best">Best Doctoral Consortium Student Award</a></strong></td>
    </tr>
</table>
<!--
<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Best Dissertation</th>
    </tr>
     <tr>
        <td><strong><a href="#best-dissertation">Best Dissertation</a></strong></td>
    </tr>
         <tr>
        <td><strong><a href="#honorable-dissertation">Honorable Mention</a></strong></td>
    </tr>
</table>
-->
<table class="styled-table" style="font-size: 0.9em; ">
    <tr>
        <th>Ready Player 22</th>
    </tr>
     <tr>
        <td><strong><a href="#ready-player-22">Winner</a></strong></td>
    </tr>
</table>


<!-- JOURNAL PAPERS -->
<h2 id='journal-best' style="text-align: center; color: #fec10d;">TVCG - Best Journal Papers</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Best Paper' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='journal-honorable' style="text-align: center; color: #fec10d;">TVCG - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='journal-nominees' style="text-align: center; color: #fec10d;">TVCG - Best Journal Paper Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Journal' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.journalpapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible1{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible1{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>


<!-- CONFERENCE -->
<h2 id='conference-best' style="text-align: center; color: #fec10d;">Best Conference Papers</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Best Paper' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='conference-honorable' style="text-align: center; color: #fec10d;">Conference Papers - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='conference-nominees' style="text-align: center; color: #fec10d;">Conference Papers - Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Conference' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.conferencepapers %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.Title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsibleC{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsibleC{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<!-- POSTER -->
<h2 id='best-poster' style="text-align: center; color: #fec10d;">Best Poster</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Poster' %}
        {% if item.award == 'Best Poster' %}
        
            {% for j in site.data.posters %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='poster-honorable' style="text-align: center; color: #fec10d;">Posters - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Poster' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.posters %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='poster-nominees' style="text-align: center; color: #fec10d;">Best Poster - Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Poster' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.posters %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsibleC{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsibleC{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<!-- DEMO -->
<h2 id='demo-best' style="text-align: center; color: #fec10d;">Best Demo</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Demo' %}
        {% if item.award == 'Best Demo' %}
        
            {% for j in site.data.demos %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='demo-honorable' style="text-align: center; color: #fec10d;">Demos - Honorable Mentions</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == 'Demo' %}
        {% if item.award == 'Honorable Mention' %}
        
            {% for j in site.data.demos %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<!-- 3DUI -->
<h2 id='3dui-best' style="text-align: center; color: #fec10d;">3DUI Contest - Best 3DUI Contest Entry</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == '3DUI Contest' %}
        {% if item.award == 'Best 3DUI' %}
        
            {% for j in site.data.3duicontest %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible3dui{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible3dui{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='3dui-nominees' style="text-align: center; color: #fec10d;">3DUI Contest - Nominees</h2>
<div>
{% for item in site.data.awards %}
    
    {% if item.type == '3DUI Contest' %}
        {% if item.award == 'Nominee' %}
        
            {% for j in site.data.3duicontest %}
                {% if j.id == item.id %}
                <h4 id="{{ j.id }}">{{ j.title }}</h4>
                <p><i>{{ j.authors }}</i></p>
                <div id="{{ j.id }}" class="wrap-collabsible"> <input id="collapsible3dui{{ j.id }}" class="toggle" type="checkbox"> <label for="collapsible3dui{{ j.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ j.abstract }}</p>
                        </div>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
    
        {% endif %}
    {% endif %}
    
{% endfor %}
</div>

<h2 id='DC-best' style="text-align: center; color: #fec10d;">Doctoral Consortium - Best Presentation</h2>
<div>
    <h4>Designing Immersive Tools for Supporting Cognition in Remote Scientific Collaboration</h4>
    <p>
        <strong>Monsurat Olaosebikan</strong><br/>
        <i>Tufts University</i><br/>
    </p>
</div>
<!--
<h2 id='best-dissertation' style="text-align: center; color: #fec10d;">Best Dissertation</h2>
<div>
    <h4>A Framework for Enhancing the Sense of Presence in Virtual and Mixed Reality</h4>
    <p>
        <strong>Misha Sra</strong><br/>
        <i>Massachusets Institute of Technology</i><br/>
        Advisor: <i>Pattie Maes</i>
    </p>
</div>
-->
<!--
<h2 id='honorable-dissertation' style="text-align: center; color: #fec10d;">Best Dissertation - Honorable Mention</h2>
<div>
    <h4>Optimal Spatial Registration of SLAM for Augmented Reality</h4>
    <p>
        <strong>Folker Wientapper</strong><br/>
        <i>Technical University of Darmstadt</i><br/>
        Advisor: <i>Arjan Kuijper</i>
    </p>
</div>
-->

<h2 id='ready-player-22' style="text-align: center; color: #fec10d;">Ready Player 22 - Winner</h2>
<div>
    <h4>Xiaodan Hu</h4>
    <i>Nara Institute of Science and Technology, Ikoma, Japan</i>
</div>