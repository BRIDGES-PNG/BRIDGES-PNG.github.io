---
---

<style>
  :root {
    --ink: #1f2d35;
    --muted: #60717d;
    --navy: #09233f;
    --ocean: #0f6f86;
    --teal: #26a69a;
    --gold: #e9b44c;
    --coral: #d95d59;
    --sand: #fffaf0;
    --paper: #ffffff;
    --line: #dfe9ec;
  }

  html { scroll-behavior: smooth; }

  .page-wrap {
    max-width: 920px;
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
    background: linear-gradient(90deg, var(--navy), var(--ocean), var(--teal), var(--gold), var(--coral));
  }

  .masthead::after {
    content: "";
    position: absolute;
    right: -45px;
    bottom: -55px;
    width: 180px;
    height: 120px;
    border: 10px solid rgba(15, 111, 134, 0.16);
    border-top-color: rgba(233, 180, 76, 0.32);
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
    background: linear-gradient(90deg, var(--teal), var(--gold));
    margin: 0.35rem 0 1rem;
  }

  .placeholder {
    color: var(--muted);
    font-style: italic;
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
    background: #f3faf9;
    color: var(--navy);
  }

  .apply-box {
    background: #f8fcfc;
    border: 1px solid var(--line);
    border-left: 6px solid var(--coral);
    border-radius: 10px;
    padding: 1rem;
  }

  .footer-contact {
    background: var(--navy);
    color: white;
    border-radius: 12px;
    padding: 1.3rem;
    margin: 1.5rem 0;
  }

  .footer-contact h2,
  .footer-contact a {
    color: white;
  }

  @media (max-width: 650px) {
    .masthead { padding: 1.5rem; }
    .masthead-inner { grid-template-columns: 1fr; }
  }
</style>

<div class="page-wrap">
  <nav class="simple-nav" aria-label="Website sections">
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
          <span>Dates to be announced</span>
          <span>Venue to be announced</span>
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
      BRIDGES 2027 will continue the mission of making software engineering more accessible, inclusive,
      and globally connected. The summer school will focus on practical software solutions, responsible AI,
      open-source collaboration, and emerging technologies in the context of Papua New Guinea and the wider Pacific region.
    </p>
    <p class="placeholder">Final 2027 theme and description coming soon.</p>
  </section>

  <section id="highlights">
    <div class="label">What to expect</div>
    <h2>Event Highlights</h2>
    <div class="section-mark"></div>
    <div class="three-col">
      <div class="plain-card"><strong>Research</strong><p>Gain feedback on ideas and connect with researchers and mentors.</p></div>
      <div class="plain-card"><strong>Education</strong><p>Learn practical skills in software engineering, AI tools, GitHub, and open source.</p></div>
      <div class="plain-card"><strong>Community</strong><p>Build connections between Pacific communities and global software engineering networks.</p></div>
      <div class="plain-card"><strong>Hackathon</strong><p class="placeholder">Team challenge details coming soon.</p></div>
      <div class="plain-card"><strong>Keynotes</strong><p class="placeholder">Speaker lineup coming soon.</p></div>
      <div class="plain-card"><strong>Certificates</strong><p>Participants will receive a certificate of attendance.</p></div>
    </div>
  </section>

  <section id="venue">
    <div class="label">Location</div>
    <h2>Venue</h2>
    <div class="section-mark"></div>
    <p class="placeholder">2027 venue to be announced.</p>
    <p>This section will include venue description, transport schedule, accommodation guidance, and travel information.</p>
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
    <h2>Speakers and Abstracts</h2>
    <div class="section-mark"></div>
    <p class="placeholder">Speaker names, photos, biographies, talk titles, abstracts, and slides will be added here.</p>
    <div class="two-col">
      <div class="plain-card"><strong>Speaker 1</strong><p>To be announced.</p></div>
      <div class="plain-card"><strong>Speaker 2</strong><p>To be announced.</p></div>
      <div class="plain-card"><strong>Speaker 3</strong><p>To be announced.</p></div>
      <div class="plain-card"><strong>Speaker 4</strong><p>To be announced.</p></div>
    </div>
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
      <p>
        BRIDGES 2027 will welcome students, researchers, practitioners, mentors, and international participants
        interested in software engineering, AI, emerging technologies, and Pacific-centered innovation.
      </p>
      <p class="placeholder">Application instructions, deadlines, registration form, and participant requirements coming soon.</p>
    </div>
  </section>

  <section id="team">
    <div class="label">Organizers</div>
    <h2>Meet the Team</h2>
    <div class="section-mark"></div>
    <p class="placeholder">2027 organizing team details coming soon.</p>
    <ul>
      <li>Organizer names and affiliations to be added.</li>
      <li>Local partners and supporting institutions to be added.</li>
    </ul>
  </section>

  <section id="past-editions">
    <div class="label">Archive</div>
    <h2>Past Editions</h2>
    <div class="section-mark"></div>
    <ul>
      <li><a href="./2026/">BRIDGES 2026</a></li>
      <li><a href="https://naist-se.github.io/PNG-BRIDGES">BRIDGES 2023</a></li>
      <li><a href="https://naist-se.github.io/BRIDGES2019">BRIDGES 2019</a></li>
    </ul>
  </section>

  <section class="footer-contact" id="contact">
    <h2>Contact</h2>
    <p>For more information, email: <strong>bridges.png@gmail.com</strong></p>
  </section>
</div>
