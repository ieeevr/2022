---
layout: ieeevr-default
title: "Program Overview"
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
        background-color: #f3f3f3;
    }

    .styled-table tbody tr:last-of-type {
        border-bottom: 2px solid #fec10d;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #fec10d;
    }


    /*************************
 * GRID SCHEDULE LAYOUT from there: https://css-tricks.com/building-a-conference-schedule-with-css-grid/
 *************************/
    @media screen and (min-width:700px) {
        .schedule {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0730] 0.5fr [time-0800] 0.5fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;
            /* Note 1:
      Use 24hr time for gridline names for simplicity

      Note 2: Use "auto" instead of "0.5fr" for a more compact schedule where height of a slot is not proportional to the session length. Implementing a "compact" shortcode attribute might make sense for this!
      Try 0.5fr for more compact equal rows. I don't quite understand how that works :)
      */

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end];
        }

        .schedule-with-expo {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end];
        }

        .schedule-sat-12 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0800] 0.5fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end track-5-start] 0.5fr [track-5-end track-6-start] 0.5fr [track-6-end];
        }

        .schedule-sun-13 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0800] 0.5fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end track-5-start] 0.5fr [track-5-end track-6-start] 0.5fr [track-6-end];
        }

        .schedule-mon-14 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end track-5-start] 0.5fr [track-5-end track-6-start] 0.5fr [track-6-end];
        }

        .schedule-tue-15 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0700] 0.5fr [time-0730] 0.5fr [time-0800] 0.5fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end track-5-start] 0.5fr [track-5-end track-6-start] 0.5fr [track-6-end];
        }

        .schedule-wed-16 {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0700] 0.5fr [time-0730] 0.5fr [time-0800] 0.5fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end track-4-start] 0.5fr [track-4-end track-5-start] 0.5fr [track-5-end track-6-start] 0.5fr [track-6-end];
        }
    }

    .time-slot {
        grid-column: times;
        text-decoration: none;

    }

    .track-slot {
        display: none;
        /* hidden on small screens and browsers without grid support */
    }

    @supports(display:grid) {
        @media screen and (min-width:700px) {
            .track-slot {
                display: block;
                padding: 10px 5px 5px;
                position: sticky;
                top: 0;
                z-index: 1000;
                background-color: rgba(255, 255, 255, .9);
            }
        }
    }

    /* Small-screen & fallback styles */
    .session {
        margin-bottom: 1em;
    }

    @supports(display:grid) {
        @media screen and (min-width: 700px) {
            .session {
                margin: 0;
            }
        }
    }

    /*************************
 * VISUAL STYLES
 * Design-y stuff ot particularly important to the demo
 ************************
    body {
        padding: 50px;
        max-width: 1100px;
        margin: 0 auto;
        line-height: 1.5;
    }
    */

    .session {
        padding: .5em;
        border-radius: 5px;
        font-size: 12px;
        box-shadow:
            rgba(255, 255, 255, .6) 1px 1px 0,
            rgba(0, 0, 0, .3) 4px 4px 0;
    }

    .session-title,
    .session-time,
    .session-track,
    .session-presenter {
        display: block;
    }

    .session-title,
    .time-slot {
        margin: 0;
        font-size: 1em;
    }

    .session-title a {
        color: #fff;
        text-decoration-style: dotted;

        &:hover {
            font-style: italic;
        }

        &:focus {
            outline: 2px dotted rgba(255, 255, 255, .8);
        }
    }

    .track-slot,
    .time-slot {
        font-weight: bold;
        font-size: .8em;
    }

    .track-1 {
        background-color: #1259B2;
        color: #fff;
    }

    .track-2 {
        background-color: #687f00;
        color: #fff;
    }

    .track-3 {
        background-color: #544D69;
        color: #fff;
    }

    .track-4 {
        background-color: #c35500;
        color: #fff;
    }

    .track-all {
        display: flex;
        justify-content: center;
        align-items: center;
        background: #ccc;
        color: #000;
        box-shadow: none;
    }

    .track-tutorial {
        background-color: #00aeef;
        color: #fff;
    }

    .track-break {
        background-color: #ddf6ff;
        color: #464646;
    }

    .track-workshop {
        background-color: rgb(52, 199, 89);
        color: #fff;
    }

    .track-dc {
        background-color: rgb(255, 149, 0);
        color: #fff;
    }

    .track-exhibition {
        background-color: rgb(175, 82, 222);
        color: #fff;
    }

    .track-event {
        background-color: rgb(90, 200, 250);
        color: #fff;
    }

    .track-panel {
        background-color: rgb(0, 122, 255);
        color: #fff;
    }

    .track-keynote {
        background-color: rgb(255, 45, 85);
        color: #fff;
    }

    .track-3dui {
        /* background-color: rgb(88, 86, 214); */
        background-color: rgb(211, 15, 69);
        color: #fff;
    }

    .text {
        max-width: 750px;
        font-size: 18px;
        margin: 0 auto 50px;
    }

    .meta {
        color: #555;
        font-style: italic;
    }

    .meta a {
        color: #555;
    }

    hr {
        margin: 40px 0;
    }


    /* Collapsible */
    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1.2rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 1rem;
        text-align: left;
        padding: 0.5rem;
        color: #ffffff;
        background: #fec10d;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        color: #FFF;
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
        border-bottom: 1px solid rgba(254, 193, 13, .45);
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }

</style>


<h1>Program Overview</h1>



<div style="text-align:center;">
        <small><span style="color:gray;">Conference local time</span></small>
        <iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=en&size=small&timezone=Pacific%2FAuckland" width="100%" height="100" frameborder="0" seamless></iframe>
</div>



<!--
<h3 style="color: rgb(255, 45, 85);">Please note that all times are given in Lisbon, Portugal local time.</h3>
<p>
    On the first day (Saturday, March 27), times are given in WET/UTC.
    The rest of the conference is affected by Daylight Saving Time (DST), and therefore, times are shown in WEST/UTC+1.
</p>
-->
<div class="notice--warning">
    <strong style="color: rgb(255, 45, 85);">All times are given in New Zealand local time (UTC +13). Please note that these times are subject to change.
    More details will be made available closer to the conference date.</strong>
</div>
<!--<div class="notice--info" style="background-color: $theme-yellow ! important; color: $theme-text ! important;">
    <strong>Locations</strong>
    <p>
        Locations in the program below refer to virtual places in the Virbela platform.
    </p>
    <center>
        <p style="font-size: 20px;">
            <a href="/2021/attend/virbela-instructions/" class="btn btn--primary" style="color: white;">Getting Started with Virbela</a>
        </p>
    </center>
</div>-->
<!--
<div class="notice--warning">
    <strong>Note:</strong>
    <p>
        The indications for locations in this program refer to virtual locations in the Virbela platform. Please find more information about and how to use Virbela <a href="/2021/attend/virbela-instructions/">here</a>.
    </p>
</div>
-->


<!-- ################################# SATURDAY ########################################### -->
<div>
    <div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible1" class="lbl-toggle">Saturday, March 12<sup>th</sup></label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>NZ Daylight Savings Time, UTC+13</strong></center>
                <div class="schedule-sat-12" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>

                    <div class="session session-1 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-0800 / time-0930;">
                        <h3 class="session-title"><!--<a href="{{ "/program/tutorials/#T4" | relative_url }}">-->Tutorial: Remote Collaboration using Augmented Reality: Development and Evaluation - Bernado Marques et al.<!--</a>--></h3>
                        <span class="session-time">8:00 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <div class="session session-2 track-workshop" style="grid-column: track-2-start / track-2-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#ARES" | relative_url }}">Workshop: ARES - Augmented Reality Enabling Superhuman Sports + Serious Games</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>
                    
                    <div class="session session-3 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#SIVA" | relative_url }}">1<sup>st</sup> International Workshop on Socially Intelligent Virtual Agents (SIVA)</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                    </div>
                    <div class="session session-4 track-workshop" style="grid-column: track-4-start / track-4-end; grid-row: time-0800 / time-1130;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#ReDigiTS" | relative_url }}">3D Reconstruction, Digital Twinning, and Simulation for Virtual Experiences (ReDigiTS)</a></h3>
                        <span class="session-time">8:00 - 11:30</span>
                    </div>
                    
                    <div class="session session-5 track-workshop" style="grid-column: track-5-start / track-5-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><!--<a href="/2021/program/tutorials/#T1">-->Tutorial: Web-Based VR Development and Instruction using Babylon.js<!--</a>--></h3>
                        <span class="session-time">8:00 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0830;"></p>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-6 track-dc" style="grid-column: track-6-start / track-6-end; grid-row: time-0900 / time-1800;">
                        <h3 class="session-title"><!--<a href="/2021/contribute/workshoppapers/#NIDIT">-->Doctoral Consortium<!--</a>--></h3>
                        <span class="session-time">9:00 - 18:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>
                    
                    <p class="time-slot" style="grid-row: time-0930;"></p>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>

                    <div class="session session-7 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-1000 / time-1130;">
                        <h3 class="session-title"><!--<a href="/2021/contribute/workshoppapers/#DISCE">-->Tutorial: Developing Situated Analytics Applications with RagRug - Dieter Schmalstieg, Philipp Fleck<!--</a>--></h3>
                        <span class="session-time">10:00 - 11:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;"></p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-8 track-workshop" style="grid-column: track-2-start / track-2-end; grid-row: time-1100 / time-1600;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#EmpathicComputing" | relative_url }}">Workshop: Empathic Computing</a></h3>
                        <span class="session-time">11:00 - 16:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-8 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-1100 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#OpenVR" | relative_url }}">Workshop: Open Access Tools and Libraries for Virtual Reality</a></h3>
                        <span class="session-time">11:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-9 track-workshop" style="grid-column: track-5-start / track-5-end; grid-row: time-1100 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#XRIOS" | relative_url }}">1<sup>st</sup> International Workshop on eXtended Reality for Industrial and Occupational Supports (XRIOS)</a></h3>
                        <span class="session-time">11:00 - 15:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;"></p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-10 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title"><!--<a href="/2021/contribute/workshoppapers/#DISCE">-->Tutorial: Empathy-Enabled Extended Reality - Denis Gra&#x10D;anin<!--</a>--></h3>
                        <span class="session-time">12:00 - 13:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1230;"></p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-11 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#Data4XR" | relative_url }}">Workshop: Data4XR: Datasets for Developing Intelligent XR Applications</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1330;"></p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <p class="time-slot" style="grid-row: time-1430;"></p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <p class="time-slot" style="grid-row: time-1530;"></p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <p class="time-slot" style="grid-row: time-1630;"></p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <p class="time-slot" style="grid-row: time-1730;"></p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>

                </div>

            </div>
        </div>
    </div>
</div>

<!-- ################################# SUNDAY ########################################### -->
<div>
    <div class="wrap-collabsible"> <input id="collapsible2" class="toggle" type="checkbox" checked> <label for="collapsible2" class="lbl-toggle">Sunday, March 13<sup>th</sup></label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>NZ Daylight Savings Time, UTC+13</strong></center>
                <div class="schedule-sun-13" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>

                    <div class="session session-1 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-0800 / time-0930;">
                        <h3 class="session-title"><!--<a href="{{ "/program/tutorials/#T4" | relative_url }}">-->Tutorial: Build Your Own Social Virtual Reality with Ubiq - Part 1 - Anthony Steed et al.<!--</a>--></h3>
                        <span class="session-time">8:00 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <div class="session session-2 track-workshop" style="grid-column: track-2-start / track-2-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#VHCIE" | relative_url }}">Workshop on Virtual Humans and Crowds in Immersive Environments (VHCIE)</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>
                    
                    <div class="session session-3 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#TrainingXR" | relative_url }}">3<sup>rd</sup> Annual Workshop on 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR)</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                    </div>
                    <div class="session session-4 track-workshop" style="grid-column: track-4-start / track-4-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#SIWI" | relative_url }}">-->Workshop: Metaverse as a promise of a bright future? - social interactions in a world of isolation</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                    </div>
                    
                    <div class="session session-5 track-workshop" style="grid-column: track-5-start / track-5-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#ANIVAE-2022" | relative_url }}">5<sup>th</sup> IEEE VR Internal Workshop on Animation in Virtual and Augmented Environments (ANIVAE-2022)</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <div class="session session-6 track-workshop" style="grid-column: track-6-start / track-6-end; grid-row: time-0800 / time-1100;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#XRHealth" | relative_url }}">Workshop: XR for Health and Wellbeing</a></h3>
                        <span class="session-time">8:00 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0830;"></p>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <p class="time-slot" style="grid-row: time-0930;"></p>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>

                    <div class="session session-7 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-1000 / time-1130;">
                        <h3 class="session-title"><!--<a href="/2021/contribute/workshoppapers/#DISCE">-->Tutorial: Build Your Own Social Virtual Reality with Ubiq - Part 2 - Anthony Steed et al.<!--</a>--></h3>
                        <span class="session-time">10:00 - 11:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;"></p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-8 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-1100 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#PERCxR" | relative_url }}">8<sup>th</sup> workshop on Perceptual and Cognitive Issues in XR (PERCxR)</a></h3>
                        <span class="session-time">11:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-8 track-workshop" style="grid-column: track-4-start / track-4-end; grid-row: time-1100 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#NIDIT" | relative_url }}">Workshop on Novel Input Devices and Interaction Techniques (NIDIT)</a></h3>
                        <span class="session-time">11:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-9 track-workshop" style="grid-column: track-5-start / track-5-end; grid-row: time-1100 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#WEVR" | relative_url }}">8<sup>th</sup> Workshop on Everyday Virtual Reality</a></h3>
                        <span class="session-time">11:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-10 track-workshop" style="grid-column: track-6-start / track-6-end; grid-row: time-1100 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#HSVRAR" | relative_url }}">Health and Safety in VR and AR</a></h3>
                        <span class="session-time">11:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;"></p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-11 track-tutorial" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#DISCE" | relative_url }}">-->Tutorial: Emotion in Virtual Reality - Darlene Barker<!--</a>--></h3>
                        <span class="session-time">12:00 - 13:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1230;"></p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <p class="time-slot" style="grid-row: time-1330;"></p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-12 track-workshop" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#KELVAR" | relative_url }}">7<sup>th</sup> Annual Workshop on K-12+ Embodied Learning through Virtual and Augmented Reality (KELVAR)</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-13 track-workshop" style="grid-column: track-4-start / track-4-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#METABUILD" | relative_url }}">METABUILD: First Workshop for Building the Foundations of the Metaverse</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <div class="session session-14 track-workshop" style="grid-column: track-5-start / track-5-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/contribute/workshoppapers/#X-IRL" | relative_url }}">Workshop: X-IRL risks: Identifying privacy and security risks in inter-reality attacks and interactions</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1430;"></p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <p class="time-slot" style="grid-row: time-1530;"></p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <p class="time-slot" style="grid-row: time-1630;"></p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                </div>

            </div>
        </div>
    </div>
</div>

<!-- ################################# MONDAY ########################################### -->
<div>
    <div class="wrap-collabsible"> <input id="collapsible3" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Monday, March 14<sup>th</sup></label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>NZ Daylight Savings Time, UTC+13</strong></center>
                <div class="schedule-mon-14" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-1 track-tutorial" style="grid-column: track-1-start / track-6-end; grid-row: time-0900 / time-1030;">
                        <h3 class="session-title"><!--<a href="{{ "/program/tutorials/#T4" | relative_url }}">-->Opening incl. VGTC Awards<!--</a>--></h3>
                        <span class="session-time">9:00 - 10:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;"></p>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>

                    <div class="session session-2 track-keynote" style="grid-column: track-1-start / track-6-end; grid-row: time-1030 / time-1130;">
                        <h3 class="session-title"><a href="{{ "/program/keynote-speakers/#keynote-dwyer" | relative_url }}">Keynote 1 - Tim Dwyer</a></h3>
                        <span class="session-time">10:30 - 11:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;"></p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-3 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1130 / time-1200;">
                        <h3 class="session-title">Break</h3>
                        <span class="session-time">11:30 - 12:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;"></p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    
                    <div class="session session-4 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.1" | relative_url }}">Papers: Displays</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <div class="session session-5 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.1" | relative_url }}">Papers: Security</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <div class="session session-6 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.1" | relative_url }}">Papers: Emotion and Cognition</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1230;"></p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-7 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Lunch</h3>
                        <span class="session-time">13:00 - 14:00</span>
                    </div>

                    <div class="session session-8 track-4" style="grid-column: track-5-start / track-6-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><!--<a href="/2021/program/doctoral-consortium/">-->Posters and Demos - Session 1 Fast Forward<!--</a>--></h3>
                        <span class="session-time">13:00 - 14:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1330;"></p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-9 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.2" | relative_url }}">Papers: 3DUI</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <div class="session session-10 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.2" | relative_url }}">Papers: Locomotion (Americas)</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <div class="session session-11 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.2" | relative_url }}">Papers: Immersive Visualization and Virtual Production</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1430;"></p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>

                    <div class="session session-12 track-4" style="grid-column: track-1-start / track-2-end; grid-row: time-1500 / time-1630;">
                        <h3 class="session-title"><!--<a href="/2021/program/doctoral-consortium/">-->Posters and Demos - Session 1<!--</a>--></h3>
                        <span class="session-time">15:00 - 16:30</span>
                    </div>

                    <div class="session session-13 track-exhibit" style="grid-column: track-3-start / track-4-end; grid-row: time-1500 / time-1630;">
                        <h3 class="session-title"><!--<a href="/2021/program/doctoral-consortium/">-->Industry Exhibition<!--</a>--></h3>
                        <span class="session-time">15:00 - 16:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;"></p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>

                    <div class="session session-15 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.3" | relative_url }}">Papers: Multimodal VR</a></h3>
                        <span class="session-time">16:30 - 17:30</span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;"></p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                    <div class="session session-17 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1730 / time-1800;">
                        <h3 class="session-title">Break</h3>
                        <span class="session-time">17:30 - 18:00</span>
                    </div>
                    
                    <p class="time-slot" style="grid-row: time-1730;"></p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>

                    <div class="session session-18 track-event" style="grid-column: track-1-start / track-6-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title">Speed Dating in Virbela</h3>
                        <span class="session-time">18:30 - 19:00</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- ################################# TUESDAY ########################################### -->
<div>
    <div class="wrap-collabsible"> <input id="collapsible4" class="toggle" type="checkbox" checked> <label for="collapsible4" class="lbl-toggle">Tuesday, March 15<sup>th</sup></label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>NZ Daylight Savings Time, UTC+13</strong></center>
                <div class="schedule-tue-15" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0700;">7:00</p>

                    <div class="session session-1 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-0730 / time-0830;">
                        <h3 class="session-title"><!--<a href="{{ "/program/tutorials/#T4" | relative_url }}">-->Posters and Demos - Session 2 Fast Forward<!--</a>--></h3>
                        <span class="session-time">7:30 - 8:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0730;"></p>
                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>

                    <div class="session session-2 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.3" | relative_url }}">Papers: Embodiment</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-3 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.4" | relative_url }}">Papers: Presence</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-4 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.3" | relative_url }}">Papers: Interaction Design</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0830;"></p>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-5 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Posters and Demos - Session 2<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-6 track-event" style="grid-column: track-3-start / track-4-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Panel 1 - Planning a Virtual Experience Research Accelerator (VERA)<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-7 track-event" style="grid-column: track-5-start / track-6-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Recruitment Fair<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;"></p>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <p class="time-slot" style="grid-row: time-1030;"></p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-8 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.4" | relative_url }}">Papers: Collaboration</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-9 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.5" | relative_url }}">Papers: Perception in AR</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-10 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.4" | relative_url }}">Papers: Virtual Humans and Agents</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;"></p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-11 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Lunch</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1230;"></p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-12 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.5" | relative_url }}">Papers: Augmented Reality</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-13 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.6" | relative_url }}">Papers: Locomotion (Asia-Pacific)</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-14 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.5" | relative_url }}">Papers: Perception</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1330;"></p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-15 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1400 / time-1430;">
                        <h3 class="session-title">Break</h3>
                        <span class="session-time">14:00 - 14:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-16 track-keynote" style="grid-column: track-1-start / track-6-end; grid-row: time-1430 / time-1530;">
                        <h3 class="session-title"><a href="{{ "/program/keynote-speakers/#keynote-staples" | relative_url }}">Keynote 2 - Aliesha Staples</a></h3>
                        <span class="session-time">14:30 - 15:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1430;"></p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>

                    <div class="session session-17 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1530 / time-1600;">
                        <h3 class="session-title">Break</h3>
                        <span class="session-time">15:30 - 16:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;"></p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>

                    <div class="session session-18 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.6" | relative_url }}">Papers: Machine Learning</a></h3>
                        <span class="session-time">18:00 - 19:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-19 track-exhibition" style="grid-column: track-3-start / track-4-end; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Industry Exhibition<!--</a>--></h3>
                        <span class="session-time">16:00 - 17:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-20 track-3" style="grid-column: track-3-start / track-4-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.8" | relative_url }}">Papers: Negative Effects</a></h3>
                        <span class="session-time">18:00 - 19:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-21 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.6" | relative_url }}">Papers: Medical and Health Care</a></h3>
                        <span class="session-time">18:00 - 19:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;"></p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <p class="time-slot" style="grid-row: time-1730;"></p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <p class="time-slot" style="grid-row: time-1830;"></p>
                    <p class="time-slot" style="grid-row: time-1900;">19:00</p>
                    
                </div>
            </div>
        </div>
    </div>
</div>

<!-- ################################# WEDNESDAY ########################################### -->
<div>
    <div class="wrap-collabsible"> <input id="collapsible5" class="toggle" type="checkbox" checked> <label for="collapsible5" class="lbl-toggle">Wednesday, March 16<sup>th</sup></label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>NZ Daylight Savings Time, UTC+13</strong></center>
                <div class="schedule-wed-16" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0700;">7:00</p>
                    <p class="time-slot" style="grid-row: time-0730;"></p>

                    <div class="session session-1 track-3dui" style="grid-column: track-5-start / track-6-end; grid-row: time-0730 / time-0830;">
                        <h3 class="session-title"><!--<a href="{{ "/program/tutorials/#T4" | relative_url }}">-->3DUI Contest Fast Forward<!--</a>--></h3>
                        <span class="session-time">7:30 - 8:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>

                    <div class="session session-2 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.7" | relative_url }}">Papers: Audio in VR</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-3 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.7" | relative_url }}">Papers: Haptics</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-4 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#3.7" | relative_url }}">Papers: Locomotion (Europe)</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-830;"></p>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>

                    <div class="session session-5 track-3dui" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->3DUI Contest<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-6 track-event" style="grid-column: track-3-start / track-4-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Panel 2 - Future Visions for IEEE VR<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-7 track-event" style="grid-column: track-5-start / track-6-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Sponsor Talks<!--</a>--></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-0730;"></p>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <p class="time-slot" style="grid-row: time-1030;"></p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-8 track-keynote" style="grid-column: track-1-start / track-6-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="{{ "/program/keynote-speakers/#keynote-debevec" | relative_url }}">Keynote 3 - Paul Debevec</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;"></p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-9 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Lunch</h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-10 track-3" style="grid-column: track-5-start / track-6-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Posters and Demos - Session 3 Fast Forward<!--</a>--></h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1230;"></p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-12 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.8" | relative_url }}">Papers: Rendering</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-13 track-2" style="grid-column: track-3-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#2.8" | relative_url }}">Papers: Computer Vision</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1330;"></p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-15 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="{{ "/program/papers/#1.9" | relative_url }}">Papers: Advanced UI</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1430;"></p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>

                    <div class="session session-18 track-break" style="grid-column: track-1-start / track-6-end; grid-row: time-1500 / time-1530;">
                        <h3 class="session-title">Break</h3>
                        <span class="session-time">15:00 - 15:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;"></p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>

                    <div class="session session-19 track-1" style="grid-column: track-1-start / track-2-end; grid-row: time-1530 / time-1700;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Posters and Demos - Session 3<!--</a>--></h3>
                        <span class="session-time">15:30 - 17:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <div class="session session-20 track-exhibition" style="grid-column: track-3-start / track-4-end; grid-row: time-1530 / time-1700;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Industry Exhibition<!--</a>--></h3>
                        <span class="session-time">15:30 - 17:00</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;"></p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                    <div class="session session-21 track-tutorial" style="grid-column: track-1-start / track-6-end; grid-row: time-1700 / time-1830;">
                        <h3 class="session-title"><!--<a href="{{ "/contribute/workshoppapers/#SIVE" | relative_url }}">-->Conference Closing<!--</a>--></h3>
                        <span class="session-time">17:00 - 18:30</span>
                        <!--<span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>-->
                    </div>

                    <p class="time-slot" style="grid-row: time-1730;"></p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <p class="time-slot" style="grid-row: time-1830;"></p>
                    <p class="time-slot" style="grid-row: time-1900;">19:00</p>
                    
                </div>
            </div>
        </div>
    </div>
</div>


