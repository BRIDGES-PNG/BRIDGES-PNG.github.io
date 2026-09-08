---
---

<style>
  :root {
    --ink: #09233F;
    --muted: #60717D;
    --navy: #09233F;
    --ocean: #0F6F86;
    --teal: #26A69A;
    --gold: #E9B44C;
    --sand: #FFFAF0;
    --paper: #FFFFFF;
    --line: #DFE9EC;
  }

  html { scroll-behavior: smooth; }

  body {
    background: #F7FAFC;
    color: var(--muted);
  }

  a { color: var(--ocean); }

  .page-wrap {
    max-width: 1240px;
    margin: 0 auto;
  }

  .simple-nav {
    border-top: 4px solid var(--teal);
    border-bottom: 1px solid var(--line);
    padding: 0.75rem 0;
    margin: 1rem 0 2rem;
  }

  .simple-nav a {
    display: inline-block;
    margin: 0.25rem 0.9rem 0.25rem 0;
    color: var(--navy);
    font-weight: 700;
    text-decoration: none;
  }

  .simple-nav .brand-link {
    margin-right: 1.3rem;
    vertical-align: middle;
  }

  .simple-nav .brand-link img {
    height: 46px;
    width: auto;
    display: inline-block;
    vertical-align: middle;
  }

  .masthead {
    background: var(--sand);
    border: 1px solid var(--line);
    border-radius: 12px;
    padding: 2.2rem;
    margin-bottom: 1.5rem;
    position: relative;
    overflow: hidden;
  }

  .masthead::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 10px;
    background: linear-gradient(90deg, var(--navy), var(--ocean), var(--teal));
  }

  .masthead::after {
    content: "";
    position: absolute;
    right: -45px;
    bottom: -55px;
    width: 180px;
    height: 120px;
    border: 10px solid rgba(15, 111, 134, 0.16);
    border-top-color: rgba(38, 166, 154, 0.28);
    border-radius: 50% 50% 0 0;
    transform: rotate(-10deg);
  }

  .label {
    color: var(--ocean);
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    font-size: 0.85rem;
  }

  .masthead h1 {
    margin: 0.4rem 0 0;
    color: var(--navy);
    font-size: clamp(2rem, 4vw, 3.2rem);
    line-height: 1.1;
  }

  .masthead h2 {
    color: var(--ink);
    font-weight: 500;
    margin-top: 0.7rem;
  }

  .status-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 1rem;
  }

  .status-row span {
    background: white;
    border: 1px solid var(--line);
    border-radius: 999px;
    padding: 0.45rem 0.75rem;
    color: var(--navy);
    font-weight: 700;
  }

  .logo-note {
    margin-top: 1.3rem;
    padding: 0.85rem 1rem;
    background: white;
    border-left: 5px solid var(--gold);
    border-radius: 8px;
    color: var(--muted);
  }

  .masthead-inner {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 1.45fr) minmax(220px, 0.55fr);
    gap: 1.5rem;
    align-items: center;
  }

  .masthead-logo {
    text-align: center;
  }

  .logo-frame {
    min-height: 210px;
    display: grid;
    place-items: center;
    padding: 1.2rem;
  }

  .logo-frame img {
    max-width: 375px;
    width: 100%;
    height: auto;
    display: block;
  }

  section {
    padding: 1.55rem 0;
    border-bottom: 1px solid var(--line);
  }

  section h2 {
    color: var(--navy);
    margin-bottom: 0.2rem;
  }

  .section-mark {
    width: 72px;
    height: 4px;
    border-radius: 99px;
    background: var(--teal);
    margin: 0.35rem 0 1rem;
  }

  .placeholder {
    color: var(--muted);
    font-style: italic;
  }

  .venue-name {
    color: var(--navy);
    font-size: 1.2rem;
    font-weight: 800;
    margin: 0 0 0.25rem;
  }

  .venue-name a {
    color: var(--navy);
  }

  .venue-location {
    color: var(--muted);
    font-size: 0.95rem;
    margin: 0 0 1rem;
  }

  .venue-notice {
    background: #F7FAFC;
    border: 1px solid var(--line);
    border-left: 5px solid var(--teal);
    border-radius: 10px;
    color: var(--muted);
    font-style: italic;
    margin: 1rem 0 0;
    padding: 0.85rem 1rem;
  }

  .team-notice {
    background: #F7FAFC;
    border: 1px solid var(--line);
    border-left: 5px solid var(--teal);
    border-radius: 10px;
    color: var(--muted);
    font-style: italic;
    margin: 1rem 0 0;
    padding: 0.8rem 1rem;
  }

  .two-col, .three-col {
    display: grid;
    gap: 1rem;
  }

  .two-col { grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); }
  .three-col { grid-template-columns: repeat(auto-fit, minmax(190px, 1fr)); }

  .plain-card {
    background: var(--paper);
    border: 1px solid var(--line);
    border-radius: 10px;
    padding: 1rem;
  }

  .plain-card strong {
    color: var(--ocean);
  }

  .highlight-grid {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .highlight-card {
    background: var(--paper);
    border: 1px solid var(--line);
    border-radius: 12px;
    display: flex;
    flex-direction: column;
    min-height: 0;
    padding: 0.9rem 1rem;
  }

  .highlight-icon {
    color: var(--ocean);
    height: 28px;
    margin-bottom: 0.65rem;
    width: 28px;
  }

  .highlight-icon svg {
    display: block;
    fill: none;
    height: 100%;
    stroke: currentColor;
    stroke-linecap: round;
    stroke-linejoin: round;
    stroke-width: 1.8;
    width: 100%;
  }

  .highlight-card strong {
    color: var(--ocean);
  }

  .highlight-card p {
    color: var(--muted);
    margin-bottom: 0;
  }


  .speaker-headshot {
    width: 100%;
    max-width: 300px;
    border-radius: 10px;
    display: block;
    margin-bottom: 0.9rem;
  }

  .speaker-label {
    color: var(--ocean);
    font-size: 0.72rem;
    font-weight: 800;
    letter-spacing: 0.08em;
    line-height: 1.1;
    margin-bottom: 0.4rem;
    text-transform: uppercase;
  }

  .speaker-note {
    color: var(--muted);
    font-style: italic;
    margin: 1rem 0 0;
  }

  .program-block {
    border-left: 4px solid var(--teal);
    padding-left: 1rem;
    margin: 1rem 0;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin: 0.8rem 0;
  }

  th, td {
    border: 1px solid var(--line);
    padding: 0.65rem;
    text-align: left;
  }

  th {
    background: #F7FAFC;
    color: var(--navy);
  }

  .apply-box {
    background: var(--paper);
    border-radius: 10px;
    padding: 0 0 0.9rem;
  }

  .apply-box h3 {
    color: var(--navy);
    margin: 0 0 0.45rem;
  }

  .apply-box p {
    margin: 0;
  }

  .registration-status {
    border: 1px solid var(--line);
    border-left: 6px solid var(--gold);
    border-radius: 10px;
    margin-top: 1rem;
    padding: 0.85rem 1rem;
  }

  .registration-label {
    color: var(--ocean);
    font-size: 0.72rem;
    font-weight: 800;
    letter-spacing: 0.08em;
    line-height: 1.1;
    text-transform: uppercase;
  }

  .registration-value {
    color: var(--navy);
    font-size: 1.15rem;
    font-weight: 800;
    margin-top: 0.25rem;
  }

  .registration-note {
    color: var(--muted);
    font-size: 0.95rem;
    margin-top: 0.25rem;
  }

  .footer-contact {
    background: #073B4C;
    color: #FFFFFF;
    border: 1px solid var(--line);
    border-radius: 12px;
    padding: 0.95rem 1.3rem;
    margin: 1.5rem 0;
  }

  .footer-contact h2 {
    color: #FFFFFF;
    margin: 0 0 0.35rem;
  }

  .footer-accent {
    width: 64px;
    height: 3px;
    border-radius: 99px;
    background: #26A69A;
    margin: 0 0 0.85rem;
  }

  .footer-contact a {
    color: #FFFFFF;
    text-decoration-color: #26A69A;
  }

  .footer-contact p {
    margin: 0 0 0.25rem;
  }

  .footer-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1.5rem;
  }

  .footer-logo {
    display: block;
    max-width: 190px;
    width: 100%;
    height: auto;
    flex: 0 0 190px;
  }

  .footer-divider {
    border: 0;
    border-top: 1px solid rgba(223, 233, 236, 0.35);
    margin: 0.95rem 0 0.65rem;
  }

  .footer-meta {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
    color: #DFE9EC;
    font-size: 0.85rem;
  }

  @media (max-width: 650px) {
    .masthead { padding: 1.5rem; }
    .masthead-inner { grid-template-columns: 1fr; }
    .highlight-grid { grid-template-columns: 1fr; }
    .footer-inner {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
    .footer-logo {
      max-width: 165px;
      flex-basis: auto;
    }
    .footer-accent { margin-left: auto; margin-right: auto; }
    .footer-meta {
      flex-direction: column;
      align-items: center;
      gap: 0.25rem;
      text-align: center;
    }
  }
</style>

<div class="page-wrap">
  <nav class="simple-nav" aria-label="Website sections">
    <a class="brand-link" href="#workshop-logo"><img src="img/BRIDGES27_logo%20text.png" alt="BRIDGES 2027"></a>
    <a href="#about">About</a>
    <a href="#highlights">Highlights</a>
    <a href="#venue">Venue</a>
    <a href="#program">Program</a>
    <a href="#speakers">Speakers</a>
    <a href="#fees">Fees</a>
    <a href="#participants">Apply</a>
    <a href="#team">Team</a>
    <a href="#past-editions">Past Editions</a>
  </nav>

  <header class="masthead" id="workshop-logo">
    <div class="masthead-inner">
      <div>
        <div class="label">BRIDGES 2027 · Summer School in the South Pacific</div>
        <h1>Bridging the Divides with Globally Engineered Software</h1>
        <h2>Papua New Guinea and Pacific communities exploring software engineering, AI, open source, and emerging technologies.</h2>
        <div class="status-row">
          <span>January 9th - 11th, 2027</span>
          <span>Loloata Island Resort</span>
          <span>Registration coming soon</span>
        </div>
      </div>
      <div class="masthead-logo">
        <div class="logo-frame">
          <img src="img/bridges_logo27_mark.png" alt="BRIDGES 2027 workshop logo">
        </div>
      </div>
    </div>
  </header>

  <section id="about">
    <div class="label">Purpose</div>
    <h2>About BRIDGES 2027</h2>
    <div class="section-mark"></div>
    <p>
      BRIDGES 2027 continues the mission of making software engineering more accessible,
      inclusive, and globally connected in Papua New Guinea and the wider Pacific. The summer
      school will bring participants together to explore practical software solutions, responsible AI,
      open-source collaboration, and emerging technologies.
    </p>
    <p>
      Under the theme “<strong>Building a Digital App Ecosystem with Agentic AI Technologies</strong>,”
      participants will develop and showcase AI-enabled applications, prototypes, and ideas through an
      open digital hub. The initiative aims to encourage collaboration and local innovation while respecting
      Papua New Guinea’s cultures, languages, regulations, data sovereignty, and social contexts.
    </p>
    <p>
      BRIDGES 2027 will also connect local talent with wider technical and professional communities,
      helping make Papua New Guinean innovation more visible nationally and internationally.
    </p>
  </section>

  <section id="highlights">
    <div class="label">What to expect</div>
    <h2>Event Highlights</h2>
    <div class="section-mark"></div>
    <div class="highlight-grid">
      <div class="highlight-card">
        <div class="highlight-icon" aria-hidden="true">
          <svg viewBox="0 0 24 24"><path d="M4 19.5V5a2 2 0 0 1 2-2h12v16H6a2 2 0 0 0-2 2z"></path><path d="M8 7h6M8 11h8"></path></svg>
        </div>
        <strong>Hands-on Learning</strong>
        <p>Practical workshops and tutorials in software engineering, AI, open source, and emerging technologies.</p>
      </div>
      <div class="highlight-card">
        <div class="highlight-icon" aria-hidden="true">
          <svg viewBox="0 0 24 24"><path d="M7 8h10M7 12h6"></path><rect x="4" y="4" width="16" height="12" rx="2"></rect><path d="M9 20h6M12 16v4"></path></svg>
        </div>
        <strong>Team Projects</strong>
        <p>Collaborate to design and build AI-enabled applications, prototypes, and solutions.</p>
      </div>
      <div class="highlight-card">
        <div class="highlight-icon" aria-hidden="true">
          <svg viewBox="0 0 24 24"><path d="M12 3l2.2 4.5L19 8.2l-3.5 3.4.8 4.8L12 14.1l-4.3 2.3.8-4.8L5 8.2l4.8-.7z"></path><path d="M8 21h8"></path></svg>
        </div>
        <strong>Keynote &amp; Expert Talks</strong>
        <p>Learn from researchers and experts in software engineering, AI, and emerging technologies.</p>
      </div>
      <div class="highlight-card">
        <div class="highlight-icon" aria-hidden="true">
          <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="8"></circle><path d="M4 12h16M12 4c2 2.2 3 4.9 3 8s-1 5.8-3 8M12 4c-2 2.2-3 4.9-3 8s1 5.8 3 8"></path></svg>
        </div>
        <strong>Pacific-Centered Innovation</strong>
        <p>Explore technology that responds to local needs and the social and cultural contexts of Papua New Guinea and the Pacific.</p>
      </div>
    </div>
  </section>

  <section id="venue">
    <div class="label">Location</div>
    <h2>Venue</h2>
    <div class="section-mark"></div>
    <p class="venue-name">Proposed Venue: <a href="https://www.loloataislandresort.com/">Loloata Island Resort</a></p>
    <p class="venue-location">📍 Port Moresby, Central Province, Papua New Guinea</p>
    <p>
      BRIDGES 2027 is tentatively planned to take place at Loloata Island Resort, located on an island
      just outside Port Moresby, the capital of Papua New Guinea. Known as the Land of the Unexpected,
      Papua New Guinea is home to more than 850 languages, rich cultural traditions, and remarkable
      biodiversity, including the iconic Bird of Paradise and Queen Alexandra’s Birdwing.
    </p>
    <p class="venue-notice">Venue confirmation and further information on transportation, accommodation, and travel arrangements will be announced soon.</p>
  </section>

  <section id="program">
    <div class="label">Schedule</div>
    <h2>Overview of Program</h2>
    <div class="section-mark"></div>
    <p class="placeholder">Detailed 2027 schedule coming soon. Draft structure below.</p>

    <div class="program-block">
      <h3>Day 1 — Welcome and Foundations</h3>
      <table>
        <tr><th>Session</th><th>Details</th></tr>
        <tr><td>Morning</td><td>Registration, welcome, and opening remarks</td></tr>
        <tr><td>Midday</td><td>Keynote talks and introductions</td></tr>
        <tr><td>Afternoon</td><td>Git, GitHub, software tools, and AI-assisted development</td></tr>
      </table>
    </div>

    <div class="program-block">
      <h3>Day 2 — Learning and Building</h3>
      <table>
        <tr><th>Session</th><th>Details</th></tr>
        <tr><td>Morning</td><td>Technical sessions and tutorials</td></tr>
        <tr><td>Midday</td><td>Team challenge or hackathon work</td></tr>
        <tr><td>Afternoon</td><td>Mentoring, prototyping, and group feedback</td></tr>
      </table>
    </div>

    <div class="program-block">
      <h3>Day 3 — Presentations and Future Directions</h3>
      <table>
        <tr><th>Session</th><th>Details</th></tr>
        <tr><td>Morning</td><td>Team presentations and live feedback</td></tr>
        <tr><td>Midday</td><td>Awards, certificates, and closing remarks</td></tr>
        <tr><td>Afternoon</td><td>Future planning discussions</td></tr>
      </table>
    </div>
  </section>

  <section id="speakers">
    <div class="label">People</div>
    <h2>Speakers</h2>
    <div class="section-mark"></div>
    <div class="two-col">
      <div class="plain-card">
        <img class="speaker-headshot" src="https://staffphoto.smu.edu.sg/s/davidlo/600x400" alt="Prof. David Lo">
        <div class="speaker-label">Keynote Speaker</div>
        <strong>Prof. David Lo</strong>
        <p><em>Vice Provost (Research) &amp; OUB Chair Professor of Computer Science</em><br>
        <strong>Singapore Management University</strong></p>
        <p>Professor David Lo is a leading researcher in software engineering and artificial intelligence. His research explores intelligent software engineering, AI-assisted software development, software analytics, and trustworthy software and AI systems. He is also Co-Director of SMU's Centre for Research for Intelligent Software Engineering (RISE).</p>
        <p><strong>Keynote Title:</strong> To be announced.</p>
      </div>
    </div>
    <p class="speaker-note">Additional speakers will be announced soon.</p>
  </section>

  <section id="fees">
    <div class="label">Registration</div>
    <h2>Tuition Fee</h2>
    <div class="section-mark"></div>
    <p class="placeholder">2027 fee structure and deadlines to be announced.</p>
    <table>
      <tr><th>Category</th><th>Fee</th><th>Deadline</th></tr>
      <tr><td>Students</td><td>To be announced</td><td>To be announced</td></tr>
      <tr><td>Early Bird</td><td>To be announced</td><td>To be announced</td></tr>
      <tr><td>Regular</td><td>To be announced</td><td>To be announced</td></tr>
    </table>
  </section>

  <section id="participants">
    <div class="label">Join us</div>
    <h2>Call for Participants</h2>
    <div class="section-mark"></div>
    <div class="apply-box">
      <h3>Who can participate?</h3>
      <p>
        BRIDGES 2027 welcomes students, researchers, practitioners, and mentors interested in software
        engineering, AI, emerging technologies, and Pacific-centered innovation. The summer school aims
        to bring together participants from Papua New Guinea, the wider Pacific, and the international
        community to learn, collaborate, and exchange ideas.
      </p>
      <div class="registration-status">
        <div class="registration-label">Registration</div>
        <div class="registration-value">Coming soon</div>
        <div class="registration-note">Application details, participant requirements, and deadlines will be announced here.</div>
      </div>
    </div>
  </section>

  <section id="team">
    <div class="label">Organizers</div>
    <h2>Meet the Team</h2>
    <div class="section-mark"></div>
    <p>BRIDGES 2027 is made possible through collaboration between organizers, researchers, educators, and partners in Papua New Guinea and the wider international software engineering community.</p>
    <div class="team-notice">The 2027 organizing team and partner information will be announced soon.</div>
  </section>

  <section id="past-editions">
    <div class="label">Archive</div>
    <h2>Past Editions</h2>
    <div class="section-mark"></div>
    <ul>
      <li><a href="https://bridges-png.github.io/2026/">BRIDGES 2026</a></li>
      <li><a href="https://naist-se.github.io/PNG-BRIDGES">BRIDGES 2023</a></li>
      <li><a href="https://naist-se.github.io/BRIDGES2019">BRIDGES 2019</a></li>
    </ul>
  </section>

  <section class="footer-contact" id="contact">
    <div class="footer-inner">
      <div>
        <h2>Contact</h2>
        <div class="footer-accent"></div>
        <p><strong>Questions about BRIDGES 2027?</strong></p>
        <p>For general enquiries, contact us at <a href="mailto:bridges.png@gmail.com"><strong>bridges.png@gmail.com</strong></a></p>
      </div>
      <img class="footer-logo" src="img/bridges_logo27.png" alt="BRIDGES 2027 logo">
    </div>
    <hr class="footer-divider">
    <div class="footer-meta">
      <span>BRIDGES 2027 · Papua New Guinea</span>
      <span>© 2027 BRIDGES</span>
    </div>
  </section>
</div>
