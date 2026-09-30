# Babies & toddlers offering: install guide

## 1. New files: upload as-is

Upload these four files to the root of the repo with "Add files via upload." None of them exist yet, so nothing gets overwritten. All three HTML pages already include the GTM snippet.

- `babies.html`
- `babies-factsheet.html`
- `babies-invitation-worksheet.pdf`: the version the site links to, because it uploads to an AI more reliably on a phone
- `babies-invitation-worksheet.docx`: optional. Keep it as your editable master; the site doesn't link to it.

## 2. Existing pages: paste into the GitHub editor

Open each file on GitHub, click the pencil icon, paste the snippet in the spot described, and commit. Don't replace whole files: your live versions contain edits that aren't in the copies I can see.

### family.html: new section

Paste this directly **above** the line `<div class="service-card">` that begins the **Parent — teen and young adult** card.

```html
  <div class="service-card">
    <h2>Babies and toddlers</h2>
    <p>It's tempting to think babies are unaware of their parents' conflict. They notice far more than we assume. They may not understand our words yet, but they are taking in the tone, the tension, and the rhythm of the household around them.</p>
    <p>And whether this is your first baby or your fifth, a baby widens the small cracks that were already there. Exhausted, overwhelmed parents rarely get the chance to step back and decide, together, who does what and when.</p>
    <p>You don't have to have decided anything about your relationship to talk with me. This isn't couples therapy. It's a practical conversation about the household you're living in right now: who handles nights, how the work gets divided, what happens when you disagree in front of the baby.</p>
    <ul style="margin:0 0 16px; padding-left:20px; font-size:15px; color:#333;">
      <li style="margin-bottom:10px;"><strong>Coaching</strong> for one parent who wants to think things through first</li>
      <li><strong>Mediation</strong> for both parents, to build agreements you can actually live inside</li>
    </ul>
    <p style="font-size:14px; color:#555;">If safety is a concern, let's talk privately first.</p>
    <div class="resource-pair" style="display:grid; grid-template-columns:1fr 1fr; gap:16px; margin:20px 0;">
      <a href="babies-factsheet.html" style="text-decoration:none; display:block; background:var(--grey-bg); border:1px solid #eee; border-radius:10px; padding:16px 18px;">
        <div style="font-size:11px; font-weight:600; letter-spacing:0.08em; text-transform:uppercase; color:var(--teal); margin-bottom:6px;">Fact sheet</div>
        <div style="font-size:14px; color:var(--navy); font-weight:600;">One conversation to start →</div>
      </a>
      <a href="babies-invitation-worksheet.pdf" target="_blank" style="text-decoration:none; display:block; background:var(--grey-bg); border:1px solid #eee; border-radius:10px; padding:16px 18px;">
        <div style="font-size:11px; font-weight:600; letter-spacing:0.08em; text-transform:uppercase; color:var(--teal); margin-bottom:6px;">AI-guided worksheet</div>
        <div style="font-size:14px; color:var(--navy); font-weight:600;">Inviting the other parent →</div>
      </a>
    </div>
    <div class="card-cta">
      <a href="babies.html" class="cta-btn cta-secondary">More on working with families of babies and toddlers</a>
      <a href="https://calendly.com/mediatorlaura/free-15-minute-getting-started-call" target="_blank" class="cta-btn cta-primary">Book a free 15-minute call</a>
    </div>
  </div>

```

### Co-parenting and divorce-status pages: one line

Paste on `we-arent-sure.html` (the "Divorce + co-parenting" entry page). Add it to any status page where a parent with a baby might land, such as `we-are-separated.html`. Put it near the top of the main content, just after the opening paragraphs.

```html
<div style="max-width:680px; margin:20px auto; padding:14px 20px; background:white; border:1px solid #eee; border-left:3px solid var(--teal); border-radius:8px; font-size:15px;">
  <strong>Separating with a baby or toddler?</strong> Young children need a different kind of plan. <a href="babies.html" style="color:var(--teal);">Here's how I help →</a>
</div>
```

### attorneys.html: referral line

Paste wherever the page lists the kinds of cases or situations you take on.

```html
<p><strong>Cases involving children under three.</strong> With a background in infant-toddler development and a PITC Fellowship, I can step in for the parenting plan piece alone, building a schedule and shared routines that fit how very young children attach, sleep, and handle transitions. <a href="babies.html" style="color:var(--teal);">More on this work →</a></p>
```

### courses.html: two new cards

The easiest safe method in the GitHub editor:

1. Find the line **More courses will be listed here as they're scheduled.** Directly above it, add this heading:
   ```html
   <h2>For expecting families</h2>
   ```
   If your other section heading ("Current courses") uses a class, copy that line exactly and change only the words.
2. Copy the entire **Personal Stress and Anxiety** card, from its opening `<div` to its closing `</div>`. Paste it twice below the new heading.
3. In each copy, replace the text and links with the following. Delete the "Enrolled? Access course materials" link, since neither class has a materials page.

**Card 1**
- Title: `Five Conversations Before Baby`
- Detail line: `<strong>Audience:</strong> Expecting couples · <strong>Format:</strong> Five small-group sessions`
- Description:
  > Most couples spend months preparing the nursery and very little time preparing for the decisions they'll face at 3 a.m. This class is five conversations you'll be glad you had before the baby arrives. We start with how each of you communicates, and how to have a hard conversation without it turning into a fight. The class then chooses the next three topics together: sleep, feeding, circumcision, how you'll divide the work, or whatever matters most to the couples in the room. Before each session, you'll get materials to help you think through where you stand, so you arrive ready to talk rather than react. Each session mixes short teaching, time with your partner, and small-group conversations with other expecting parents, so you leave with connections as well as a plan. The last conversation pulls it all together: a plan for what you'll do when you disagree, and for what happens when your baby doesn't follow the plan. *Grandparents-to-be: see Preparing to Be Grandparents below.*
- Offered line: `Offered by inquiry, for small groups. Online or in person.`
- Button text: `Ask about upcoming sessions →`
- Button link: `mailto:Laura@GradientResolutions.com?subject=Five%20Conversations%20Before%20Baby`

**Card 2**
- Title: `Preparing to Be Grandparents`
- Detail line: `<strong>Audience:</strong> Grandparents-to-be · <strong>Format:</strong> One two-hour session`
- Description:
  > You've raised a family, and you have a lifetime of experience to offer. The hard part is offering it in a way your children can take in. Stories and advice come from love, but when they arrive first, they can put up walls before the real conversation even starts. This class is about becoming a partner to your adult children, so that when the baby arrives, everyone is ready to work together. You'll learn how to follow your children's lead, so that when they do need your help, they're ready to hear it; how to ask questions that serve them, so your help goes where it's actually needed; and how to listen and connect in the moment, so your timing lands well. *Your children can take Five Conversations Before Baby.*
- Offered line: `Offered by inquiry, for small groups. Online or in person.`
- Button text: `Ask about upcoming sessions →`
- Button link: `mailto:Laura@GradientResolutions.com?subject=Preparing%20to%20Be%20Grandparents`

## 3. Check before you publish

- **babies.html FAQ:** confirm "Master Infant-Toddler Teacher credentials" and "Before returning to mediation" are accurate. I changed "hundreds of families" to "many families."
- **Hotline numbers:** call or check each one once.
- **After uploading:** open babies.html on your phone. Tap a few FAQ questions to make sure they expand, and tap "Book a free 15-minute call" to confirm it opens the new Calendly page.
