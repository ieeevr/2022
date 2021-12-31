---
layout: ieeevr-default
title: "Workshop Papers"
subtitle: "IEEE VR 2022"
title_separator: "|"
---

<style>
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
        background-color: #00aeef;
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
    <h1 id="call-for-workshop-papers"> Workshops </h1>
    <p>
        IEEE VR 2022 seeks high-quality contributions to the following 21 workshops. 
        These will be held virtually on March 12<sup>th</sup>-13<sup>th</sup>. For more details, see each workshop's Call for Papers below.
    </p>
    
    <table class="styled-table">

        <tr>
            <th>Workshops</th>
        </tr>
        {% for workshop in site.data.workshops %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ workshop.id }}">{{ workshop.title }}</a></td>
        </tr>
        {% endfor %}
    </table>


<!-- ------------------------------------------------ANIVAE-2022-------------------------------------------------------- -->

    <h2 id="ANIVAE-2022"> 5<sup>th</sup> IEEE VR Internal Workshop on Animation in Virtual and Augmented Environments (ANIVAE-2022) </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE-2022' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://anivae.fhstp.ac.at/" target="_blank"> https://anivae.fhstp.ac.at/ </a>
    </p>
    <ul>
        <li> Submission deadline: 2<sup>nd</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        By encouraging synergies of interdisciplinary approaches, the workshop maps animation within the AVR context from different 
        angles and creates new knowledge in this research field.   
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Thomas Moser
    </p>
    

<!-- ------------------------------------------------OpenVR-------------------------------------------------------- -->

    <h2 id="OpenVR"> Open Access Tools and Libraries for Virtual Reality </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'SeatedVR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://openvrlab.github.io/" target="_blank">https://openvrlab.github.io/</a>
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        Virtual Reality technologies are growing fast, and so is the VR research community. In this scenario, it is more important than ever that 
        academic research builds upon best practices and results to amplify impact in the broader field. Open-Source tools are one means to propagate 
        best practice as they lower the barrier to entry for researchers from an engineering point of view, while also embodying the prior work on 
        which the tools were built. Open access tools are also critical to eliminate redundancies and increase world research collaboration in VR. 
        At a time that academic research is growing it also needs to move as fast as the industry, collaboration and shared tools is the best way to do it.  
        In this workshop, we will gather with creators and users of open-access libraries ranging from avatars (like the Microsoft Rocketbox avatar library) 
        to animation to networking (Ubiq toolkit) to explore how open access tools are helping advance the VR community.
    </p>
    <p>
        We invite all researchers to join this workshop and learn from existing libraries. We also invite submissions on technical and systems papers that 
        describe new libraries and or new features on existing libraries. In this workshop, we will explore these open-access tools, their accessibility, 
        and what type of applications they enable. Finally, we invite users of current libraries to submit their papers and share their learnings while 
        using these tools. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Matias Volonte
    </p>
    

<!-- ------------------------------------------------TrainingXR-------------------------------------------------------- -->

    <h2 id="TrainingXR"> 3rd Annual Workshop on 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'SIVE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/trainingxrieeevr2022" target="_blank">https://sites.google.com/view/trainingxrieeevr2022</a>
    </p>
    <ul>
        <li> Submission deadline: 12<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        This workshop discusses and articulates research visions on using the latest extended reality (VR/AR/MR) technologies for 
        education and training purposes, and on creating immersive 3D virtual content for delivering effective and personalized training 
        experiences. This workshop will gather researchers and practitioners in a variety of computer disciplines related to XR training 
        and content creation. This workshop will accept research papers on these topics. We will also invite renowned speakers from the 
        research community and the industry to give talks related to XR-based training to inspire the field to further explore this 
        promising direction. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Lap Fai (Craig) Yu
    </p>
    

<!-- ------------------------------------------------Data4XR-------------------------------------------------------- -->

    <h2 id="Data4XR"> Data4XR: Datasets for Developing Intelligent XR Applications </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'VHCIE2021' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/ieee-vr-data4xr/" target="_blank">https://sites.google.com/view/ieee-vr-data4xr/</a>
    </p>
    <ul>
        <li> Submission deadline: 7<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        Whenever AI researchers want to propose different data-driven models, datasets are the most fundamental resources. With 
        easy access to standard datasets, they can develop state-of-the-art AI algorithms to achieve excellent prediction performance. 
        However, when XR researchers decide to import these algorithms for developing intelligent immersive interactive applications, 
        the lack of publicly available datasets arises as a challenge despite advanced AI algorithms being developed.
    </p>
    <p>
        Many works related to datasets have been published, e.g., MINIST, ImageNet, CIFAR-10, etc. To unleash the full power of XR, 
        the community also needs standard datasets for developing data-driven models with machine&#47;deep learning. The workshop on 
        Datasets for Developing Intelligent XR Applications (Data4XR), hosted by the IEEE VR 2022, proposes a meaningful platform for 
        domain researchers to find valuable resources and develop collaborations across labs. It aims to promote XR research by 
        involving artificial intelligence.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Yuyang Wang
    </p>
    
    
<!-- ------------------------------------------------ReDigiTS-------------------------------------------------------- -->

    <h2 id="ReDigiTS"> 3D Reconstruction, Digital Twinning, and Simulation for Virtual Experiences (ReDigiTS) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'WISP' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/redigits" target="_blank">https://sites.google.com/view/redigits</a>
    </p>
    <ul>
        <li> Submission deadline: 5<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 25<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The aim of this workshop is to attract a collection of high-quality submissions reporting state-of-the-art research 
        activities targeted to the next generation of immersive experiences, reporting the latest methodologies, applications, 
        standards, evaluations, and&#47;or use cases for 3D reconstruction, digital twinning, and simulation for immersive experiences.
        Despite the pivotal role played by these research directions in the design and development of immersive experiences, 
        they are only partially addressed in the topics of workshops organized in the previous editions of IEEE VR.    
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Fabrizio Lamberti
    </p>
    
    
<!-- ------------------------------------------------VHCIE-------------------------------------------------------- -->

    <h2 id="VHCIE"> Workshop on Virtual Humans and Crowds in Immersive Environments (VHCIE) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'NIDIT' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://files.inria.fr/vhcie/2022" target="_blank">https://files.inria.fr/vhcie/2022</a>
    </p>
    <ul>
        <li> Submission deadline: 11<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        Nowadays many tools, including algorithms and systems, are available to create and design believable virtual humans and 
        crowds in immersive virtual environments (IVEs). One traditional research area is thereby the population of IVEs. With sophisticated 
        crowd simulations, environments with the size of an entire city can be efficiently enlivened with thousands of authentic virtual 
        characters, termed virtual agents. Typically, these agents only react to VR users in terms of interactions between walkers, including 
        collision avoidance, gazing, and interpersonal distance constraints. To this end, a second research area focuses on direct agent-user 
        interactions including communicative abilities and social behavior to design believable verbal and non-verbal behavior for agents in 
        face-to-face interactions. Research on both facets has been presented and discussed in the previous VHCIE editions, primarily from the 
        viewpoint of VR research. Thus, VHCIE 2022 widens the focus by starting a cross-community exchange with researchers from industry and 
        other disciplines involved in modeling, developing, and evaluating virtual humans and crowds. 
    </p>
    <p>
        The objective of VHCIE workshop on &quot;Virtual Humans and Crowds in Immersive Environments&quot; is then threefold. Through a panel and a 
        selection of submitted presentations (short papers and late breaking research), we will: 
        <ol>
            <li>
                Present state of the art character and crowd animation techniques for interactive agents. Recent developments in character 
                and crowd animations have impressively improved the level of quality for motions, as well as computational performances. 
                One objective of the workshop is to present how VR and immersive environments can benefit from these recent developments.
            </li>
            <li>
                Present some examples of new research opportunities offered by the availability of populated virtual environments. 
                Populating VEs with several autonomous characters is a relatively recent advancement. What research can benefit 
                from such capability? We expect presentations related to how recent technological advances enable or facilitate 
                such research. 
            </li>
            <li>
                Discuss technological requirements for future applications. Recent technologies and software have clearly eased the 
                creation of populated immersive VEs. However, there is still a way for improvement. Thus, the third objective of the
                workshop is to gather the requirements of current users of these technologies for future applications. To this end, 
                our audience and an invited cross-community panel from different research areas (VR, IVA, ..) as well as industry will 
                try to answer questions such as: Do users expect better animation quality? Better rendering? Or, higher level of 
                autonomy? What kind of interactivity is expected with autonomous agents?
            </li>
        </ol>
        Finally, we expect that the workshop will provide an opportunity for researchers to develop new techniques for virtual humans 
        and crowds and will possibly lead to new intersectoral collaborations.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Anne-H&eacute;l&egrave;ne Olivier
    </p>
    

<!-- ------------------------------------------------SIWI-------------------------------------------------------- -->

    <h2 id="SIWI"> Metaverse as a promise of a bright future? - social interactions in a world of isolation </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'WEVR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://workshop.htt.events/" target="_blank">https://workshop.htt.events/</a>
    </p>
    <ul>
        <li> Submission deadline: 12<sup>th</sup> January 2022 </li>
        <li> Notification of results: 18<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 25<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The Metaverse is before us. Extended Reality, which has so far been on the periphery of life, has a chance of 
        becoming an element of everyday life. The arrival of such a world has been accelerated, on the one hand, by 
        technological development and the readiness of IT corporations to invest in VR/XR technology, and on the other 
        hand, by a pandemic that prompted us to look for alternative ways to exist in isolation.
    </p>
    <p>
        This situation forces us to face completely new challenges. We must find ways to define ourselves in the virtual 
        world in various dimensions, including establishing social relationships or creating our own identity. We invite 
        you to our online workshop - a space for reflection on issues of social functioning in the world of the Metaverse. 
        The event has been designed to allow participants to interact in three autonomous forms: lectures combined with Q&A 
        sessions, an experiment involving participant observation in the VR environment, and thematic discussion sessions.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Anna Mierzecka
    </p>

<!-- ------------------------------------------------SIVE-------------------------------------------------------- -->

    <h2 id="SIVE"> Sonic Interaction in Virtual Environments </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'WEVR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sive.create.aau.dk/" target="_blank">https://sive.create.aau.dk/</a>
    </p>
    <ul>
        <li> Submission deadline: 12<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The main goal of this workshop is to increase among the virtual reality community the awareness of the importance 
        of sonic elements when designing virtual/augmented/mixed reality (VR/AR/MR) environments. We will also discuss how 
        research in other related fields such as film sound theory, product sound design, sound and music computing, game 
        sound design, and computer music can inform designers of VR/AR/MR environments. Moreover, the workshop will feature 
        state-of-the-art research on the field of sound for VR/AR/MR environments.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Michele Geronazzo
    </p>
    

<!-- ------------------------------------------------WEVR-------------------------------------------------------- -->

    <h2 id="WEVR"> 8th Workshop on Everyday Virtual Reality </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'KELVAR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://wevr.adalsimeone.me/" target="_blank">https://wevr.adalsimeone.me/</a>
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        WEVR aims at fostering discussion and bringing advance understanding on challenges and opportunities for &quot;Everyday&quot; Virtual, 
        Augmented and Mixed Reality topics in contexts and scenarios going beyond research laboratories and specialist environments. 
        Bringing together experts with diverse background, i.e. researchers, technicians, engineers, game developers, industry partners, 
        we hope to a new perspectives look and re-thinking on the following specified themes:
        <ul>
            <li>Gameplay Design and Player Interaction in consumer VR/AR</li>
            <li>Overcoming constraints of ordinary environments (e.g. locomotion techniques, object avoidance)</li>
            <li>Tangible and haptics support to interaction with the environment</li>
            <li>Co-located and Remote Social & Collaborative VR/AR and related challenges</li>
            <li>Cross-reality intersection (e.g., immersed, non/semi-immersed users)</li>
            <li>3D User Interfaces for Desktop or semi-immersive VR</li>
            <li>VR/AR for home healthcare and education</li>
            <li>Effects of prolonged VR use in domestic settings</li>
            <li>VR/AR development for non-technical creators</li>
            <li>New trends of VR applications</li>
        </ul>
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Adalberto Simeone
    </p>
    

<!-- ------------------------------------------------ARES-------------------------------------------------------- -->

    <h2 id="ARES"> ARES - Augmented Reality Enabling Superhuman Sports &#43; Serious Games </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'EXR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://wiki.tum.de/pages/viewpage.action?pageId=1003688592" target="_blank">https://wiki.tum.de/pages/viewpage.action?pageId=1003688592</a>
    </p>
    <ul>
        <li> Submission deadline: 12<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        In the last years, the usage of Augmented Reality (AR) advanced into new frontiers through the widespread adoption of affordable 
        mobile devices. For example, in Superhuman Sports, AR provides the potential to be a driving factor by revolutionizing team sports 
        or by introducing novel game mechanics. In the field of Serious Games, AR can bring 3D serious content into the physical world to 
        enhance immersion and knowledge transfer. In both areas, the full potential of this vision-based technology is still limited through 
        the lack of framework support and tangible controller feedback for purely virtual objects.
    </p>
    <p>
        We want to bring together experts from different computing and engineering disciplines to overcome the barriers of complex AR game 
        concepts and to enhance interactions with augmented objects in a playful way in two important research fields:
        <ul>
            <li>
                The goal of Superhuman Sports is to surpass the limitations of the human body by incorporating technology. Cognitive and 
                physical capabilities are augmented by involving rich interactions through tangible and virtual game objects. Concepts of 
                team sports based on competition and the exploration of new experiences through novel senses and reflexes, are helping to 
                augment traditional sports or to path the way towards new game ideas.
            </li>
            <li>
                Serious Games combine the world of playing games for entertainment with the goal of learning in an almost subconsciously manner. 
                Combining these two approaches requires meeting the demands of both. Learning content must be presented correctly and coherently, 
                but on the other hand, it must be perfectly integrated into a game concept.
            </li>
        </ul>
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Christian Eichhorn
    </p>
    

<!-- ------------------------------------------------XRHealth-------------------------------------------------------- -->

    <h2 id="XRHealth"> XR for Health and Wellbeing </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/xrhealth/" target="_blank">https://sites.google.com/view/xrhealth/</a>
    </p>
    <ul>
        <li> Submission deadline: 14<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The XR for Health and Wellbeing Workshop will take place during IEEE VR 2022 (Christchurch, NZ online virtual) focusing on 
        XR (AR/VR/MR) technologies to help in the broad areas of interest related to healthcare and wellbeing. XR technologies have 
        been experimented with in many areas of healthcare and well being over the years. With the ubiquitous use of XR devices 
        creates a great opportunity to further XR research to help support healthcare professionals and the wellbeing of people. 
        XR has demonstrated many advantages to various healthcare and wellbeing areas, however, more research is required. We aim 
        to gather the intersection of researchers working in the areas of XR for healthcare and wellbeing from the HCI community 
        to come together to share their ideas and discuss possible future grand challenges. We solicit short paper submissions with 
        lightning talks at the workshop. We will have a break-out session to discuss the topics of the workshop in more depth. We 
        will have two invited talks, one from academia and one from industry.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Craig Anslow
    </p>
    
    
<!-- ------------------------------------------------AVEH-------------------------------------------------------- -->

    <h2 id="AVEH"> Second Workshop on Applied VR for Enhanced Healthcare (AVEH) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> TBA <!--<a href="https://openarcloud/IEEE2021" target="_blank">https://openarcloud/IEEE2021</a>-->
    </p>
    <ul>
        <li> Submissions due: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 28<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        This workshop goal is to bring together expert knowledge in both technology and healthcare in order to explore how the potential 
        of VR can be used to support and enhance health and well-being. We will also encourage discussion of the challenges to development 
        and adoption of VR in healthcare, and how these might be addressed. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Wendy Powell
    </p>
    

<!-- ------------------------------------------------X-IRL-------------------------------------------------------- -->

    <h2 id="X-IRL"> X-IRL risks: Identifying privacy and security risks in inter-reality attacks and interactions </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'Finding-a-way-forward-in-VR-locomotion' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> TBA <!--<a href="https://locomotionvault.github.io/workshopieeevr.html" target="_blank">https://locomotionvault.github.io/workshopieeevr.html</a> -->
    </p>
    <ul>
        <li> Submission deadline: TBA </li>
        <li> Notification of results: TBA </li>
        <li> Camera-ready submission due: TBA </li>
    </ul>
    <p>
        This workshop extrapolates how virtual interactions and data trails may generate IRL (in real-life) consequences. 
        Participation in the metaverse and other XR technologies and spaces (AR and MR) may lead to new surface attacks and 
        vectors, the emergence of new adversaries and threat scenarios, and a heightened need for regulatory action, organisational 
        defences, and user-specific security tools. The goal of this workshop is to illuminate the potential inter-reality risks 
        generated between real and virtual worlds. It aims to gather insight from researchers and industry leaders in the 
        digital-to-XR and privacy and security communities in a collaborative and thought-provoking examination of the 
        expanding cybersecurity terrain. The one-hour workshop will be held online presenting a moderated discussion and 
        question time.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Moya Kate Baldry
    </p>
    

<!-- ------------------------------------------------METABUILD-------------------------------------------------------- -->

    <h2 id="METABUILD"> METABUILD: First Workshop for Building the Foundations of the Metaverse </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'PrXR' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://metabuild-workshop.herokuapp.com/" target="_blank">https://metabuild-workshop.herokuapp.com/</a>
    </p>
    <ul>
        <li> Submission deadline: 6<sup>th</sup> January 2022 </li>
        <li> Notification of results: 19<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The goal of this workshop is to discuss the issues related to building the metaverse under two directions: (1) technological 
        and engineering aspects allowing to develop the metaverse's ecosystems, and (2) content creation for and in the metaverse to 
        provide ownership to users. These two goals are interconnected as technology should support content creation, while content 
        creation should happen with respect of the technological advances. In more details, we target:
        <ol>
            <li>
                Engineering the metaverse. This workshop aims to discuss the engineering aspects of the metaverse, from the 
                supporting technologies (Mixed Reality, computer vision, IoT and robotics, Blockchain, User Interaction, Future 
                Networking Technologies, Cloud and Edge Computing, Artificial Intelligence), the building bricks of the metaverse 
                ecosystem (avatar and presence, virtual economy, content creation, social acceptability, privacy and ethics), and 
                applications (games, digital commerce, remote work and study, remote training).
            </li>
            <li>
                Content creation in and for the metaverse. With the vision of building the metaverse, numerous users, represented 
                by their avatars, can create valuable contents in highly diversified virtual worlds. In particular, users can 
                participate in creating elements to enrich the metaverse, including but not limited to cinematic, imagery, textual, 
                musical, elements. Such an enriched profile of content creation refers to 'metacreation'. Supporting such key 
                activities of user content creation in the metaverse are crucial for the development of the metaverse. 
            </li>
        </ol>
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Pan Hui
    </p>
    

<!-- ------------------------------------------------XRIOS-------------------------------------------------------- -->

    <h2 id="XRIOS"> 1st International Workshop on eXtended Reality for Industrial and Occupational Supports (XRIOS) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/xrios2022" target="_blank">https://sites.google.com/view/xrios2022</a>
    </p>
    <ul>
        <li> Submission deadline: 13<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        This workshop-eXtended Reality for Industrial and Occupational Supports (XRIOS)-aims to identify the current state 
        of XR research and the gaps in the scope of human factors and ergonomics, mainly related to the industrial and 
        occupational tasks, and discuss potential future research directions. XRIOS will build a community that bridges XR 
        developers, human factors and ergonomics researchers interested in industrial and occupational applications.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Heejin Jeong
    </p>
    

<!-- ------------------------------------------------SIVA-------------------------------------------------------- -->

    <h2 id="SIVA"> 1st International Workshop on Socially Intelligent Virtual Agents (SIVA) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/sivaieeevr2022" target="_blank">https://sites.google.com/view/sivaieeevr2022</a>
    </p>
    <ul>
        <li> Submission deadline: 13<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The workshop aims at the presentation of projects with innovative ideas in the field of socially intelligent 
        virtual agents and subsequent discussion of challenges emerging from these projects. In particular, the workshop 
        will focus on individualized, social human-agent relationships enabled by recent advances in AI research. 
        This will complement existing activities at IEEE VR that focus on either user-controlled avatars or the 
        functional aspects of conversational agents.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Susanne Schmidt
    </p>
    

<!-- ------------------------------------------------PERCxR-------------------------------------------------------- -->

    <h2 id="PERCxR"> 8th workshop on Perceptual and Cognitive Issues in XR (PERCxR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://percxr.com" target="_blank">https://percxr.com</a>
    </p>
    <ul>
        <li> Submission deadline: No papers accepted </li>
    </ul>
    <p>
        The crux of this workshop is the creation of a better understanding of the various perceptual and cognitive 
        issues that inform and constrain the design of effective extended reality systems.  There is neither an in-depth 
        overview of these factors, nor well-founded knowledge on most effects as gained through formal validation. In 
        particular, long-term usage effects are inadequately understood. Meanwhile, mobile platforms and emerging display 
        hardware (&quot;glasses&quot;) promise to ignite the number of users, as well as the system usage duration. To fulfill 
        usability needs, a thorough understanding of perceptual and intertwined cognitive factors is highly needed by 
        both research and industry: issues such as depth misinterpretation, object relationship mismatches and information 
        overload can severely limit usability of applications, or even pose risks in their usage. Based on the gained 
        knowledge, for example, new interactive visualization and view management techniques can be iteratively defined, 
        developed and validated, optimized to be congruent with human capabilities and limitations in route to more 
        usable application interfaces.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Rick Skarbez
    </p>
    

<!-- ------------------------------------------------EmpathicComputing-------------------------------------------------------- -->

    <h2 id="EmpathicComputing"> Empathic Computing </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong>  <a href="http://empathiccomputing.org/ecl-workshops/workshop-on-empathic-computing/" target="_blank">http://empathiccomputing.org/ecl-workshops/workshop-on-empathic-computing/</a>
    </p> 
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 18<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 28<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The goal of this workshop is to present important research topics in Empathic Computing, collaborative AR/VR and 
        related topics, and to identify key areas for the future research. It will hopefully contribute to growing the
        community of researchers interested in Empathic Computing related research topics.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Arindam Dey
    </p>
    

<!-- ------------------------------------------------HSVRAR-------------------------------------------------------- -->

    <h2 id="HSVRAR"> Health and Safety in VR and AR </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="http://empathiccomputing.org/ecl-workshops/workshop-on-health-and-safety-vrar/" target="_blank">http://empathiccomputing.org/ecl-workshops/workshop-on-health-and-safety-vrar/</a>
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 18<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 28<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        The goal of this workshop is to identify potential health and safety challenges associated with using AR 
        and VR systems, and research that should be conducted to address these concerns.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Mark Billinghurst
    </p>

<!-- ------------------------------------------------NIDIT-------------------------------------------------------- -->

    <h2 id="NIDIT"> Workshop on Novel Input Devices and Interaction Techniques (NIDIT)</h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> TBA
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        This full-day workshop will bring together researchers and industry practitioners to discuss and experience the future of input devices for VR, AR, and 3D User Interfaces, and help chart a course for the future of 3D interaction techniques.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Francisco R. Ortega
    </p>
    

<!-- ------------------------------------------------KELVAR-------------------------------------------------------- -->

    <h2 id="KELVAR"> 7th Annual Workshop on K-12&#43; Embodied Learning through Virtual and Augmented Reality (KELVAR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
    {% if event.location %}
    <div class="notice--info">
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
            {% endif %}
        </p>
    </div>
    {% endif %}
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/site/vrkelvar/" target="_blank">https://sites.google.com/site/vrkelvar/</a>
    </p>
    <ul>
        <li> Submission deadline: 3<sup>rd</sup> January 2022 </li>
        <li> Notification of results: 20<sup>th</sup> January 2022 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2022 </li>
    </ul>
    <p>
        In this workshop we aim to bring together educators, developers and researchers who are interested in 
        creating and deploying XR technologies for the educational contexts of the future. The workshop will 
        enable participants to discuss and engage with different approaches for designing and integrating XR 
        technologies with a specific focus on the challenges and potential for embodied learning in the classroom 
        for K-12, vocational and higher education.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Erica Southgate
    </p>
    
</div>
