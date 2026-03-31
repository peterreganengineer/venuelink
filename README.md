# VenueLink

> **Connecting event promoters with venues through rich, detailed profiles**

VenueLink is a marketplace platform that eliminates the back-and-forth friction between music event promoters and venue owners. By using a LinkedIn/Tinder-style profile model, both parties can see everything they need in one view to make confident booking decisions.

## Overview

The platform solves a critical pain point in the live music industry: promoters waste hours sending cold emails that get ghosted, while venues drown in unqualified inquiries. VenueLink creates transparency, accountability, and efficiency through:

- **Rich Profiles**: Complete promoter and venue information collected once, used forever
- **Application System**: $3 application fee (Groover model) ensures serious inquiries
- **Guaranteed Responses**: 7-day response guarantee or automatic refund
- **Feedback Loop**: Constructive feedback on declined applications helps promoters improve
- **Real-time Availability**: Venues manage calendars, promoters see what's actually available

## Features

### For Promoters
- Browse hundreds of verified venues with detailed specs
- See complete equipment lists, past events, and real-time availability
- Apply with rich profiles including artist lineups, social links, and past event photos
- Track application status with Domino's-style progress tracking
- Get actionable feedback when declined
- One profile, unlimited applications

### For Venues
- Receive comprehensive applications showing complete promoter profiles
- See artist lineups with photos, Spotify links, Instagram handles, and follower counts
- Make decisions in minutes instead of weeks of email tennis
- Manage availability calendar
- Accept or decline with optional feedback
- Build reputation through ratings and reviews

## Tech Stack

### Frontend
- Pure HTML5/CSS3 (no framework dependencies)
- Google Fonts: Space Grotesk (headings) + Inter (body)
- Responsive design with CSS Grid and Flexbox
- Dark theme optimized for nightlife industry

### Backend (To Be Built)
- Node.js + Express
- PostgreSQL database
- JWT authentication
- Stripe for payments
- SendGrid/Mailgun for email notifications
- AWS S3 or Cloudflare R2 for media storage

## Design System

### Color Palette
```css
--black: #0a0a0a           /* Main background */
--dark-bg: #121212         /* Card backgrounds */
--dark-card: #1a1a1a       /* Nested cards */
--blue-dark: #0f172a       /* Gradient start */
--blue-mid: #1e3a8a        /* Gradient mid/end */
--yellow: #fbbf24          /* Primary accent */
--yellow-bright: #fcd34d   /* Hover states */
--text-primary: #ffffff    /* Main text */
--text-secondary: #a1a1aa  /* Secondary text */
--border: #27272a          /* Borders */
```

### Typography
- **Headings**: Space Grotesk, 700 weight, -0.03em to -0.05em letter spacing
- **Body**: Inter, 400 weight, -0.01em letter spacing

## Project Structure

```
venuelink-build/
├── README.md                          # This file
├── BUILD_SUMMARY.md                   # Technical build notes
├── HANDOFF_DOCUMENT.md                # Detailed feature documentation
│
├── landing-redesign.html              # ✅ Homepage with hero, features, pricing
├── marketplace-redesign.html          # ✅ Browse venues with filters
├── venue-profile-redesign.html        # ✅ Individual venue details
├── venue-intake-form.html             # 🔨 Venue onboarding (needs redesign)
├── dashboard-redesign.html            # ✅ Venue dashboard (STAR FEATURE)
├── promoter-profile-page.html         # ✅ Promoter profile view
├── promoter-profile-builder.html      # ✅ Promoter onboarding wizard
├── promoter-intake-form.html          # 🔨 Alternative onboarding (needs redesign)
├── widget-redesign.html               # ✅ Embeddable booking widget
└── signup-page.html                   # ✅ Account creation

Legend: ✅ Complete | 🔨 Needs work
```

## Completed Pages (8/13)

### 1. Landing Page
- Dark blue gradient hero with value proposition
- Top venues recommendation cards (Groover-style)
- Features grid, stats bar, pricing section
- Professional typography and hover effects

### 2. Marketplace
- Search and filter venues by location, capacity, genre, equipment
- Responsive venue card grid with quick stats
- Sort options: recommended, highest rated, fastest response
- 106 sample venues with detailed information

### 3. Venue Dashboard (THE KILLER FEATURE)
Rich application cards showing:
- Complete promoter profile with avatar, rating, verification
- Quick stats: events hosted, total attendees, social followers, email list
- Event details: name, date, attendance, ticket price, genre
- **Artist lineup with photos, Spotify/Instagram/SoundCloud links**
- Past 3 events with photos
- Marketing strategy and social proof
- One-click Accept/Decline with feedback modal

### 4. Venue Profile Page
What promoters see before applying:
- Venue specs: capacity, square footage, hours, parking
- Equipment breakdown: sound system, DJ gear, lighting, amenities
- Past events with promoter attribution
- Availability calendar
- Sticky apply sidebar with response stats

### 5. Promoter Profile Builder
4-step onboarding wizard:
- **Step 1**: Basic info, genres, avg attendance, preferred days/times
- **Step 2**: Past events with detailed artist lineups (photos, social links)
- **Step 3**: Audience reach, social followers, marketing strategy
- **Step 4**: Media uploads, social profiles, venue references

### 6. Promoter Profile Page
What venues see:
- Hero with avatar, name, location, genres, rating
- Key stats grid: events, attendees, followers, email subscribers
- Past events showcase with images and attendance
- Marketing and audience reach details
- Social media presence with follower counts
- Venue testimonials

### 7. Embeddable Widget
Resy-inspired compact widget for venue websites:
- 3 tabs: Availability, Apply, Venue Info
- Interactive calendar showing open dates
- Quick application form
- Shows venue specs
- Easy embed code (5-line script)

### 8. Signup Page
- Role selector toggle: Event Promoter vs Venue Owner
- Minimal friction signup form
- Social login options (Google, Facebook)
- Redirects to appropriate profile builder

## Pages Still Needed

### High Priority
1. **Application Form** - Multi-step form for promoters to apply to venues
2. **Status Tracker** - Domino's-style progress bar for applications
3. **Messaging Interface** - Chat/email thread between venues and promoters
4. **Calendar Management** - Venue availability management system

### Medium Priority
5. **Browse Promoters** - Reverse marketplace for venues to discover promoters
6. **Notifications Center** - Centralized notification hub

### Polish
7. **Venue Intake Form Redesign** - Apply dark theme to existing detailed form
8. **Promoter Intake Form Redesign** - Visual refresh for consistency
9. **Settings Page** - Account, billing, notification preferences
10. **Welcome Tour** - First-time user onboarding

## Key Innovations

### 1. Profile-First Model
All information collected once during onboarding, then reused for every application. No repetitive form-filling.

### 2. Artist Lineup Detail
Unlike competitors, VenueLink captures complete artist information:
- Professional photos
- Spotify profiles (venues can preview music)
- Instagram handles (venues can check following/engagement)
- SoundCloud links, websites
- Notable achievements, label affiliations

### 3. Rich Application Cards
Venues see everything they need in one view:
- Who the promoter is (stats, rating, past events)
- What the event is (details, lineup, marketing plan)
- Social proof (follower counts, past attendance, testimonials)

No more "Can you send more info?" email chains.

### 4. Feedback System
When declining applications, venues provide constructive feedback:
- Pre-defined checkboxes (date conflict, genre mismatch, capacity issues)
- Optional text field for detailed feedback
- Helps promoters improve future applications
- Builds higher quality ecosystem

### 5. Guaranteed Response
7-day response guarantee with automatic refund creates accountability and reduces ghosting anxiety.

## Monetization Strategy

- **$3 per application** (Groover model - proven to work)
- **Pro Plan**: $49/mo for unlimited applications (promoters)
- **Venue Plan**: $79/mo to receive unlimited applications (venues)
- **Future**: Take rate on ticket sales, featured listings

## Value Propositions

### For Venues
> "Stop wasting hours on email back-and-forth. See complete promoter profiles with past events, social reach, and marketing plans in one click. Accept or decline in 30 seconds."

**Benefits**:
- Save hours per application
- Make confident decisions with full context
- Fill calendar faster with quality events
- Build reputation through ratings

### For Promoters
> "Never get ghosted again. Guaranteed response in 7 days or your $3 back. See real-time availability and all venue specs before you apply. One profile, unlimited applications."

**Benefits**:
- Guaranteed responses (no more ghosting)
- See real availability upfront
- Know exact venue equipment before applying
- Get actionable feedback to improve
- One-time profile setup, infinite applications

## Next Steps for Development

### Phase 1: Backend (10-15 hours)
- Set up Node.js + Express server
- PostgreSQL database with tables: users, venues, promoters, applications, availability
- JWT authentication
- API endpoints for CRUD operations
- File upload integration (AWS S3 / Cloudflare R2)

### Phase 2: Payments & Email (5-8 hours)
- Stripe integration for $3 application fees
- Subscription billing for Pro/Venue plans
- Email notifications via SendGrid/Mailgun
- Refund logic for 7-day guarantee

### Phase 3: Complete Remaining Pages (8-12 hours)
- Build application form
- Build status tracker
- Build messaging interface
- Build calendar management
- Redesign intake forms

### Phase 4: Deploy (2-3 hours)
- Deploy backend to Railway/Render/Heroku
- Deploy frontend to Vercel/Netlify
- Configure domain and SSL
- Set up environment variables

### Phase 5: Beta Testing
- Launch with 5 venues + 10 promoters in NYC house/techno scene
- Gather feedback and iterate
- Refine UX based on real usage
- Expand to full NYC market, then other cities/genres

## Estimated Timeline

**With developer support:**
- Backend setup: 2 weeks
- Payment/email integration: 1 week
- Complete remaining pages: 1-2 weeks
- Deploy + polish: 1 week
- **Total: 4-6 weeks to live product**

## Running Locally

Currently, the project consists of static HTML files. To view:

```bash
# Option 1: Open files directly in browser
open landing-redesign.html

# Option 2: Use a local server
python3 -m http.server 8000
# Then visit http://localhost:8000

# Option 3: Use VS Code Live Server extension
# Right-click any HTML file → "Open with Live Server"
```

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (responsive design)

## Credits

**Built by**: Claude  
**For**: Peter Regan  
**Date**: March 2026  
**Industry**: Live Music / Event Production  
**Inspiration**: Groover (music submission platform), Beatport (design aesthetic), LinkedIn (profile model)

## License

All rights reserved. This is a proprietary project.

---

## Contact

For questions about this build or to continue development, refer to the detailed documentation in [HANDOFF_DOCUMENT.md](HANDOFF_DOCUMENT.md) and [BUILD_SUMMARY.md](BUILD_SUMMARY.md).
