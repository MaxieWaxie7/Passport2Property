
<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,300;1,400&family=Inter:wght@300;400;500&display=swap');
*{margin:0;padding:0;box-sizing:border-box;}
:root{
  --gold:#B8935A;
  --gold-lt:#E2C99A;
  --cream:#F8F4EE;
  --deep:#181410;
  --ink:#2A2218;
  --muted:#7A6E5F;
  --terra:#B85C38;
  --sage:#5A7050;
  --off:#FDFAF6;
}
.site{font-family:'Inter',sans-serif;color:var(--ink);background:#fff;width:100%;}

nav{display:flex;align-items:center;justify-content:space-between;padding:1.1rem 2.5rem;border-bottom:1px solid rgba(184,147,90,0.18);background:#fff;position:sticky;top:0;z-index:10;}
.logo{font-family:'Cormorant Garamond',serif;font-size:1.55rem;font-weight:400;letter-spacing:0.03em;color:var(--deep);}
.logo span{color:var(--gold);}
.nav-r{display:flex;align-items:center;gap:2rem;}
.nav-r a{font-size:0.72rem;letter-spacing:0.13em;text-transform:uppercase;color:var(--muted);text-decoration:none;}
.nav-r a:hover{color:var(--ink);}
.nav-btn{background:var(--gold);color:#fff !important;padding:0.5rem 1.2rem;border-radius:2px;letter-spacing:0.1em !important;}

.hero{background:var(--cream);padding:3rem 2.5rem 2.5rem;position:relative;overflow:hidden;}
.hero::before{content:'';position:absolute;inset:0;background:repeating-linear-gradient(90deg,rgba(184,147,90,0.06) 0px,rgba(184,147,90,0.06) 1px,transparent 1px,transparent 80px),repeating-linear-gradient(0deg,rgba(184,147,90,0.06) 0px,rgba(184,147,90,0.06) 1px,transparent 1px,transparent 80px);}
.hero-inner{position:relative;max-width:680px;}
.eyebrow{display:flex;align-items:center;gap:0.7rem;margin-bottom:1.25rem;}
.eline{width:2rem;height:1px;background:var(--gold);}
.etxt{font-size:0.68rem;letter-spacing:0.22em;text-transform:uppercase;color:var(--gold);}
.hero h1{font-family:'Cormorant Garamond',serif;font-size:clamp(2.8rem,5.5vw,4.4rem);font-weight:300;line-height:1.1;color:var(--deep);margin-bottom:1.1rem;}
.hero h1 em{font-style:italic;color:var(--terra);}
.hero p{font-size:0.95rem;color:var(--muted);line-height:1.75;max-width:500px;margin-bottom:1.75rem;font-weight:300;}
.hero-btns{display:flex;gap:1rem;align-items:center;flex-wrap:wrap;margin-bottom:2rem;}
.btn{background:var(--gold);color:#fff;padding:0.85rem 2rem;font-size:0.75rem;letter-spacing:0.13em;text-transform:uppercase;border:none;cursor:pointer;border-radius:2px;font-family:'Inter',sans-serif;transition:opacity 0.2s;}
.btn:hover{opacity:0.88;}
.btn-out{background:transparent;color:var(--muted);padding:0.85rem 0;font-size:0.75rem;letter-spacing:0.12em;text-transform:uppercase;border:none;cursor:pointer;font-family:'Inter',sans-serif;}
.btn-out:hover{color:var(--ink);}
.hero-badges{display:flex;gap:1.5rem;}
.badge{font-size:0.65rem;letter-spacing:0.13em;text-transform:uppercase;color:var(--muted);display:flex;align-items:center;gap:0.4rem;}
.bdot{width:5px;height:5px;border-radius:50%;background:var(--gold);opacity:0.7;}

.section{padding:5rem 2.5rem;}
.section.cream{background:var(--cream);}
.section.white{background:#fff;}
.sec-label{font-size:0.68rem;letter-spacing:0.2em;text-transform:uppercase;color:var(--gold);margin-bottom:0.9rem;}
.sec-h{font-family:'Cormorant Garamond',serif;font-size:2.3rem;font-weight:400;line-height:1.2;color:var(--deep);margin-bottom:0.7rem;}
.sec-sub{font-size:0.88rem;color:var(--muted);line-height:1.7;max-width:520px;font-weight:300;margin-bottom:3rem;}

.steps{display:grid;grid-template-columns:repeat(4,1fr);gap:0;border:1px solid rgba(184,147,90,0.2);}
.step{padding:2rem 1.6rem;border-right:1px solid rgba(184,147,90,0.2);background:#fff;}
.step:last-child{border-right:none;}
.step-n{font-family:'Cormorant Garamond',serif;font-size:2.2rem;font-weight:300;color:var(--gold-lt);line-height:1;margin-bottom:1rem;}
.step h3{font-family:'Cormorant Garamond',serif;font-size:1.1rem;font-weight:500;color:var(--deep);margin-bottom:0.55rem;}
.step p{font-size:0.8rem;color:var(--muted);line-height:1.65;font-weight:300;}

.dest-row{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:rgba(184,147,90,0.18);}
.dest{background:#fff;padding:2.25rem 1.75rem;}
.dest:hover{background:var(--off);}
.dest-emoji{font-size:1.75rem;display:block;margin-bottom:0.9rem;}
.dest h3{font-family:'Cormorant Garamond',serif;font-size:1.7rem;font-weight:400;color:var(--deep);margin-bottom:0.25rem;}
.dest-sub{font-size:0.72rem;letter-spacing:0.08em;color:var(--terra);text-transform:uppercase;margin-bottom:0.9rem;display:block;}
.dest p{font-size:0.8rem;color:var(--muted);line-height:1.7;margin-bottom:1.25rem;font-weight:300;}
.tags{display:flex;flex-wrap:wrap;gap:0.35rem;}
.tag{font-size:0.65rem;letter-spacing:0.07em;text-transform:uppercase;color:var(--sage);background:rgba(90,112,80,0.09);padding:0.25rem 0.6rem;border-radius:2px;}

.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:start;}
.about-quote{font-family:'Cormorant Garamond',serif;font-size:1.45rem;font-weight:300;font-style:italic;color:var(--deep);line-height:1.5;border-left:2px solid var(--gold);padding-left:1.5rem;margin-bottom:2rem;}
.about-body{font-size:0.85rem;color:var(--muted);line-height:1.8;font-weight:300;margin-bottom:1.5rem;}
.stats-row{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;border:1px solid rgba(184,147,90,0.2);margin-top:2.5rem;}
.stat{padding:1.25rem;background:#fff;text-align:center;}
.stat-n{font-family:'Cormorant Garamond',serif;font-size:2rem;font-weight:400;color:var(--deep);display:block;}
.stat-l{font-size:0.68rem;letter-spacing:0.1em;text-transform:uppercase;color:var(--muted);margin-top:0.2rem;display:block;}

.contact-card{border:1px solid rgba(184,147,90,0.25);padding:2.25rem;background:var(--off);}
.cc-head{display:flex;align-items:center;gap:1rem;margin-bottom:1.75rem;padding-bottom:1.5rem;border-bottom:1px solid rgba(184,147,90,0.18);}
.cc-avatar{width:52px;height:52px;border-radius:50%;background:var(--gold);display:flex;align-items:center;justify-content:center;font-family:'Cormorant Garamond',serif;font-size:1.35rem;color:#fff;flex-shrink:0;}
.cc-name{font-family:'Cormorant Garamond',serif;font-size:1.25rem;font-weight:500;color:var(--deep);}
.cc-title{font-size:0.75rem;color:var(--muted);margin-top:0.15rem;}
.contact-row{display:flex;align-items:center;gap:0.75rem;padding:0.75rem 0;border-bottom:1px solid rgba(184,147,90,0.12);}
.contact-row:last-child{border-bottom:none;}
.ci{width:32px;height:32px;border-radius:50%;border:1px solid rgba(184,147,90,0.3);display:flex;align-items:center;justify-content:center;font-size:0.85rem;flex-shrink:0;}
.c-label{font-size:0.68rem;letter-spacing:0.1em;text-transform:uppercase;color:var(--muted);}
.c-val{font-size:0.85rem;color:var(--ink);text-decoration:none;}
.c-val:hover{color:var(--gold);}
.brokerage-badge{margin-top:1.5rem;padding:1rem 1.25rem;background:rgba(184,147,90,0.07);border-radius:2px;font-size:0.78rem;color:var(--muted);line-height:1.6;}
.brokerage-badge strong{color:var(--ink);font-weight:500;}

.dark-section{background:var(--deep);padding:5rem 2.5rem;}
.dark-section .sec-label{color:var(--gold);}
.dark-section .sec-h{color:#fff;}
.dark-section .sec-sub{color:rgba(255,255,255,0.45);}
.for-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:rgba(184,147,90,0.12);}
.for-card{background:rgba(255,255,255,0.03);padding:1.75rem 1.5rem;}
.for-card:hover{background:rgba(184,147,90,0.06);}
.check{width:26px;height:26px;border-radius:50%;border:1px solid rgba(184,147,90,0.35);display:flex;align-items:center;justify-content:center;font-size:0.6rem;color:var(--gold);margin-bottom:1.1rem;}
.for-card h3{font-family:'Cormorant Garamond',serif;font-size:1.1rem;font-weight:500;color:#fff;margin-bottom:0.45rem;}
.for-card p{font-size:0.78rem;color:rgba(255,255,255,0.42);line-height:1.65;font-weight:300;}

.cta-section{padding:5rem 2.5rem;background:var(--cream);text-align:center;}
.cta-inner{max-width:540px;margin:0 auto;}
.cta-section .sec-h{margin-bottom:0.75rem;}
.cta-section p{font-size:0.88rem;color:var(--muted);line-height:1.7;font-weight:300;margin-bottom:2.25rem;}
.cta-row{display:flex;gap:0.75rem;max-width:420px;margin:0 auto;}
.cta-row input{flex:1;padding:0.8rem 1.1rem;border:1px solid rgba(184,147,90,0.3);background:#fff;font-family:'Inter',sans-serif;font-size:0.83rem;color:var(--ink);border-radius:2px;outline:none;}
.cta-row input:focus{border-color:var(--gold);}
.cta-note{font-size:0.7rem;color:var(--muted);margin-top:0.85rem;opacity:0.75;}

footer{background:var(--deep);padding:2rem 2.5rem;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:0.75rem;}
.f-logo{font-family:'Cormorant Garamond',serif;font-size:1.25rem;color:#fff;}
.f-logo span{color:var(--gold);}
footer p{font-size:0.72rem;color:rgba(255,255,255,0.28);}
</style>

<div class="site">
  <h2 style="position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0,0,0,0)">Passport2Property — European property discovery tours with Toronto realtor Karyn Filiatrault</h2>

  <nav>
    <div class="logo">Passport<span>2Property</span></div>
    <div class="nav-r">
      <a href="#">How it works</a>
      <a href="#">Destinations</a>
      <a href="#">About Karyn</a>
      <a href="#" class="nav-btn">Join a tour</a>
    </div>
  </nav>

  <section class="hero">
    <div class="hero-inner">
      <div class="eyebrow"><div class="eline"></div><span class="etxt">European property discovery tours</span></div>
      <h1>Find where you<br><em>belong</em> in Europe.</h1>
      <p>A guided group journey to Spain, Portugal, and Italy — part immersive trip, part property discovery. You explore beautiful places, see real homes, and fall in love. Then Karyn connects you with a trusted local agent to make it real.</p>
      <div class="hero-btns">
        <button class="btn" onclick="sendPrompt('Tell me more about how the Passport2Property tour works')">Explore the experience</button>
        <button class="btn-out" onclick="sendPrompt('What destinations does Passport2Property offer?')">See destinations →</button>
      </div>
      <div class="hero-badges">
        <div class="badge"><div class="bdot"></div>Spain</div>
        <div class="badge"><div class="bdot"></div>Portugal</div>
        <div class="badge"><div class="bdot"></div>Italy</div>
      </div>
    </div>
  </section>

  <section class="section white">
    <p class="sec-label">How it works</p>
    <h2 class="sec-h">A trip that opens a door.</h2>
    <p class="sec-sub">Buying abroad is overwhelming on your own. Karyn handles the logistics so your only job is to discover what feels like home.</p>
    <div class="steps">
      <div class="step"><div class="step-n">01</div><h3>We plan the trip</h3><p>Flights, hotels, group transfers, and curated local experiences — all taken care of for you.</p></div>
      <div class="step"><div class="step-n">02</div><h3>You explore real homes</h3><p>Walk through properties, neighbourhoods, and villages in each destination on your list.</p></div>
      <div class="step"><div class="step-n">03</div><h3>We make the connection</h3><p>When something sparks your interest, Karyn introduces you to a trusted local agent in that region.</p></div>
      <div class="step"><div class="step-n">04</div><h3>Your chapter begins</h3><p>The agent takes it from there. Karyn stays in your corner throughout the process.</p></div>
    </div>
  </section>

  <section class="section cream">
    <p class="sec-label">Current destinations</p>
    <h2 class="sec-h">Three countries. Endless possibilities.</h2>
    <p class="sec-sub">Each tour focuses on regions known for quality of life, accessible property, and a warm welcome to newcomers.</p>
    <div class="dest-row">
      <div class="dest">
        <span class="dest-emoji">🇪🇸</span>
        <h3>Spain</h3>
        <span class="dest-sub">Sun, culture, and remarkable value</span>
        <p>From the Costa del Sol to Andalusia, Spain offers a rich lifestyle at a price that surprises most first-time visitors.</p>
        <div class="tags"><span class="tag">Costa del Sol</span><span class="tag">Barcelona</span><span class="tag">Seville</span></div>
      </div>
      <div class="dest">
        <span class="dest-emoji">🇵🇹</span>
        <h3>Portugal</h3>
        <span class="dest-sub">Europe's best-kept secret</span>
        <p>Low cost of living, warm climate, and one of the safest countries in Europe. Lisbon and the Algarve attract international buyers every year.</p>
        <div class="tags"><span class="tag">Lisbon</span><span class="tag">Porto</span><span class="tag">Algarve</span></div>
      </div>
      <div class="dest">
        <span class="dest-emoji">🇮🇹</span>
        <h3>Italy</h3>
        <span class="dest-sub">La dolce vita, for real</span>
        <p>Tuscany, Sicily, and the lakes are perennial dreams — and closer to reality than most people think.</p>
        <div class="tags"><span class="tag">Tuscany</span><span class="tag">Sicily</span><span class="tag">Lake Como</span></div>
      </div>
    </div>
  </section>

  <section class="section white">
    <p class="sec-label">Your guide</p>
    <h2 class="sec-h">Meet Karyn Filiatrault</h2>
    <div class="about-grid">
      <div class="about-left">
        <p class="about-quote">"Anything but a traditional real estate agent."</p>
        <p class="about-body">Karyn Filiatrault has been one of Toronto's top-producing real estate agents since 2013, consistently ranking in the top 2–3% of TREB agents by sales. Before real estate, she spent years as a documentary producer at the Discovery Channel — and that storytelling instinct is woven into everything she does.</p>
        <p class="about-body">With over $125 million in closed Toronto real estate deals, multiple negotiation expert designations, and a reputation for being straight-talking and deeply human, Karyn brings that same energy to Passport2Property — helping people navigate one of the biggest decisions of their lives without the stiff-suit formality.</p>
        <p class="about-body">When she's not working, you'll find her somewhere in Europe checking off another country on her bucket list. This venture is personal.</p>
        <div class="stats-row">
          <div class="stat"><span class="stat-n">$125M+</span><span class="stat-l">Closed deals</span></div>
          <div class="stat"><span class="stat-n">10+</span><span class="stat-l">Years in real estate</span></div>
          <div class="stat"><span class="stat-n">Top 2%</span><span class="stat-l">TREB agents 2025</span></div>
        </div>
      </div>
      <div class="about-right">
        <div class="contact-card">
          <div class="cc-head">
            <div class="cc-avatar">KF</div>
            <div>
              <div class="cc-name">Karyn Filiatrault</div>
              <div class="cc-title">Real Estate Salesperson · Passport2Property Founder</div>
            </div>
          </div>
          <div class="contact-row">
            <div class="ci">📞</div>
            <div><div class="c-label">Phone</div><a class="c-val" href="tel:4168881844">416-888-1844</a></div>
          </div>
          <div class="contact-row">
            <div class="ci">✉️</div>
            <div><div class="c-label">Email</div><a class="c-val" href="mailto:karyn@homesweetkaryn.com">karyn@homesweetkaryn.com</a></div>
          </div>
          <div class="contact-row">
            <div class="ci">🌐</div>
            <div><div class="c-label">Toronto real estate website</div><a class="c-val" href="https://homesweetkaryn.com" target="_blank">homesweetkaryn.com</a></div>
          </div>
          <div class="contact-row">
            <div class="ci">📍</div>
            <div><div class="c-label">Based in</div><span class="c-val">Downtown Toronto, ON</span></div>
          </div>
          <div class="brokerage-badge">Licensed under <strong>Sage Real Estate Ltd. Brokerage</strong> · Toronto, Ontario. Karyn is an active Toronto realtor and founder of the Passport2Property European discovery tour program.</div>
        </div>
      </div>
    </div>
  </section>

  <section class="dark-section">
    <p class="sec-label">Who this is for</p>
    <h2 class="sec-h">Made for people who've thought about this for years.</h2>
    <p class="sec-sub">You don't need to be ready to buy. You just need to be curious.</p>
    <div class="for-grid">
      <div class="for-card"><div class="check">✓</div><h3>Soon-to-retire dreamers</h3><p>You've pictured a slower, sunnier life in Europe. Now's the time to actually go see it.</p></div>
      <div class="for-card"><div class="check">✓</div><h3>Vacation home seekers</h3><p>A place to escape to every summer. Something to pass on. A base in Europe that's truly yours.</p></div>
      <div class="for-card"><div class="check">✓</div><h3>First-time international buyers</h3><p>Buying abroad can feel daunting. This trip takes the mystery out of the process, step by step.</p></div>
      <div class="for-card"><div class="check">✓</div><h3>The curious and undecided</h3><p>No pressure to buy. This is about finding out where — and whether — you'd want to.</p></div>
    </div>
  </section>

  <section class="cta-section">
    <div class="cta-inner">
      <p class="sec-label">Ready to explore?</p>
      <h2 class="sec-h">Your European chapter<br>starts with one step.</h2>
      <p>Join the interest list and be the first to hear about upcoming tour dates, destinations, and limited group spots.</p>
      <div class="cta-row">
        <input type="email" placeholder="your@email.com" />
        <button class="btn" onclick="sendPrompt('How do I sign up for a Passport2Property tour?')">Join the list →</button>
      </div>
      <p class="cta-note">No spam. Just news about upcoming tours and open spots.</p>
    </div>
  </section>

  <footer>
    <div class="f-logo">Passport<span>2Property</span></div>
    <p>416-888-1844 · karyn@homesweetkaryn.com</p>
    <p>© 2025 Passport2Property · Spain · Portugal · Italy</p>
  </footer>
</div>

