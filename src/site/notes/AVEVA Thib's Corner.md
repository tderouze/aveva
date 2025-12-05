---
{"dg-publish":true,"dg-home":true,"permalink":"/aveva-thib-s-corner/","tags":["gardenEntry"],"dgPassFrontmatter":true}
---

# Welcome to Thib's Corner

👋 Hello and welcome on my AVEViAn Website

<u>**Who am I :**</u>
From Elicitator to AI Prompt Architect, via Ultracrepidarianist, I am just a normal Presales Engineer who like to speak about Tech and Operations. If it grabbed your attention, check my linked profile for more details:
<center><script src="https://platform.linkedin.com/badges/js/profile.js" async defer type="text/javascript"></script>
<div class="badge-base LI-profile-badge" data-locale="fr_FR" data-size="medium" data-theme="light" data-type="VERTICAL" data-vanity="tderouze" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://fr.linkedin.com/in/tderouze?trk=profile-badge">Thibaud de Rouzé</a></div></center>


<div id="forest-graph">
    <div class="forest-body">
        {% for row in userComputed.forest.trees %}
        <div class="forest-row">
            {% for tree in row %}
            {% if tree[0] == 0 %}
            <span class="tree plane}">
                <span></span>
            </span>
            {% else %}
            <a class="tree" href="{{tree[1]}}" title="{{tree[2]}}">
                <img src="/img/{{tree[0]}}.svg" alt="" style="width: auto;height: {{5 + (10 * tree[3])}}px;" />
            </a>
            {% endif %}
            {% endfor %}
        </div>
        {% endfor %}
    </div>
    <div class="forest-legends">
        {% for count in userComputed.forest.legends %}
        <div class="stat"><img src="/img/{{count.icon}}.svg" alt="{{count.label}}" />{{count.count}} {% if count.count > 1 %}{% if count.plural %}{{count.plural}}{% else %}{{count.label}}s{% endif %}{% else %}{{count.label}}{% endif %}</div>
        {% endfor %}
    </div>
</div>

### My Last Blog Post

- 2025-11-28 - [[Blog Articles/AVEVA PI System/Comparing AVEVA PI System and Optimistik – Which Fits Your Operational Data Journey\|Comparing AVEVA PI System and Optimistik – Which Fits Your Operational Data Journey]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/CONNECT vs PI Integrator - Choosing the Right Tool for Your Industrial Data Needs\|CONNECT vs PI Integrator - Choosing the Right Tool for Your Industrial Data Needs]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/AVEVA PI System vs Cloud Historian - Why PI Excels in Industrial Environments\|AVEVA PI System vs Cloud Historian - Why PI Excels in Industrial Environments]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/Data Diode Architecture for AVEVA PI System\|Data Diode Architecture for AVEVA PI System]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/Deploying AVEVA PI System at Scale - A Comprehensive Guide\|Deploying AVEVA PI System at Scale - A Comprehensive Guide]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/PI AF 10 Commandments - Your Guide to Data Management Excellence\|PI AF 10 Commandments - Your Guide to Data Management Excellence]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/Port Operations with AVEVA PI System\|Port Operations with AVEVA PI System]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/The top five advantages of PI Datalink\|The top five advantages of PI Datalink]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/Revolutionizing Batch Management with AVEVA PI System\|Revolutionizing Batch Management with AVEVA PI System]]
- 2025-11-28 - [[Blog Articles/AVEVA PI System/Unlock Maritime Efficiency and Sustainability with AVEVA PI System\|Unlock Maritime Efficiency and Sustainability with AVEVA PI System]]

{ .block-language-dataview}

### My Last Youtube Videos

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/l8Cpq6hN_ag?si=YI0I0_LBNDJbGTlG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></center>

<hr><center>
    <small><span id="visit-counter"><code></code></span> Page Visits</small>
</center>

<script>
// Get the current page URL (host + pathname) for consistent counting
const currentUrl = window.location.host + window.location.pathname;
const encodedUrl = encodeURIComponent(currentUrl);

fetch(`https://visit-counter.vercel.app/counter?page=${encodedUrl}`)
  .then(response => response.text())
  .then(count => {
    console.log('Visit count:', count);
    // Optional: Display the count on your page
    const counterElement = document.getElementById('visit-counter');
    if (counterElement) {
      counterElement.innerHTML = `<code>${count}</code>`;
    }
  })
  .catch(error => {
    console.error('Error fetching visit count:', error);
  });
  </script>