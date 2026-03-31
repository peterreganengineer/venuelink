# VenueLink - Complete Handoff Document
**Last Updated:** March 8, 2026
**Status:** 8 pages complete, 5 pages in progress, ready to continue

---

## 📦 WHAT'S BEEN BUILT (Ready for Peter)

### **1. Landing Page** (`landing-redesign.html`)
**Status:** ✅ Complete
**Features:**
- Dark theme with blue gradient hero
- Yellow accent CTAs
- Space Grotesk typography throughout
- Hero section with value prop
- "Top Venues For You" recommendation cards (Groover-style)
- Stats bar (venues, events, response rate)
- Features grid (3 columns)
- Pricing section
- Footer

**Design Notes:**
- Uses the full design system (see Design Tokens below)
- Beatport-inspired dark aesthetic
- Responsive grid layouts

---

### **2. Marketplace** (`marketplace-redesign.html`)
**Status:** ✅ Complete
**Features:**
- Search bar in hero section
- Left sidebar with filters:
  - Location checkboxes (Brooklyn, Manhattan, Queens, Bronx)
  - Capacity slider (50-1000+)
  - Genre checkboxes (House, Techno, Hip-Hop, Rock)
  - Equipment filters (CDJ-3000s, Pro Sound, Full Bar, Security)
  - Availability filters
  - "Clear All Filters" button
- Venue card grid (responsive, auto-fill)
- Each card shows:
  - Verified badge
  - Quick stats (capacity, response rate)
  - Venue name, location, rating
  - Genre tags
  - Description
  - Specs grid (equipment, bar, hours, security)
  - Apply price ($3)
- Sort dropdown (Recommended, Highest Rated, Fastest Response, Newest, Capacity)
- Results count display

**Design Notes:**
- Sticky sidebar on desktop
- Cards have yellow hover glow effect
- Clean, scannable layout

---

### **3. Venue Dashboard** (`dashboard-redesign.html`) ⭐ **THE STAR**
**Status:** ✅ Complete + Enhanced
**Features:**
- Top navigation with notifications bell (badge count)
- Left sidebar with:
  - Applications (with count badge)
  - Accepted
  - Calendar
  - Messages (with badge)
  - My Profile
  - Analytics
  - Settings
- Filter tabs (All, New, Under Review)
- **Rich Application Cards** showing:
  - Promoter avatar, name, location, rating, verification
  - NEW badge for fresh applications
  - Quick stats grid (4 columns):
    - Events Hosted
    - Total Attendees
    - Instagram Followers
    - Email List Size
  - Event details grid:
    - Event name, date, attendance, ticket price, genre, time
  - **Proposed Lineup Section** (NEW):
    - Artist cards with photos
    - Headliner highlighted in yellow
    - Support and opener cards
    - Each artist shows:
      - Photo (80x80px)
      - Name, location, follower counts
      - Clickable social links (Spotify, Instagram, SoundCloud)
      - Notable info (labels, achievements)
  - Event description
  - Past 3 events with photos
  - Marketing strategy with social proof badges
  - Application fee and timestamp
  - Action buttons:
    - View Full Profile
    - Decline (opens feedback modal)
    - Accept Application
- **Feedback Modal** (when declining):
  - Checkbox reasons:
    - Date not available
    - Doesn't match vibe/genre
    - Capacity mismatch
    - Concerns about past events
    - Price point doesn't work
    - Other
  - Optional text field for additional feedback
  - Helper text encouraging constructive feedback
  - Shows promoter name in header
  - Cancel / Send Decline buttons

**Design Notes:**
- This is the CORE VALUE PROP of the product
- Everything a venue needs in ONE view
- Zero back-and-forth required
- Artist details with photos/socials are critical for decision-making

---

### **4. Venue Profile Page** (`venue-profile-redesign.html`)
**Status:** ✅ Complete
**Features:**
- Hero section with:
  - Venue logo/avatar
  - Name, location, rating
  - Verified badge
  - Genre tags (House, Techno, Late Night, Full Bar, CDJ-3000s)
- Sticky apply sidebar with:
  - Price ($3)
  - Apply button
  - Save button
  - Stats box (response rate, avg time, events booked, rating)
- About section with description
- Photo gallery (hero image + 3 smaller)
- Venue specifications grid:
  - Capacity, square footage, stage size, load-in, hours, parking
- Equipment & Amenities by category:
  - Sound System (main speakers, subs)
  - DJ Equipment (CDJs, mixer)
  - Lighting & Visual (LED, lasers, haze)
  - Amenities (bar, security, recording, coat check)
- Past events list with promoter attribution
- Availability calendar widget (monthly view)

**Design Notes:**
- 2-column layout (main content + sticky sidebar)
- Equipment shown with icons and detailed specs
- Calendar shows available/booked dates

---

### **5. Embeddable Widget** (`widget-redesign.html`)
**Status:** ✅ Complete
**Features:**
- Example venue website showing widget integration
- Widget has 3 tabs:
  - **Availability:** Interactive calendar, legend, CTA to apply
  - **Apply:** Quick application form (name, email, phone, group name, date, attendance, description)
  - **Venue Info:** Specs grid (capacity, hours, equipment, etc.)
- Shows "Powered by VenueLink" branding
- Compact design (not full page takeover)
- Dark theme matches platform
- Integration code section shows:
  - Copy/paste embed code
  - Simple 5-line script
  - Configuration options (venueId, theme, accentColor)

**Design Notes:**
- Resy-inspired compact widget
- Fits naturally on venue's existing website
- Tab switching works smoothly
- Clicking available date auto-switches to apply tab

---

### **6. Signup Page** (`signup-page.html`)
**Status:** ✅ Complete
**Features:**
- Role selector (Event Promoter vs Venue Owner toggle)
- Form fields:
  - Full name
  - Email
  - Phone number
  - Password
  - Terms checkbox
- Social login options:
  - Continue with Google
  - Continue with Facebook
- "Already have account? Log in" link
- On submit, redirects to appropriate profile builder

**Design Notes:**
- Clean, centered card layout
- Minimal friction - only essential fields
- Fast signup to reduce drop-off
- Role toggle is visual and clear

---

### **7. Promoter Profile Builder** (`promoter-profile-builder.html`)
**Status:** ✅ Complete
**Features:**
- Progress bar with 4 steps (visual completion tracking)
- Step indicators show active/completed status

**Step 1: Basic Info**
- Group/promoter name
- Location, year founded
- About your events (textarea pitch)
- Primary music genre dropdown
- Secondary genres (tag input)
- Avg attendance, ticket price range
- Preferred event days (checkboxes)
- Preferred event times (dropdown)

**Step 2: Past Events**
- Add multiple past events
- For each event:
  - Event name, date, venue
  - Attendance vs capacity
  - **Artist Lineup Builder:**
    - Headliner section (expandable)
    - Support acts section (expandable)
    - Opening acts section (expandable)
    - For each artist:
      - Name
      - Photo upload
      - Location/origin
      - **Spotify profile link**
      - **Instagram link**
      - **SoundCloud link** (optional)
      - Website (optional)
      - Notable info (labels, follower counts, achievements)
    - Can add multiple artists per role
  - Event photos upload (5-15 recommended)
  - "+ Add Another Event" button
- Overall stats:
  - Total events hosted
  - Total attendees
  - Notable artists worked with

**Step 3: Audience & Reach**
- Social media followers:
  - Instagram, Facebook, TikTok, Twitter
- Email list size and open rate
- Typical marketing strategy (textarea)
- Advance notice needed (dropdown)
- Presale performance (text)

**Step 4: Media & Links**
- Social media profile links:
  - Instagram, Facebook, Website, Resident Advisor, Other
- Profile photo/logo upload
- Event photos upload (5-15 photos)
- Video content links (YouTube/Vimeo)
- Venue references (textarea)

**Completion Screen:**
- Success message
- "Browse Venues" CTA button

**Design Notes:**
- Progress bar updates with each step
- Forms validate before allowing next step
- Artist lineup builder is comprehensive with social links
- All data stored to create rich profile for venues
- One-time setup, then never asked again

---

### **8. Promoter Profile Page** (`promoter-profile-page.html`)
**Status:** ✅ Complete
**Features:**
- Hero section with:
  - Large avatar (140x140px)
  - Name, location, genres, founding year
  - Verified badge
  - Star rating with review count
- Key stats grid (4 columns):
  - Events Hosted
  - Total Attendees
  - Instagram Followers
  - Email Subscribers
- About section with full description
- Genre tags
- Past events grid (cards with images, dates, attendance, artists)
- Marketing & Audience Reach section:
  - Marketing strategy description
  - Stats grid (email open rate, week 1 presales, Facebook, avg attendance)
- Social Media & Online Presence:
  - Large clickable cards for each platform
  - Shows follower counts
  - Instagram, Facebook, Resident Advisor, Website
- Venue Testimonials:
  - 3 testimonials with quotes
  - Author name and venue
  - Left border accent
- Notable Artists section (tag pills)

**Design Notes:**
- LinkedIn-style professional profile
- Everything a venue needs to make a decision
- Social proof throughout (testimonials, follower counts, past events)
- This is what venues see when clicking "View Full Profile" on dashboard

---

## 🔨 WHAT'S LEFT TO BUILD (In Progress)

### **9. Application Form** (NOT STARTED)
**Purpose:** When promoters apply to a venue
**Key Requirement:** Pull from existing profile, only ask event-specific details

**Should Include:**
- Multi-step form (3-4 steps)
- Step 1: Event Basics
  - Event name
  - Preferred date (calendar picker)
  - Backup dates
  - Expected attendance
  - Ticket price range
  - Event time (start/end)
- Step 2: Event Details
  - Event description
  - **Artist lineup for THIS event:**
    - Same detailed artist builder as profile
    - Headliner, support, openers
    - Photos, socials, Spotify links
  - Special requirements (if any)
- Step 3: Marketing Plan
  - How will you promote THIS event?
  - Timeline
  - Collaborative promotion opportunities
- Step 4: Review & Submit
  - Preview of full application
  - Shows $3 charge
  - Submit button
  - "Guaranteed response in 7 days or refund"

**Design Notes:**
- Pre-fill as much as possible from profile
- Show venue info at top (reminder of where they're applying)
- Progress indicator
- Save draft functionality
- Success screen after submission with application tracking link

---

### **10. Messaging/Email Thread Interface** (NOT STARTED)
**Purpose:** Chat between venues and promoters + track email replies

**Key Features:**
- Inbox view (list of conversations)
- Thread view (messages with timestamp)
- Compose new message
- **Email integration:**
  - When venue replies via email, show in thread
  - When promoter replies via email, show in thread
  - "Replied via email" indicator
- Message status (sent, delivered, read)
- Attachment support (PDFs, images)
- Quick actions:
  - Accept application (from message thread)
  - Decline with feedback
  - Request more info
- Notification badges
- Search/filter messages

**Design Notes:**
- Similar to LinkedIn messaging
- Left sidebar with conversation list
- Right panel with active thread
- Email messages styled differently (gray background, "via email" badge)
- Real-time updates when new message arrives

---

### **11. Status Tracker** (NOT STARTED)
**Purpose:** Domino's-style progress bar showing application status

**Statuses:**
1. **Application Submitted** ✓
   - Green checkmark
   - Timestamp
2. **Under Review** (current)
   - Yellow dot (pulsing)
   - "Venue is reviewing your application"
3. **Response Received**
   - Either: Accepted (green) or Declined (gray)
   - Feedback shown if declined
4. **Event Confirmed** (if accepted)
   - Green checkmark
   - Date locked in
5. **Event Complete** (after event happens)
   - Leave review prompt

**Where to Show:**
- Dashboard (for each application)
- Individual application detail page
- Email notifications include status link

**Design Notes:**
- Horizontal progress bar at top
- Each status is a circle node
- Line connects nodes (green = completed, gray = upcoming)
- Current status pulsates or glows
- Click any status to see details/timeline
- Shows time elapsed at each stage
- Countdown timer if approaching 7-day guarantee

---

### **12. Venue Intake Form - Updated Design** (NOT STARTED)
**Purpose:** Update existing detailed venue intake form to new dark theme
**Existing File:** `/mnt/user-data/outputs/venue-intake-form.html` (1297 lines)

**What to Update:**
- Apply dark theme (black, blue gradient, yellow accents)
- Use Space Grotesk for headings
- Keep ALL existing functionality:
  - 4-step form
  - Granular equipment specs (sound, DJ, lighting, backline, technical)
  - Media uploads (venue photos, floor plan, videos)
  - Social media links
  - Capacity, hours, accessibility details
- Update visual design only, not content/structure

**Design Notes:**
- This form is already comprehensive
- Just needs visual refresh to match new design system
- Keep all the detailed equipment dropdowns (Funktion-One, L-Acoustics, CDJ-3000, etc.)

---

### **13. Promoter Intake Form - Updated Design** (NOT STARTED)
**Purpose:** Full promoter onboarding (alternative to profile builder, same content)
**Existing File:** `/mnt/user-data/outputs/promoter-intake-form.html`

**What to Update:**
- Apply dark theme
- Use Space Grotesk typography
- Match the content from Promoter Profile Builder
- 4-step structure
- Update visual design only

**Design Notes:**
- May be redundant with Promoter Profile Builder
- Could merge or use one as the canonical version

---

## 🎨 DESIGN SYSTEM (Use These Everywhere)

### **Colors:**
```css
--black: #0a0a0a;           /* Main background */
--dark-bg: #121212;         /* Card backgrounds */
--dark-card: #1a1a1a;       /* Nested cards */
--blue-dark: #0f172a;       /* Gradient start */
--blue-mid: #1e3a8a;        /* Gradient end */
--yellow: #fbbf24;          /* Primary accent */
--yellow-bright: #fcd34d;   /* Hover states */
--text-primary: #ffffff;    /* Main text */
--text-secondary: #a1a1aa;  /* Secondary text */
--border: #27272a;          /* Borders */
--success: #10b981;         /* Success green */
--danger: #ef4444;          /* Error/decline red */
```

### **Typography:**
```css
/* Headings */
font-family: 'Space Grotesk', sans-serif;
font-weight: 700;
letter-spacing: -0.03em to -0.05em;

/* Body */
font-family: 'Inter', sans-serif;
font-weight: 400;
letter-spacing: -0.01em;
```

### **Google Fonts Import:**
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">
```

### **Common Patterns:**

**Button Styles:**
```css
.btn-primary {
    background: var(--yellow);
    color: var(--black);
    padding: 0.875rem 2rem;
    border-radius: 8px;
    font-weight: 700;
    font-family: 'Space Grotesk', sans-serif;
}

.btn-primary:hover {
    background: var(--yellow-bright);
    transform: translateY(-2px);
    box-shadow: 0 10px 30px rgba(251, 191, 36, 0.3);
}
```

**Card Styles:**
```css
.card {
    background: var(--dark-card);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 2rem;
}

.card:hover {
    border-color: var(--yellow);
    box-shadow: 0 8px 32px rgba(251, 191, 36, 0.15);
}
```

**Section Headings:**
```css
h2 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    letter-spacing: -0.02em;
    font-family: 'Space Grotesk', sans-serif;
}
```

**Tag/Badge Styles:**
```css
.tag {
    background: rgba(251, 191, 36, 0.15);
    border: 1px solid rgba(251, 191, 36, 0.3);
    color: var(--yellow);
    padding: 0.5rem 1.25rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 600;
}
```

---

## 🚀 ADDITIONAL FEATURES TO BUILD

### **14. Calendar/Availability Management** (HIGH PRIORITY)
**Purpose:** Venues manage their availability
**Features:**
- Monthly calendar view
- Click dates to mark available/unavailable
- Recurring availability (e.g., "every Friday")
- Block out date ranges
- See booked dates (from accepted applications)
- Sync with Google Calendar (nice to have)
- Export calendar (ICS file)

**Design Notes:**
- Similar to Airbnb calendar
- Color coding: Available (yellow), Booked (red), Blocked (gray)
- Drag to select multiple dates
- Quick toggle buttons ("Mark all Fridays available")

---

### **15. Browse Promoters Page** (MEDIUM PRIORITY)
**Purpose:** Reverse marketplace - venues browse promoters
**Features:**
- Search/filter promoters by:
  - Genre
  - Location
  - Audience size (followers, email list)
  - Past venue ratings
  - Event frequency
- Promoter cards showing:
  - Avatar, name, location
  - Quick stats (events, attendees, followers)
  - Genre tags
  - Rating
  - "Invite to Apply" button
- Sort options (highest rated, most events, most followers)

**Design Notes:**
- Mirror marketplace design
- Sidebar filters
- Card grid layout
- Clicking card goes to full promoter profile

---

### **16. Welcome/Onboarding Tour** (LOW PRIORITY)
**Purpose:** First-time user walkthrough
**Features:**
- After signup completion
- 3-5 slide carousel:
  - "Welcome to VenueLink"
  - "How to browse/apply" (for promoters)
  - "How to review applications" (for venues)
  - "Guaranteed responses"
  - "Get started" CTA
- Skip button
- Progress dots
- Remembers if user has seen it

---

### **17. Notifications Center** (MEDIUM PRIORITY)
**Purpose:** All notifications in one place
**Features:**
- List of notifications with:
  - Icon, title, timestamp
  - Read/unread status
  - Click to go to relevant page
- Types:
  - "New application from [Promoter]"
  - "[Venue] accepted your application"
  - "Response time reminder" (approaching 7 days)
  - "Leave a review for [Event]"
- Mark all as read
- Filter by type

---

### **18. Settings Page** (LOW PRIORITY)
**Purpose:** Account and notification settings
**Sections:**
- Profile settings (edit basic info)
- Email notification preferences
- SMS notification preferences
- Password change
- Payment methods (linked to Stripe)
- Billing history
- Delete account

---

## 💾 FILES STRUCTURE FOR PETER

```
venuelink/
├── frontend/
│   ├── landing-redesign.html ✅
│   ├── marketplace-redesign.html ✅
│   ├── venue-profile-redesign.html ✅
│   ├── venue-dashboard-redesign.html ✅ (THE STAR)
│   ├── promoter-profile-page.html ✅
│   ├── promoter-profile-builder.html ✅
│   ├── signup-page.html ✅
│   ├── widget-redesign.html ✅
│   ├── application-form.html 🔨 (TO BUILD)
│   ├── messaging-interface.html 🔨 (TO BUILD)
│   ├── status-tracker.html 🔨 (TO BUILD)
│   ├── venue-intake-form-redesign.html 🔨 (UPDATE EXISTING)
│   ├── promoter-intake-form-redesign.html 🔨 (UPDATE EXISTING)
│   ├── calendar-management.html 💡 (NICE TO HAVE)
│   ├── browse-promoters.html 💡 (NICE TO HAVE)
│   └── [other pages as needed]
│
├── backend/ (PETER BUILDS THIS)
│   ├── server.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── venues.js
│   │   ├── promoters.js
│   │   ├── applications.js
│   │   ├── messages.js
│   │   └── calendar.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Venue.js
│   │   ├── Promoter.js
│   │   ├── Application.js
│   │   └── Message.js
│   └── config/
│       ├── database.js
│       └── stripe.js
│
└── BUILD_SUMMARY.md ✅
```

---

## 📋 WHAT PETER NEEDS TO BUILD

### **Backend (Node.js + Express + PostgreSQL)**

**Database Tables:**
1. **users** (id, email, password_hash, role [venue/promoter], created_at)
2. **venues** (id, user_id, name, location, capacity, equipment_json, photos_json, etc.)
3. **promoters** (id, user_id, name, location, stats_json, social_json, etc.)
4. **applications** (id, promoter_id, venue_id, event_details_json, status, created_at)
5. **messages** (id, application_id, sender_id, content, is_email, created_at)
6. **availability** (id, venue_id, date, is_available)
7. **reviews** (id, application_id, reviewer_id, rating, comment)

**API Endpoints:**
```
POST   /api/auth/signup
POST   /api/auth/login
POST   /api/auth/reset-password

GET    /api/venues
GET    /api/venues/:id
POST   /api/venues (create)
PUT    /api/venues/:id (update)

GET    /api/promoters
GET    /api/promoters/:id
POST   /api/promoters (create)
PUT    /api/promoters/:id (update)

GET    /api/applications (list with filters)
POST   /api/applications (submit new)
PUT    /api/applications/:id (accept/decline)
POST   /api/applications/:id/feedback (add decline feedback)

GET    /api/messages/:applicationId
POST   /api/messages (send new message)

GET    /api/availability/:venueId
POST   /api/availability (update dates)

POST   /api/payments/create-charge (Stripe)
POST   /api/payments/refund (7-day guarantee)
```

**Integrations:**
1. **Stripe** - $3 application fees, subscriptions
2. **SendGrid/Mailgun** - Email notifications
3. **AWS S3 or Cloudflare R2** - File uploads (photos, videos)
4. **Twilio** (optional) - SMS notifications

**Authentication:**
- JWT tokens
- Password hashing (bcrypt)
- Email verification

**Deployment:**
- Backend: Railway, Render, or Heroku
- Frontend: Vercel or Netlify
- Database: PostgreSQL (managed)
- Domain: venuelink.com

---

## 🎯 PRIORITY FOR NEXT SESSION

When you return tonight, we should build **in this order:**

### **Must Build (Core Features):**
1. **Application Form** - Promoters need this to apply
2. **Status Tracker** - Domino's-style transparency
3. **Messaging Interface** - Communication after acceptance
4. **Calendar Management** - Venues manage availability

### **Should Build (Important):**
5. **Browse Promoters** - Reverse marketplace
6. **Update Venue Intake Form** - Visual refresh

### **Nice to Have (Polish):**
7. **Update Promoter Intake Form** - Visual refresh
8. **Notifications Center** - Centralized alerts
9. **Welcome Tour** - First-time UX
10. **Settings Page** - Account management

---

## 💡 NOTES & INSIGHTS

### **Key Design Decisions:**
- **Dark theme** - Beatport-inspired, feels premium and nightlife-appropriate
- **Yellow accents** - High contrast, draws eye to CTAs
- **Space Grotesk** - Bold, modern, tight tracking for headings
- **LinkedIn/Tinder model** - Rich profiles eliminate back-and-forth
- **Feedback on decline** - Builds ecosystem quality
- **Artist details with socials** - Critical for venue decision-making
- **Domino's tracker** - Transparency reduces anxiety

### **Core Value Props:**
**For Venues:**
- See EVERYTHING in one view (no email tennis)
- Make decisions in 2 minutes vs 2 weeks
- Build reputation through feedback ratings
- Guaranteed applicant quality (verified profiles)

**For Promoters:**
- Never get ghosted (7-day guarantee)
- See real availability upfront
- One profile, unlimited applications
- Actionable feedback when declined

### **Competitive Advantages:**
1. **Profile-first model** - Data collected once, used forever
2. **Artist lineup detail** - No competitor does this
3. **Email integration** - Venues can reply via email, shows in app
4. **Status transparency** - Domino's-style tracking
5. **Feedback system** - Helps promoters improve

### **Monetization:**
- $3 per application (Groover model proven)
- Pro plan: $49/mo unlimited applications
- Venue plan: $79/mo receive unlimited
- Take rate on ticket sales (future)
- Featured venue listings (future)

---

## 🔥 WHEN YOU RETURN TONIGHT

**Start fresh conversation with:**

> "Hey Claude, I'm back to finish VenueLink. I have a handoff document with everything we've built so far. Let me upload it.
> 
> We need to build:
> 1. Application Form
> 2. Status Tracker (Domino's-style)
> 3. Messaging Interface
> 4. Calendar Management
> 5. Browse Promoters page
> 
> Use the same dark theme, Space Grotesk typography, and design system from the handoff doc. Let's start with the Application Form."

Then upload this file and I'll pick up exactly where we left off! 🚀

---

**Built by Claude for Mike | March 8, 2026**
**Total Pages Complete: 8 | Pages To Build: 5+ | Ready for Peter: Almost**
