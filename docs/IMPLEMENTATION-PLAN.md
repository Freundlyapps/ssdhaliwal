# Implementation Plan: ssdhaliwal.dev Portfolio Website
**For**: Sarabjit Singh Dhaliwal | No-Code/Low-Code AI Developer
**Timeline**: 5 Days (Full Build) + Ongoing Maintenance
**Platform**: Webflow (Primary) + Integrations

---

## Executive Summary

This plan converts your RAW-PLAN.md into actionable implementation steps. The website positions you as a versatile AI builder for content creators and SMBs, with live project demos, service offerings, and tech partnership positioning (Facebook API, LinkedIn integration expertise).

**Primary Goal**: Convert visitors into consultations, partnerships, or beta users
**Success Metric**: 50%+ conversion rate on primary CTAs

---

## Phase 1: Foundation & Setup (Day 1)

### 1.1 Account & Domain Setup
| Task | Action | Owner | Status |
|------|--------|-------|--------|
| Webflow Account | Create/upgrade to Workspace plan ($23/month) | Sarabjit | ⬜ Pending |
| Domain Purchase | Buy ssdhaliwal.dev via Namecheap/GoDaddy | Sarabjit | ⬜ Pending |
| Domain Connect | Connect domain to Webflow hosting | Sarabjit | ⬜ Pending |
| Email Setup | Create hello@ssdhaliwal.dev (Google Workspace) | Sarabjit | ⬜ Pending |

### 1.2 Tool Integration Setup
| Tool | Purpose | Setup Action |
|------|---------|--------------|
| Google Analytics | Traffic tracking | Create GA4 property, add tracking code |
| Google Tag Manager | Tag management | Create container, add to Webflow |
| Calendly | Booking consultations | Create "Free Audit" event type |
| Typeform | Contact form (optional) | Create form or use Webflow native |
| Mailchimp | Newsletter capture | Create audience, embed form |

### 1.3 Design System Configuration
Create in Webflow Project Settings:
```
Color Variables:
  --primary: #007BFF (Trust Blue)
  --primary-dark: #006FE6
  --accent: #FF9500 (Creative Orange)
  --accent-dark: #E68600
  --bg-light: #FFFFFF
  --bg-dark: #121212
  --text-light: #1A1A1A
  --text-dark: #E0E0E0
  --neutral-light: #E0E0E0
  --neutral-dark: #333333

Typography:
  --font-heading: Inter (48px H1, 32px H2, 24px H3)
  --font-body: Inter (16px body, 12px meta)
  --font-mono: JetBrains Mono (code snippets)

Spacing:
  --section-padding: 32px
  --container-max: 1200px
  --border-radius: 12px

Transitions:
  --hover-scale: scale(1.02)
  --hover-duration: 0.3s ease
```

---

## Phase 2: Content Preparation (Day 1-2)

### 2.1 Copywriting Requirements

#### Hero Section Content
```
Tagline: "No-Code/Low-Code AI Expert: Building Custom SaaS & Tools for Content Creators and SMBs—from Scratch"

Sub-headline: "I solve real creator pains like content fatigue and image workflows. Creator of open-source PicShifter (10K+ users) and beta Writola."

CTA Buttons:
- Primary: "Explore Portfolio" (anchor scroll)
- Secondary: "Book Free Audit" (Calendly modal)
```

#### About Section (300 words)
Key points to cover:
1. **Your Journey**: From SMB automations to creator-focused tools
2. **Technical Skills**: Bubble, Webflow, Zapier, OpenAI API, Make.com
3. **Specializations**: AI video generation, content pipelines, workflow automation
4. **Philosophy**: "I build scalable, issue-solving apps without code bloat"
5. **Tech Partnerships**: Mention Facebook API Auth expertise, LinkedIn integrations

#### Services Section Pricing Table
| Service | Description | Deliverables | Price |
|---------|-------------|--------------|-------|
| Custom SaaS Builds | AI-integrated apps from scratch | MVP, user auth, payment integration, documentation | $2,000+ |
| Website Development | No-code sites with tool embeds | Responsive site, CMS, SEO, contact forms | $1,000–3,000 |
| AI Problem-Solving | Custom prototypes & automations | Working prototype, documentation, handoff | $100/hour |
| Tech Integration | APIs: Facebook, LinkedIn, OpenAI | Auth setup, data sync, workflow automation | $500–1,500 |
| Open-Source Consulting | Audits & scaling advice | Analysis report, implementation roadmap | Free Intro |

#### Portfolio Projects (Prepare content for each)
1. **PicShifter.com**
   - Tagline: "Open-source image optimizer—privacy-first"
   - Problem solved: Creator time-wasters with bulk image editing
   - Impact: 10,000+ uses, 500+ GitHub stars
   - Tech stack: Bubble, API integrations
   - Live demo: Embed iframe
   - Links: GitHub, Live Site

2. **PDFtoImage.PicShifter.com**
   - Tagline: "Free drag-drop PDF converter"
   - Use case: Quick thumbnails, newsletter prep
   - Features: No registration, instant processing
   - Embed tool directly

3. **Writola.com**
   - Tagline: "Beta AI SaaS for writing & SEO publishing"
   - Problem: Content creation time reduced 70%
   - Status: Beta - accepting testers
   - CTA: "Join Beta Waitlist"

4. **AI Video Generation App**
   - Tagline: "Script-to-short videos, automated"
   - Status: In development
   - Teaser: Screenshot preview
   - CTA: "Get Early Access"

### 2.2 Assets Checklist
| Asset | Specs | Needed |
|-------|-------|--------|
| Headshot Photo | Circular, 500x500px min | ⬜ Yes |
| Project Screenshots | 1200x800px, 3-4 per project | ⬜ Yes |
| Project Logos | 200x200px PNG with transparency | ⬜ Yes |
| GitHub Stars Count | Current stats | ⬜ Yes |
| Testimonial Quotes | 4-6 with names/photos | ⬜ Yes |

---

## Phase 3: Webflow Build (Day 2-3)

### 3.1 Site Structure
```
ssdhaliwal.dev/
├── Hero (80vh)
├── About (600px)
├── Services (800px)
├── Portfolio (1,200px)
├── Testimonials (400px)
├── Blog/Resources (600px)
├── Contact (300px)
└── Footer
```

### 3.2 Build Sequence
1. **Setup Navigation**
   - Sticky header with logo
   - Nav links: Home, About, Services, Portfolio, Blog, Contact
   - Dark/Light mode toggle (top-right)
   - Mobile hamburger menu

2. **Build Hero Section**
   - Full-screen gradient background (#007BFF → #FF9500)
   - Two-column layout (photo left, text right)
   - Mobile: Stacked vertically
   - Animations: Fade-in on load

3. **Build About Section**
   - Two-column grid
   - Skills icons with tooltips
   - Tech partnership badges (Facebook, LinkedIn, OpenAI)

4. **Build Services Section**
   - 3-column card grid
   - Hover effects: Scale 1.02, shadow increase
   - Modal popups for detailed pricing
   - CTA: "Get Quote" per service

5. **Build Portfolio Section**
   - Masonry grid layout
   - Project cards with screenshots
   - Live demo embeds (iframes)
   - "View Project" buttons with lightbox

6. **Build Testimonials**
   - Carousel/slider component
   - Auto-scroll with manual controls
   - Star ratings

7. **Build Contact Section**
   - Form: Name, Email, Subject, Message
   - Social links: LinkedIn, X/Twitter, GitHub
   - Direct email: hello@ssdhaliwal.dev

### 3.3 Dark/Light Mode Implementation

Add to Webflow Project Settings > Custom Code:

```html
<!-- In <head> -->
<style>
  :root {
    --bg: #FFFFFF;
    --text: #1A1A1A;
    --primary: #007BFF;
    --accent: #FF9500;
    --neutral: #E0E0E0;
  }

  .dark-mode {
    --bg: #121212;
    --text: #E0E0E0;
    --primary: #4DA6FF;
    --accent: #FFB74D;
    --neutral: #333333;
  }

  body {
    background: var(--bg);
    color: var(--text);
    transition: background 0.3s ease, color 0.3s ease;
  }

  .theme-toggle {
    position: fixed;
    top: 20px;
    right: 20px;
    z-index: 1000;
  }
</style>
```

```html
<!-- Before </body> -->
<script>
  // Theme Switcher
  (function() {
    const toggle = document.querySelector('[data-theme-toggle]');
    const html = document.documentElement;

    // Check localStorage or system preference
    const savedTheme = localStorage.getItem('theme');
    const systemDark = window.matchMedia('(prefers-color-scheme: dark)').matches;

    if (savedTheme === 'dark' || (!savedTheme && systemDark)) {
      html.classList.add('dark-mode');
    }

    // Toggle handler
    toggle?.addEventListener('click', () => {
      html.classList.toggle('dark-mode');
      localStorage.setItem('theme',
        html.classList.contains('dark-mode') ? 'dark' : 'light'
      );
    });
  })();
</script>
```

---

## Phase 4: Integrations & Features (Day 3)

### 4.1 Calendly Integration
```
Embed Type: Inline embed or Popup modal
Event Type: "Free 30-Minute Audit"
Questions to ask:
- What's your main challenge?
- What type of project?
- Timeline?
```

### 4.2 Google Analytics Setup
```
Events to Track:
- CTA clicks (scroll_to_portfolio, book_audit, contact_form)
- Project demo views
- Dark/light mode toggle
- External link clicks (GitHub, live projects)

Conversions:
- Form submissions
- Calendly bookings
- Beta signups
```

### 4.3 Live Demo Embeds
```
PicShifter: <iframe src="https://picshifter.com/demo" width="100%" height="400px"></iframe>
PDFtoImage: <iframe src="https://pdetoimage.picshifter.com" width="100%" height="400px"></iframe>

Note: Ensure embeds support theme switching via URL params or postMessage
```

### 4.4 Social Proof Integration
```
GitHub Stats:
- Link to github.com/ssdhaliwal
- Display: Repos, Stars, Followers

LinkedIn:
- Profile badge embed
- "Open to Work" indicator

Twitter/X:
- Follow button
- Recent tweets embed (optional)
```

---

## Phase 5: Tech Partnership Positioning (Day 3-4)

### 5.1 Partnership Showcase Section
Add dedicated section or integrate into About/Services:

```
Title: "Trusted Tech Partners"
Layout: Logo grid with tooltips

Partners to Highlight:
- Facebook: "Meta API Integration Expert - Auth, Graph API, Messenger"
- LinkedIn: "LinkedIn API Specialist - Profile sync, Share automation"
- OpenAI: "GPT-4 Integration - Custom AI workflows"
- Bubble: "Certified Bubble Developer"
- Webflow: "Expert Partner"

CTA: "Discuss Integration Project"
```

### 5.2 Integration Case Studies
Create mini-case studies for portfolio:
1. "Facebook API Auth for SaaS" - How you implemented OAuth
2. "LinkedIn Auto-Share for Writola" - Content distribution automation
3. "OpenAI API for Content Generation" - Custom prompts & workflows

---

## Phase 6: Testing & Optimization (Day 4)

### 6.1 Performance Checklist
| Check | Target | Tool |
|-------|--------|------|
| Page Load Speed | <2 seconds | Google PageSpeed Insights |
| Lighthouse Score | >90 | Chrome DevTools |
| Mobile Responsiveness | All breakpoints | Webflow Preview |
| Cross-Browser | Chrome, Safari, Firefox | Manual testing |
| Dark Mode Toggle | Works & persists | Manual testing |

### 6.2 Accessibility Testing
| Check | Target | Tool |
|-------|--------|------|
| Color Contrast | WCAG AA 4.5:1 | WebAIM Contrast Checker |
| Alt Text | All images | Lighthouse |
| Keyboard Navigation | Tab through all elements | Manual |
| Screen Reader | VoiceOver/NVDA compatible | Manual |
| ARIA Labels | All interactive elements | Lighthouse |

### 6.3 SEO Checklist
```
On-Page SEO:
- Title tag: "No-Code AI Developer | Tools for Creators & SMBs | Sarabjit Dhaliwal"
- Meta description: "Custom AI SaaS & tools for content creators. Creator of PicShifter, Writola. Facebook & LinkedIn API expert. Book free audit."
- Open Graph images: 1200x630px
- Twitter Card: Summary with large image
- Structured data: Person schema

Sitemap:
- Submit to Google Search Console
- Submit to Bing Webmaster Tools
```

### 6.4 Form & Conversion Testing
```
Test Scenarios:
- Form submission → Email received
- Calendly modal → Booking flow works
- Dark mode toggle → Persists on reload
- Mobile menu → All links work
- Project demos → Iframes load correctly
```

---

## Phase 7: Launch & Promotion (Day 5)

### 7.1 Pre-Launch Checklist
```
□ Domain propagation complete
□ SSL certificate active
□ All forms tested & working
□ Analytics tracking verified
□ Dark/light mode working
□ Mobile responsive on all devices
□ Social meta tags working
□ Calendly integrated
□ Newsletter form connected
```

### 7.2 Launch Announcement Template

**LinkedIn Post:**
```
🚀 Excited to launch my new portfolio: ssdhaliwal.dev

As a no-code/low-code AI developer, I've been busy building tools for content creators:
- PicShifter (10K+ users, open-source)
- Writola (AI writing SaaS, beta)
- PDFtoImage (free converter)

Specialties: Facebook API, LinkedIn integrations, OpenAI workflows

Open to:
🤝 Custom SaaS projects
🔧 Tool development
📊 Tech partnerships

Check it out and let me know what you think!

#NoCode #AI #SaaS #WebDevelopment
```

**Twitter/X Post:**
```
Just shipped my portfolio 🚀

ssdhaliwal.dev

I build AI tools for creators:
→ PicShifter (image optimizer)
→ Writola (AI writing SaaS)
→ + more in the works

Specialties: Facebook/LinkedIn APIs, Bubble, Webflow

Open for partnerships & projects 👇
```

### 7.3 Post-Launch Tasks
```
Week 1:
- Monitor analytics daily
- Fix any bugs reported
- Share on 3-4 platforms
- Send to existing network

Week 2-4:
- Add first blog post
- A/B test CTAs
- Gather feedback
- Update based on data

Ongoing (Monthly):
- Add new projects
- Publish blog content
- Review analytics
- Update testimonials
```

---

## Phase 8: Maintenance & Growth

### 8.1 Content Calendar
```
Week 1: Launch announcement
Week 2: "How I Built PicShifter" blog post
Week 3: "AI Tools for Content Creators" guide
Week 4: "Facebook API Integration Tips" article
Month 2: Case studies, project updates
```

### 8.2 Optimization Loop
```
Monthly Review:
1. Check Google Analytics for top pages
2. Identify drop-off points
3. A/B test weaker CTAs
4. Add requested features
5. Update portfolio with new work

Quarterly:
- Full site audit
- Refresh outdated content
- Add new testimonials
- Review pricing
- SEO keyword research
```

### 8.3 Growth Roadmap
```
Month 1-3: Foundation
- Launch & optimize
- Build initial traffic (LinkedIn, Twitter)
- Collect 5+ testimonials

Month 4-6: Authority Building
- Publish 10+ blog posts
- Guest posts on dev communities
- Podcast appearances

Month 7-12: Scaling
- Premium service offerings
- Online course / templates
- Affiliate partnerships
- Hire support for overflow
```

---

## Appendix: Quick Reference

### File Structure
```
project/
├── IMPLEMENTATION-PLAN.md (this file)
├── RAW-PLAN.md
├── assets/
│   ├── headshot.jpg
│   ├── screenshots/
│   └── logos/
├── content/
│   ├── copy.docx
│   └── testimonials.json
└── launch/
    ├── announcement-templates.md
    └── social-links.txt
```

### Key Contact Points
- Primary Email: hello@ssdhaliwal.dev
- Calendly: [Link when created]
- LinkedIn: [Profile URL]
- GitHub: [Profile URL]
- Twitter/X: [Profile URL]

### Budget Summary
| Item | Cost | Frequency |
|------|------|-----------|
| Domain (ssdhaliwal.dev) | $15 | Yearly |
| Webflow Workspace | $23 | Monthly |
| Google Workspace | $6 | Monthly |
| Calendly Premium | $0-16 | Monthly |
| **Total Monthly** | **$29-45** | |
| **First Year** | **~$500** | |

---

## Next Steps

1. ✅ Review this implementation plan
2. ⬜ Approve or request modifications
3. ⬜ Begin Phase 1: Foundation & Setup
4. ⬜ Prepare assets and content
5. ⬜ Schedule build days

---

**Document Version**: 1.0
**Last Updated**: 2025-12-27
**Status**: Ready for Review
