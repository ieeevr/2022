---
layout: ieeevr-default
title: "Reviewers"
subtitle: "IEEE VR 2022"
title_separator: "|"
---

<style>
	.styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.9em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        /*box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);*/
        display: table;
		border:none;
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
</style>


<div>

    <h2> IEEE VR 2022 Reviewers for Journal Papers </h2>
    <table class="styled-table" style="font-size: 0.8em; ">
        {% tablerow reviewer in site.data.journalreviewers cols:3 %}
            {{ reviewer.name }}{%if reviewer.affiliation %} - <i>{{ reviewer.affiliation }}</i>{% endif %}
        {% endtablerow %}
    </table>


    <h2> IEEE VR 2022 Reviewers for Conference Papers </h2>
	<table class="styled-table" style="font-size: 0.8em; ">
        {% tablerow reviewer in site.data.conferencereviewers cols:3 %}
            {{ reviewer.name }}{%if reviewer.affiliation %} - <i>{{ reviewer.affiliation }}</i>{% endif %}
        {% endtablerow %}
    </table>
</div>
