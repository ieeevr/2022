---
layout: ieeevr-default
title: "Tutorials"
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

</style>

<h1>Tutorials</h1>

<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Saturday, March 12, NZDT, UTC+13</th>
            <th></th>
        </tr>
        {% for tutorial in site.data.tutorials %}
            {% if tutorial.day == 'Saturday, March 12' %}
                <tr>
                    <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ tutorial.name }}</a></td>
                    <td style="white-space: nowrap; text-align: right;">{{ tutorial.time }}</td>
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>
<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        <tr>
            <th>Sunday, March 13, NZDT, UTC+13</th>
            <th></th>
        </tr>
        {% for tutorial in site.data.tutorials %}
            {% if tutorial.day == 'Sunday, March 13' %}
                <tr>
                    <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ tutorial.name }}</a></td>
                    {% if tutorial.time2 %}
                        <td style="white-space: nowrap; text-align: right;">Part 1: {{ tutorial.time }}<br>Part 2: {{ tutorial.time2 }}</td>
                    {% else %}
                        <td style="white-space: nowrap; text-align: right;">{{ tutorial.time }}</td>
                    {% endif %}
                </tr>
            {% endif %}
        {% endfor %}
    </table>
</div>

{% for day in site.data.workshopdays %}
<div>
    {% for tutorial in site.data.tutorials %}
        {% if tutorial.day == day.day %}

            <h2 id="{{ tutorial.id }}">Tutorial: {{ tutorial.name }}</h2>
    
            {% if tutorial.time2 %}
                <p><strong>
                    Part 1: {{ tutorial.day }}, {{ tutorial.time }}, {{ tutorial.timezone }}<br>
                    Part 2: {{ tutorial.day }}, {{ tutorial.time2 }}, {{ tutorial.timezone }}
                </strong></p>
            {% else %}
                <p><strong>{{ tutorial.day }}, {{ tutorial.time }}, {{ tutorial.timezone }}</strong></p>
            {%endif %}
            {% if tutorial.organiser %}
                <p><small>Organisers: <b style="color: black;">{{ tutorial.organiser }}</b></small></p>
            {% endif %}
            {% if tutorial.discordurl %}
                <p><small><b style="color: black;">Discord URL:</b> <a href="{{ tutorial.discordurl }}" target="_blank">{{ tutorial.discordurl }}</a></small></p>
            {% endif %}

            {% if tutorial.abstract %}
                <div id="{{ tutorial.id }}" class="wrap-collabsible"> <input id="collapsible{{ tutorial.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ tutorial.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ tutorial.abstract }}</p>
                        </div>
                    </div>
                </div>
            {% endif %}
    
            <!-- TAKE ME TO THE EVENT START -->
            <!--{% for event in site.data.events %}
                {% if event.id == tutorial.id %}
                    {% if event.location %}
                    <div class="notice--info" style="background-color: $theme-yellow ! important; color: $theme-text ! important;">
                        <strong style="padding-bottom: 5px;">Take me to the event:</strong>
                        <p>
                            <strong style="color: black;">Virbela Location:</strong> {{ event.location }} (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)

                            {% if event.stream-url %}
                                <br />
                                {% if event.aindanaoaconteceu %}
                                    <strong style="color: black;">Watch video stream live:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
                                {% else %}
                                    <strong style="color: black;">Watch the recorded video stream:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
                                {% endif %}
                            {% endif %}
                            {% if event.discordurl %}
                                <br />
                                <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
                            {% endif %}
                        </p>
                    </div>
                    {% endif %}
                {% endif %}
            {% endfor %}-->
            <!-- TAKE ME TO THE EVENT END-->

        {% endif %}
    {% endfor %}
</div>
{% endfor %}