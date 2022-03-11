---
layout: ieeevr-default
title: "Panels"
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

<h1>Panels</h1>

<div>
    <table class="styled-table" style="font-size: 0.9em; ">
        {% for panel in site.data.panels %}
            <tr>
                <td style="font-size: 0.9em;"><a href="#{{ panel.id }}">{{ panel.title }}</a></td>
                <td style="white-space: nowrap; text-align: right;">{{ panel.day }}, {{ panel.starttime }} - {{ panel.endtime }}</td>
            </tr>
        {% endfor %}
    </table>
</div>


<div>
    {% for panel in site.data.panels %}

        <h2 id="{{ panel.id }}">{{panel.name}}: {{ panel.title }}</h2>
        
        <p><strong>{{ panel.day }}, {{ panel.starttime }} - {{ panel.endtime }}, {{ panel.timezone }}</strong></p>
        
        {% if panel.moderator %}
            <p><small><b style="color: black;">Moderators:</b> <br>{{ panel.moderator }}</small></p>
        {% endif %}

        {% if panel.panelists %}
            <p><small><b style="color: black;">Panelists:</b> <br>{{ panel.panelists }}</small></p>
        {% endif %}

        {% if panel.discordurl %}
            <p><small><b style="color: black;">Discord URL:</b> <a href="{{ panel.discordurl }}" target="_blank">{{ panel.discordurl }}</a></small></p>
        {% endif %}

        {% if panel.abstract %}
            <div id="{{ panel.id }}" class="wrap-collabsible"> <input id="collapsible{{ panel.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ panel.id }}" class="lbl-toggle">Abstract</label>
                <div class="collapsible-content">
                    <div class="content-inner">
                        <p>{{ panel.abstract }}</p>
                    </div>
                </div>
            </div>
        {% endif %}
    
        <!-- TAKE ME TO THE EVENT START -->
        <!--{% for event in site.data.events %}
            {% if event.id == panel.id %}
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

    {% endfor %}
</div>
