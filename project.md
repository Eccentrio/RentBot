# Create the PRD as a Markdown file
prd_content = """# 🏠 RentBot — Tenant Communication Tool for Small Landlords

## 1. Overview

**Purpose:**  
RentBot simplifies and automates communication between small landlords and tenants. It helps landlords manage rental inquiries, FAQs, and rent-related follow-ups — without switching between texts, emails, or calls.

**Vision:**  
Build an **AI-powered communication assistant** that helps landlords with 2–10 rental units handle tenant messages efficiently — reducing missed leads and saving hours each week.

**Goal for MVP:**  
Launch a minimal, working product that handles **automated inquiry responses and appointment scheduling** via SMS and email — integrated with landlords’ existing tools (Google Calendar, Gmail, or Outlook).

---

## 2. Target Users

**Primary User:**  
Independent landlords or small property owners managing **2–10 residential units**.

**User Characteristics:**
- Handles communication manually (texts, calls, emails)  
- Juggles property management with a full-time job  
- Loses time answering repetitive questions (rent amount, availability, pets, etc.)  
- May not use advanced tools like AppFolio or Buildium due to cost/complexity  

---

## 3. Problem Statement

Small landlords lose money and time due to poor communication systems:
- Missed inquiries → lost tenants → vacancy cost ($2K+/month)  
- Delayed responses → bad tenant experience  
- No unified inbox or automation → manual chaos  

**Solution:**  
RentBot acts as a virtual assistant — automating repetitive communication through SMS, email, and (later) WhatsApp.

---

## 4. MVP Scope

### 🧩 Core Features (MVP)

| Feature | Description | Tools / Implementation |
|----------|--------------|------------------------|
| **Automated FAQ Response (AI Chat)** | RentBot answers common questions (rent, pets, availability, address, etc.) using predefined templates or AI (GPT-4 API). | GPT API + Twilio SMS / Gmail integration |
| **Inquiry Routing** | If question is complex, forward message to landlord or schedule callback. | Rule-based routing logic |
| **Showing Scheduler** | Sync with landlord’s calendar (Google/Outlook) to auto-schedule showings. | Google Calendar API |
| **Follow-Up Reminders** | Auto-follow-up with tenants after inquiry or showing (e.g., “Are you still interested?”). | Scheduled tasks / cron jobs |
| **Simple Dashboard (Web)** | Centralized view of tenant messages, scheduled showings, and automation history. | Low-code web app (Bubble, Replit, or React + Firebase) |

---

## 5. Out of Scope (Future Versions)

| Future Feature | Description |
|-----------------|--------------|
| **Maintenance Requests** | Tenants submit issues; RentBot routes them to vendors. |
| **Rent Collection** | Automated reminders and payment integration (Stripe). |
| **Lease Renewals** | Notify landlord and tenant before expiration. |
| **Document Storage** | Keep lease and compliance docs in one place. |
| **Tenant Screening** | Integrated background and credit checks. |

---

## 6. User Journey (MVP)

1. **Landlord signs up** → Enters property details, FAQs, and preferred communication channel.  
2. **Tenant inquiry arrives** (SMS or email).  
3. **RentBot analyzes message** → Responds instantly if it’s a known FAQ.  
4. If unavailable → **suggests available time slots** via integrated calendar.  
5. **Logs interaction** in dashboard and sets auto follow-up reminder.

---

## 7. Success Metrics

| Metric | Target (First 3 Months) |
|--------|--------------------------|
| **Active landlords** | 50+ landlords using RentBot |
| **Avg. response time** | <10 seconds automated reply |
| **Conversion rate** | 1 in 10 inquiries → scheduled showing |
| **Retention** | 70% landlords active after first month |
| **Revenue** | $15–30 per unit/month (target $2K MRR MVP stage) |

---

## 8. Tech Stack (MVP)

| Layer | Suggested Tools |
|--------|----------------|
| **Frontend** | Replit + React / Bubble |
| **Backend** | Firebase or Supabase |
| **Messaging** | Twilio (SMS), SendGrid (email) |
| **AI** | OpenAI GPT-4 API for NLP/FAQ generation |
| **Scheduling** | Google Calendar API |
| **Hosting** | Vercel / Replit Cloud |

---

## 9. Go-To-Market (Initial Launch)

| Channel | Strategy |
|----------|-----------|
| **Facebook Groups** | Engage landlord and real estate investor communities. |
| **Reddit Threads** | Participate in r/Landlord, r/RealEstateInvesting, r/PropertyManagement. |
| **YouTube Creators** | Partner with small real estate content creators for shoutouts. |
| **Landing Page** | Clear CTA: “Automate your tenant messages in 10 minutes.” |

---

## 10. Risks & Mitigation

| Risk | Mitigation |
|------|-------------|
| Low adoption (skepticism toward AI) | Start with clear value: “Save 5 hours/week — guaranteed.” |
| Message errors or tone mismatch | Provide adjustable tone settings & landlord review option. |
| Integration complexity | Limit MVP to SMS + Google Calendar only. |
| Privacy concerns | Store minimal tenant data, show compliance badge (GDPR-lite policy). |

---

## 11. MVP Deliverables & Timeline

| Milestone | Description | Duration |
|------------|-------------|-----------|
| **Week 1** | Setup basic SMS auto-reply (Twilio + GPT). | 1 week |
| **Week 2** | Add Google Calendar scheduling. | 1 week |
| **Week 3** | Build minimal dashboard (Replit / Bubble). | 1 week |
| **Week 4** | Test with 10 landlords (closed beta). | 1 week |

**Total Duration:** 4 weeks to MVP launch 🚀

---

## 12. Future Expansion (Post-MVP Roadmap)

1. Maintenance Request Automation  
2. Rent Reminder + Stripe Integration  
3. WhatsApp & Messenger Integrations  
4. Multi-Property Dashboard  
5. Mobile App (React Native)

---

## 13. Appendix

**Pricing Model:**
- $15/unit/month → Basic Automation (up to 10 units)  
- $25/unit/month → Pro (adds maintenance and renewals)  
- Add-ons:  
  - Tenant Screening → $10/applicant  
  - Vendor Network Access → $20/month  
"""

# Write the PRD to a markdown file
with open("/mnt/data/RentBot_PRD.md", "w") as f:
    f.write(prd_content)

"/mnt/data/RentBot_PRD.md"
