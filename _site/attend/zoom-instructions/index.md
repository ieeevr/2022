---
layout: ieeevr-default
title: "Zoom Instructions"
subtitle: "IEEE VR 2022"
title_separator: "|"
---

<style>
    <style>* {
        box-sizing: border-box;
    }

    .exhibitors-center {
        margin: auto;
        width: 90%;
    }

    .exhibitors-row {
        display: flex;
        background-color: #00aeef;
        border-radius: 10px;
        padding: 10px;
    }

    .exhibitors-column {
        flex: 50%;
        padding: 20px;
        position: relative;
    }

    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
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
        width: 50%;
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
        color: #00aeef;
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
        padding: 0.1rem;
        color: #00aeef;
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
        border-bottom: 1px solid rgba(0, 105, 255, .45);
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
        background-color: #00aeef;
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
        background-color: #fffbed;
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
    
    div {
        text-align: justify;
        text-justify: inter-word;
        }

</style>


<div>
    <h1>Zoom Events Instructions</h1>

    <div>
        <br>
        <div style="">
        <center>
            <p style="font-size: 20px;">
                <a href="https://events.zoom.us/ev/AMhPE42qSa3t0DDhNEdVpwntLRhotRRpkXfFrCuFaDN7WNQXQHbMvw2fnfGgpsnKf27gWYU" class="btn btn--primary" style="" download>Click here to join the Zoom event</a>
            </p>
        </center>
    </div>

    <p>
        Dear IEEEVR 2022 attendee,
    </p>
    <p>
        This year, workshops, tutorials, paper presentations, and the opening and closing ceremonies will be presented via a Zoom event. Below is a quick guide to
        help you navigate the Zoom Events interface.
    </p>

    <div>

        <h2>Joining the Zoom Event</h2>

        <p>
            All sessions will be accessed through the Zoom Events hub, joinable via the link above. <strong>If you are registered as a speaker or panelist for conference 
            you should have also received an email invitation; please ensure that you accept this invitation prior to accessing the Zoom hub.</strong>
        </p>

        <p>
            After clicking the above link, you will be brought to a webpage similar to the one below:
        </p>

        <!--    image here -->
        <img src="{{ "/assets/zoom/events-web-interface.jpg" | relative_url }}" alt="A screenshot of the Zoom Events web interface. The conference logo is displayed on the left, with a large button labeled Join Lobby on the right">

        <p>
            Click &quot;Join Lobby&quot; to bring up the main interface. <strong>Important: If you are asked to log in to Zoom, ensure you use the same email address
            as was used to register for the conference.</strong>
        </p>

    </div>

    <div>

        <h2>Joining a Session</h2>

        <p>You should now be in the IEEE VR Zoom hub! This is your gateway to all of the sessions available in this year's conference. The hub will look similar to the image below:</p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/events-lobby.jpg"" | relative_url }}" alt="The Zoom Event lobby for IEEE VR 22">
        <br>

        <p>
            There are several main components you should be aware of. This area shows all of the sessions currently in progress:
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/events-lobby-sessions.jpg" | relative_url }}" alt="The lobby with the active session area circled">
        <br>

        <p>
            By clicking the &quot;Play&quot; button in the lower right corner of this area you can watch sessions straight from the hub. If multiple sessions are running concurrently they will 
            be shown as a thumbnail on the right hand side&#59; simply click on each to cycle between active sessions.
        </p>
        <p>
            All current and upcoming sessions are also shown in the lower area of this screen. To join a session, simply click the appropriate &quot;Join&quot; button. Please note that you will be unable 
            to join a session until it is started by the session chair or you are a speaker for that session. <strong>If you cannot access a session you are meant to be speaking in, please get in contact 
            with the streaming chairs via Discord.</strong>
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/events-lobby-upcoming.jpg" | relative_url }}" alt="The lobby with the active session area circled">
        <br>
    </div>

    <div>
        <h2>Questions and Answers</h2>

        <p>
            In each session, speakers will speak concurrently with no time for questions in between. Instead, there will be a dedicated 15 minutes at the end of each session for questions.
        </p>
        <p>
            While viewing a session you may notice that the chat and Q&amp;A functions are disabled. Instead, <strong>all questions must be submitted via the appropriate Discord channel.</strong> 
            This is so that attendees watching via Zoom and Virbela have equal opportunity to ask the speakers questions.
        </p>
        <p>
            You can find links to each session's Discord channel in the conference program: <a href="https://ieeevr.org/2022/program/overview/" target="_blank">https://ieeevr.org/2022/program/overview/</a> 
            If a link to the channel is not yet available, you can join the official Discord from the following link: <a href="https://discord.gg/STCgpaWg" target="_blank">https://discord.gg/STCgpaWg</a>
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/discord-question-example.jpg" | relative_url }}" alt="An example of someone asking a question in Discord.">
    </div>

    <div>
        <h2>Viewing Session Information</h2>

        <p>
            To see all past, present, and future sessions, click the &quot;Sessions&quot; button on the left hand side of the event hub:
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/events-lobby-sessions-tab.jpg" | relative_url }}" alt="The lobby with the session button, which is halfway down the leftmost edge, circled.">
        <br>

        <p>
            This will bring you to a page with every session being presented via Zoom this year.
        </p>
        <p>
            Each session is presented as a card. By clicking on this, you can bring up information about that session depending on what type of session it is and who is scheduled to speak in it. Each 
            card will also notify you of any special roles you have in that session, such as if you are scheduled to speak in it. <strong>If you are registered as a speaker or host for any session in which 
            you shouldn't be, please get in touch with the Streaming Chairs via Discord.</strong>
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/example-session-info.jpg" | relative_url }}" alt="An example session with its information displayed. In this case it is the first keynote abstract.">
        <br>
    </div>

    <div>
        <h2>Customising your IEEE VR Experience</h2>

        <p>
            If you find a session you are interested in, you can bookmark it by clicking the flag icon in the lower left corner of its session card. If it's yellow, you've bookmarked it. 
            Any session in which you are registered as a speaker or host will be automatically bookmarked. You can also see how many other attendees have bookmarked this session.
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/session-bookmark-example.jpg" | relative_url }}" alt="A session card with the bookmark button in the lower left corner circled.">
        <br>

        <p>
            Clicking on the &quot;Itinerary&quot; tab on the left hand side of the window will then bring up a personalised timetable with all sessions you have bookmarked. Please feel free to 
            use this feature to plan your IEEE VR experience for 2022.
        </p>
        <!--    image here -->
        <img src="{{ "/assets/zoom/events-itinerary.jpg" | relative_url }}" alt="The itinerary window showing a personalised conference schedule. The Itinerary button halfway down the left edge of the window is also circled.">
        <br>
    </div>

    <div>
        <h2>Need additional help?</h2>

        <p>
            If you need additional help navigating the Zoom interface, or think that your registration has been configured incorrectly, please get in touch with the help desk on Discord 
            (<a href="https://discord.com/channels/842181663248482334/950905251962167356" target="_blank">link</a>) or email the Streaming Chairs: streaming2022 [at] ieeevr.org
        </p>
    </div>

</div>
