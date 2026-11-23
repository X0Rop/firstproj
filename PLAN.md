# Gita Scroll: Build & Revenue Plan

Working name: **Gita Scroll**. Check the name is free on the App Store, Play Store and domains before you commit to it.

Written for a non-technical founder. Each phase lists what to do, who does it, what it costs and when it's done.

---

## 1. What we learned from Scroll The Bible

| Fact | Detail |
|---|---|
| Who built it | Gabriel Jacobson, a solo developer in Oregon (JCBSN LLC). His first app, *Bible Word Study* (July 2025), reportedly earned about $60K/month first. |
| Launch | December 17, 2025, on iPhone only. |
| Core idea | The Bible as a TikTok-style feed: one verse per screen, swipe up for the next. It's built to replace doomscrolling. |
| Rank | Highest-ranked Bible app on the US App Store as of Aug 29, 2026. About 18K ratings at 4.8★. |
| Revenue (estimates only) | Third-party trackers range from about $220K to $2M per month. Nothing is confirmed, so assume six figures a month. |
| Downloads | More than 15K a week after Meta ads started in July 2026. Estimates run from 90K to 400K a month. |
| Pricing | Free scrolling, plus a premium tier at about $4.99/month or $19.99 to $29.99/year with a 3 to 7 day trial. |
| Premium features | AI explanations and Q&A, original-language (Greek/Hebrew) word study, reading plans. |
| Shipped since launch | Reading plans, a Discover tab, red-letter mode, lock-screen widgets, progress tracking, Spanish. |
| Growth | Mostly organic first: faith creators posting 60 to 90 second TikTok/Reels videos that show the app around 40 seconds in. Paid Meta ads came only once the funnel was proven. |
| Complaints | The paywall shows up too early. There's no Android version. |
| Competition | YouVersion (the biggest Bible app) launched a copy, *Bible Loop*, in May 2026, and many clones followed. |

### What this means for us
1. **The format works, and nobody owns it for the Gita yet.** Existing Gita apps such as "Bhagavad Gita For All" (1M+ downloads) are traditional readers, not feeds.
2. **One person can win this.** It was one developer with no funding. Speed and marketing mattered more than team size.
3. **Launch on Android too.** India is mostly Android, and Scroll The Bible skipped it entirely.
4. **Don't put the paywall in front of the verses.** Keep scrolling free and charge for depth: AI, audio, commentary.

---

## 2. The product

### Target users
- **Primary: Indian diaspora in the US, UK, Canada and Australia, ages 18 to 40.** They pay at US prices and are culturally connected but rarely read the Gita.
- **Secondary: young urban Indians**, a huge base on Android who pay at India prices.
- **Tertiary: Western yoga and mindfulness audiences**, who already know the Gita as a source of "wisdom".

### Features by phase

**Version 1 (MVP, launch in 8 to 10 weeks)**
- Vertical verse feed covering all 700 verses: Sanskrit, transliteration and English (Hindi in v1.1).
- Mood filters: Anxious, Lost, Grieving, Angry, Work & study.
- Like, save and share (shared as a nicely designed image card for Instagram Stories or WhatsApp; this is your free marketing).
- A short explanation of every verse.
- Daily streak, plus a "verse of the day" push notification.
- Onboarding quiz (why are you here, how do you feel, how much time do you have), then the paywall with a free trial.
- **Premium:** AI guide ("Ask Krishna's teaching about my problem"), audio chanting of each verse, chapter-by-chapter reading plans.

**Version 2 (months 3 to 6)**
- Home and lock-screen widgets.
- Hindi, Gujarati, Tamil, Telugu and Marathi.
- Word-by-word Sanskrit meanings.
- Reading plans: "7 days to beat anxiety", "Gita in 30 days".
- Commentary from several traditions.
- Festival content: Gita Jayanti, Janmashtami, Diwali.

**Later**
- Other texts (Upanishads, Ramayana verses, Hanuman Chalisa) to grow into a "Hindu wisdom" app.
- Family and gift subscriptions.
- Apple Watch.

### Content and legal (this matters)
- **The Sanskrit text is public domain.** Use it freely.
- **Most popular English translations are copyrighted**, including Prabhupada's *Bhagavad-gītā As It Is* (BBT), Eknath Easwaran and Gita Press's modern editions. **Do not copy them.**
- Safe options: (a) older public-domain translations such as Annie Besant (1905) or K.T. Telang (1882), or (b) **commission your own modern translation** (recommended). A Sanskrit scholar costs about ₹1 to 3 lakh, or you can draft with AI and have a scholar edit. Owning your translation is also a moat.
- Every AI answer must be grounded in the verse text and carry a "not a substitute for a guru or professional help" note. Add crisis-helpline handling for users who mention self-harm.
- Use respectful design: no ads on scripture, and careful imagery of Krishna.

---

## 3. Technology (decided for you)

| Piece | Choice | Why |
|---|---|---|
| App framework | **React Native with Expo** | One codebase gives you iPhone and Android, there are many developers for hire, and it's fast to ship. |
| Backend and database | **Supabase** (or Firebase) | User accounts, saved verses and streaks. A free tier covers you to about 50K users. |
| Subscriptions | **RevenueCat** | Handles Apple and Google payments, trials and paywall A/B tests. Free until $2.5K/month in revenue. |
| AI guide | **Claude API** (Anthropic) | Answers grounded in the verse plus its commentary. Costs cents per user per month. Put it behind the paywall. |
| Audio | Record a real chanter (best), or use licensed recordings | Authentic chanting is a premium feature people pay for. |
| Analytics | **PostHog** or Mixpanel, plus the store dashboards | Track onboarding completion, trial starts and day-1/day-7 retention. |
| Push notifications | Expo Notifications or OneSignal | Verse of the day and streak reminders. |
| Attribution | Adjust or AppsFlyer (once you start paid ads) | So you know which ad brought which paying user. |

All 700 verses are a small file (under 2 MB) bundled inside the app, so the feed works offline.

---

## 4. Step-by-step roadmap

### Phase 0: Set up the company (weeks 1 to 2)
1. **Register a company.** If you're in India, a Private Limited (around ₹10 to 15K via Vakilsearch or IndiaFilings). If you're in the US, an LLC through Stripe Atlas or a state filing. Apple and Google pay out to the company.
2. **Open a business bank account.**
3. **Get a D-U-N-S number** (free) so you can enrol in Apple's developer program as an organization.
4. **Apple Developer account**: $99/year. **Google Play Console**: $25 one time.
5. Buy the domain (for example gitascroll.app) and set up an email at that domain.
6. Claim the same handle on Instagram, TikTok, YouTube and X.
7. Trademark search, then file for the name (later is fine).

### Phase 1: Validate before building (weeks 1 to 3, in parallel)
1. Show the prototype (link below) to 20 people in the target audience and watch them use it.
2. Start an Instagram/TikTok page **now** and post one Gita verse video a day. If those posts get views, the app will too. This also builds your launch audience.
3. Make a one-page website with an email waitlist. The goal is 1,000 signups before launch.

### Phase 2: Hire the builder (weeks 2 to 3)
You need **one strong React Native developer**, not an agency team.
- Where to look: Upwork, Toptal, Contra, LinkedIn, or Indian freelancers on Twitter/X who post their shipped apps.
- What to require: at least 2 published apps in the stores, Expo experience, and RevenueCat experience.
- Budget: India-based senior freelancer ₹3 to 6 lakh for the MVP. US or EU freelancer $15K to $40K.
- How to pay: in **milestones** (feed working, accounts and paywall, AI and audio, store launch).
- **You own the code.** It goes in *your* GitHub account (this repository) and *your* Apple and Google accounts. Put that in the contract.
- Ask me to write the job post and screen the candidates' code. That's part of my role as CTO.

Alternative: **build with me.** I can write most of the app here in this repository, and you hire a part-time developer only for store submission and testing. That's cheaper but slower, because you need to learn to run builds.

### Phase 3: Build the MVP (weeks 3 to 10)
| Week | Deliverable |
|---|---|
| 3–4 | All 700 verses cleaned into a structured file, the feed screen, mood filters, like and save |
| 5–6 | Onboarding quiz, accounts, streaks, push notifications, share-as-image |
| 7–8 | RevenueCat paywall, AI guide, audio player |
| 9 | Internal testing (TestFlight and Play internal testing) with 50 waitlist users |
| 10 | Store screenshots, description, privacy policy, then submission |

At the same time, **you** handle content: translation, explanations, audio recording, mood tags.

### Phase 4: Launch (week 10 to 12)
- App Store Optimization: the title "Gita Scroll: Bhagavad Gita Daily" and keywords like *bhagavad gita, gita, krishna, hindu, sanskrit, daily verse, meditation*.
- Email the waitlist, post on Reddit (r/hinduism, r/indianamerican, carefully and within the rules), WhatsApp groups, temple communities and student associations.
- Time the launch near a festival. **Gita Jayanti** (November/December) or **Janmashtami** (August/September) give free attention.

### Phase 5: Grow (month 3 onward)
1. **The creator engine (the main growth method).** Pay 20 to 50 small Hindu, spiritual and self-help creators ($50 to $300 per video, or ₹2K to 15K in India) to make 60 to 90 second videos. Start with a real problem ("I was anxious before my exam…"), read a verse, show the app around 40 seconds. Keep paying the creators whose videos convert.
2. **Run your own faceless accounts.** Post 3 to 5 videos a day of verse cards over calm music, all filmed straight from the app.
3. **Paid ads, only after organic proves the funnel.** Meta (Instagram and Facebook) ads aimed at the diaspora in the US, UK and Canada. Rule: only scale while the first-week subscription revenue covers about 50% or more of ad spend.
4. Share cards from inside the app are free advertising. Every shared verse carries your logo and link.

---

## 5. Revenue model

- **Free:** the full verse feed, mood filters, saves, streaks.
- **Plus** with a 7-day free trial:
  - US/UK/CA: **$29.99/year** or $4.99/month
  - India: **₹999/year** or ₹149/month (use the stores' regional pricing)
- Later: lifetime ($79.99), family plan, and a donation-style "Gift Gita to someone" option.
- Never put ads in the scripture feed.

### Rough numbers (illustrative, not a forecast)
| | Month 6 | Month 12 |
|---|---|---|
| Downloads per month | 30,000 | 120,000 |
| Trial start rate | 15% | 18% |
| Trial to paid | 35% | 40% |
| New paying users per month | about 1,575 | about 8,640 |
| Blended price per year | about $20 | about $22 |
| Monthly revenue (all active subscribers) | about $8K to 15K | about $60K to 120K |

Apple and Google take **15%** on your first $1M per year (apply for the Small Business Program) and 15% on subscriptions after year one.

---

## 6. Budget for the first 6 months

| Item | Lean (India-based) | Comfortable |
|---|---|---|
| Company setup and legal | ₹25K | $1,500 |
| Store accounts | about $125 | about $125 |
| Developer (MVP) | ₹4 lakh | $30,000 |
| Translation and commentary | ₹1.5 lakh | $5,000 |
| Audio recording | ₹50K | $2,000 |
| Design (icon, screenshots) | ₹40K | $3,000 |
| Servers, AI, tools | ₹10K/month | $300/month |
| Creator marketing | ₹2 lakh | $10,000 |
| Paid ads (after validation) | ₹3 lakh | $20,000 |
| **Total** | **about ₹13 to 15 lakh** | **about $70K** |

---

## 7. Your weekly scoreboard
Check these every week. They tell you whether the business works:
1. **Onboarding completion**: target above 70%
2. **Trial start rate**: target above 12%
3. **Trial to paid**: target above 30%
4. **Day-7 retention**: target above 25%
5. **Verses scrolled per session**: target above 8
6. **Creator video views to installs**

---

## 8. Risks
| Risk | What we do about it |
|---|---|
| A big player copies us (as YouVersion did with Bible Loop) | Move fast, own the translation and audio, build community and streaks, and serve Indian languages better than anyone. |
| Copyright claims on translations | Use only public-domain or commissioned text and keep the contracts. |
| AI says something wrong or offensive about scripture | Ground answers in the verse, have a scholar review common answers, add a report button. |
| App Store rejects us as a "template/clone" | Use original design, real content depth and a native feel. Don't copy Scroll The Bible's UI or name. |
| Founder runs out of money | Validate with organic content first and pay the developer in milestones. |

---

## 9. Your next 7 days
1. Open the prototype on your phone and show it to 10 people.
2. Decide on the name and check the App Store, Play Store, domain and Instagram handle.
3. Start the company registration and the D-U-N-S request.
4. Post your first 7 Gita verse videos on Instagram and TikTok.
5. Decide between **hiring a developer** and **building with me**, then tell me. I'll write the job post or start coding the real app in this repository.
