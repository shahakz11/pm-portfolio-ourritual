## Product Requirement Document: Ritual Match - Transparent Therapist & Session Customization

---

### 2. Objective & Vision

**Objective:** To empower OurRitual users with greater control and transparency in selecting their relationship expert and customizing session parameters, thereby fostering stronger therapeutic alliances, increasing user satisfaction, and strengthening the overall trust in the OurRitual platform.

**Vision:** To become the most trusted and personalized platform for relationship support, where users confidently connect with the ideal expert and build a tailored therapeutic journey that seamlessly integrates into their lives, leading to healthier, lasting partnerships. This feature aims to shift OurRitual from an expert-assigned model to a user-driven, choice-centric experience, aligning with our mission to democratize expert assistance through accessibility and flexibility.

---

### 3. Target Audience

This feature targets all OurRitual users and potential new subscribers, particularly those:

*   **Seeking initial expert connection:** Individuals and couples looking to begin their journey with OurRitual who value choice and transparency in their therapist selection.
*   **Dissatisfied with current therapist matching:** Users who have experienced suboptimal matches or felt a lack of connection with assigned experts.
*   **Requiring specific expertise:** Couples navigating unique challenges (e.g., new parents, long-distance, LGBTQ+) who want to ensure their expert has relevant specialization.
*   **With varying time and budget constraints:** Users who desire flexibility in session length to better fit their schedules and financial considerations.
*   **Tech-savvy individuals:** Those comfortable utilizing app-based tools for search, filtering, and booking.

**Persona Examples:**
*   **The Proactive Professional Couple (Sarah & Mark):** They will appreciate the ability to find a therapist who specializes in communication and proactive relationship building, can accommodate their busy schedules with flexible session lengths, and whose profile aligns with their preference for evidence-based approaches.
*   **The Stressed New Parents (Emily & David):** They will benefit immensely from being able to find an expert specializing in "love after kids" who understands their unique challenges, and to select session durations that can be realistically managed around their childcare responsibilities. The transparency will reduce anxiety about the initial connection.

---

### 4. User Stories

As a [type of user], I want to [action] so that [benefit].

1.  **As a new OurRitual user,** I want to browse a list of available relationship experts with detailed profiles **so that** I can confidently choose a therapist whose background and approach align with my relationship goals before booking my first session.
2.  **As a couple seeking therapy for a specific issue (e.g., new parenthood),** I want to filter experts by their specialization and experience **so that** I can find someone with relevant expertise to address our unique challenges.
3.  **As a busy professional,** I want to see a therapist's availability and choose between different session lengths (e.g., 20, 40, or 60 minutes) **so that** I can schedule sessions that fit my unpredictable schedule and preferred therapeutic depth.
4.  **As a user evaluating an expert,** I want to watch a short introductory video from the therapist and read aggregated client feedback (internal ratings) **so that** I can get a better feel for their personality and style before making a commitment.
5.  **As an OurRitual subscriber,** I want to easily switch to a different expert if my initial match isn't a good fit, **so that** I don't feel locked into an unproductive therapeutic relationship.
6.  **As a user concerned about cost,** I want to see the pricing options clearly displayed for different session lengths and therapist tiers **so that** I can make an informed decision within my budget.

---

### 5. Functional Requirements & Specs

This section details the user-facing interactions and system behaviors for the "Ritual Match" feature.

**5.1. Expert Discovery & Search (Browse/Filter)**

*   **FR-5.1.1: Expert Listing Page:**
    *   Display a paginated list of available relationship experts.
    *   Each expert card shall display: Profile Photo, Name, Primary Specializations (e.g., "Communication," "Parenting," "Conflict Resolution"), Average Rating (if available), and a short one-liner bio.
*   **FR-5.1.2: Advanced Filtering System:**
    *   **Filter Options (Multi-select where applicable):**
        *   **Specialization:** e.g., Gottman Method, EFT, Communication, Intimacy, Parenting, Life Transitions, LGBTQ+ Relationships, Pre-Marital, Conflict Resolution.
        *   **Availability:** Day of Week, Time of Day (Morning, Afternoon, Evening).
        *   **Language:** English, Spanish, etc.
        *   **Gender of Expert:** Male, Female, Non-binary, Prefer not to say.
        *   **Session Length Preference:** 20 min, 40 min, 60 min.
        *   **Price Tier (MVP: Implicit, Phase 2: Explicit):** Standard, Premium.
    *   **FR-5.1.3: Search Bar:** Allow users to search for experts by name or keywords within their bio/specializations.
    *   **FR-5.1.4: Real-time Filter Application:** Filters should apply dynamically, updating the expert list immediately.
    *   **FR-5.1.5: Clear Filters Button:** Provide an option to reset all applied filters.

**5.2. Expert Profile Page**

*   **FR-5.2.1: Comprehensive Expert Bio:**
    *   Full Name, Professional Photo, Credentials (e.g., LMFT, LCSW), Years of Experience, Primary Specializations.
    *   Detailed "About Me" section describing their philosophy, therapeutic approach, and what clients can expect.
    *   List of specific methods used (e.g., Gottman Method, EFT, CBT).
*   **FR-5.2.2: Introductory Video (Phase 2):**
    *   A short (1-2 minute) video where the expert introduces themselves and their approach.
    *   Video player with standard controls (play/pause, volume, fullscreen).
*   **FR-5.2.3: Availability Calendar:**
    *   Display the expert's upcoming available slots in a clear, interactive calendar format (weekly/monthly view).
    *   For each slot, show available session lengths (e.g., 20min, 40min, 60min) and associated pricing (if tiered pricing is implemented).
*   **FR-5.2.4: Client Feedback/Ratings (Phase 2):**
    *   Display an aggregated star rating (out of 5).
    *   Option to view anonymized, moderated feedback comments from other OurRitual users.
*   **FR-5.2.5: Integration with Pathways:**
    *   Display the core "Pathways" that the expert commonly works with or recommends.

**5.3. Session Booking & Customization**

*   **FR-5.3.1: Session Length Selection:**
    *   When an available slot is selected, present a clear choice of available session lengths (20 min, 40 min, 60 min) with their respective costs.
    *   Default to 40-minute sessions but allow user override.
*   **FR-5.3.2: Booking Confirmation:**
    *   Display a summary of the selected expert, date, time, duration, and total cost.
    *   Require explicit user confirmation before finalizing the booking.
*   **FR-5.3.3: Payment Integration:**
    *   Utilize existing payment system for booking.
    *   Clearly display payment amount and method.
*   **FR-5.3.4: Booking Notifications:**
    *   Send email and in-app notifications upon successful booking.
    *   Send reminders X hours/days before the session.
*   **FR-5.3.5: Reschedule/Cancel Session:**
    *   Allow users to reschedule or cancel a session within the platform, adhering to OurRitual's established cancellation policy (which should be improved as per overall product investigation).
    *   Clearly display any associated fees or refund policies during the process.

**5.4. User Dashboard & My Experts**

*   **FR-5.4.1: My Experts Section:**
    *   A dedicated section on the user dashboard displaying the currently chosen expert(s).
    *   Option to view their profile, upcoming sessions, and a prominent "Switch Expert" button.
*   **FR-5.4.2: Switch Expert Flow:**
    *   Provide a guided flow for users to select a new expert.
    *   Clearly communicate implications (e.g., continuity of care, data transfer to new expert if opted-in).
    *   Offer a brief, optional survey on why they are switching to gather feedback.

**5.5. Expert-Facing Management (Admin Portal - brief)**

*   **FR-5.5.1: Expert Profile Management:** Experts can create and update their profiles (bio, specializations, credentials, professional photo).
*   **FR-5.5.2: Availability Management:** Experts can set their working hours, block off time, and specify available session lengths for different slots.
*   **FR-5.5.3: Introductory Video Upload:** Experts can upload and manage their introductory videos (Phase 2).

---

### 6. Non-Functional Requirements

*   **Performance:**
    *   Expert search and filter results should load within 2 seconds.
    *   Expert profile pages should load within 1.5 seconds.
    *   Session booking confirmation should process within 3 seconds.
    *   The system should efficiently handle concurrent searches and bookings.
*   **Scalability:**
    *   The platform must scale to support a growing database of experts (thousands) and increasing user demand for search, filtering, and booking.
    *   Availability calendar and scheduling system must handle complex schedules for numerous experts.
*   **Security:**
    *   All user and expert data (profiles, booking history, payment information) must be encrypted both in transit and at rest.
    *   Adhere to all relevant data privacy regulations (e.g., HIPAA compliance for session content, though OurRitual currently operates as coaching).
    *   Robust authentication and authorization mechanisms for both users and experts.
    *   Protection against common web vulnerabilities (OWASP Top 10).
*   **Usability & Accessibility:**
    *   The interface must be intuitive and easy to navigate for users of all technical proficiencies.
    *   Adhere to WCAG 2.1 AA accessibility standards for users with disabilities (e.g., screen reader compatibility, keyboard navigation, sufficient color contrast).
    *   Responsive design for seamless experience across web, iOS, and Android platforms.
*   **Reliability:**
    *   High availability (99.9% uptime) for expert discovery and booking functionality.
    *   Robust error handling and graceful degradation in case of system failures.
*   **Maintainability:**
    *   Codebase should be modular, well-documented, and follow established coding standards to facilitate future enhancements and bug fixes.

---

### 7. Success Metrics

**North Star Metric:**
*   **Number of long-term (3+ months) active couples/individual users engaged in expert-led sessions.** This reflects successful matching and sustained therapeutic engagement, leading to "healthier, lasting partnerships."

**Key Performance Indicators (KPIs):**

*   **Conversion Rate (Expert Selection):** % of users who view expert profiles and successfully book a first session.
*   **First Session Satisfaction Score:** Post-first-session survey score related to the expert match (e.g., "How satisfied are you with your chosen expert?").
*   **Expert Switch Rate:** % of users who switch experts after their first or subsequent sessions. *(Goal: Reduce this over time as initial matching improves)*.
*   **Average Session Duration Chosen:** Average length of sessions booked (e.g., shift towards more 40/60 min sessions if that's a business goal).
*   **Churn Rate (Expert-related reasons):** Track cancellations where users cite "poor therapist match" or "lack of transparency" as reasons. *(Goal: Reduce)*.
*   **Customer Service Inquiries (Expert Matching/Cancellation):** Number of support tickets related to expert matching, selection, or dissatisfaction. *(Goal: Reduce)*.
*   **Average Revenue Per User (ARPU):** Track changes as flexible session lengths and potential tiered pricing are introduced. *(Goal: Increase)*.

**Adoption Goals (First 6 months post-launch):**

*   **Expert Profile Completion:** 90% of active OurRitual experts have completed their detailed profiles.
*   **User Engagement with Feature:** 70% of new users utilize the search/filter functionality before booking.
*   **Positive Feedback:** Achieve an average 4.0+/5.0 rating on first-session satisfaction surveys regarding expert match.
*   **Reduction in Expert-Related Complaints:** 20% reduction in customer service tickets related to expert matching and transparency issues.

---

### 8. Release Plan & Phases

**Phase 1: Minimum Viable Product (MVP)** - Focus on core functionality for choice and transparency.

*   **Timeline:** 3-4 months
*   **Features:**
    *   **Basic Expert Listing:** Display a paginated list of experts with photo, name, primary specializations, and short bio.
    *   **Essential Filters:** Specialization, Availability (Day/Time), Language, Gender.
    *   **Expert Profile Page:** Comprehensive bio, credentials, therapeutic approach, and availability calendar with **fixed 20/40/60 minute session options** and existing pricing structure (no explicit tiered pricing yet).
    *   **Booking Flow:** Select expert, choose available slot and desired length, confirm, process payment (existing system), receive notifications.
    *   **"My Experts" Dashboard:** View current expert, upcoming sessions, and a prominent "Switch Expert" button.
    *   **Basic "Switch Expert" Flow:** Allow users to initiate a switch, showing a generic message about finding a new expert.
    *   **Expert Admin Portal:** Experts can manage their profile and availability.
*   **User Stories Covered:** 1 (partial), 2, 3 (partial), 5, 6 (partial).
*   **Success Metrics Focus:** Conversion Rate, First Session Satisfaction, Expert Switch Rate (early reduction), CS Inquiries (initial reduction).

**Phase 2: Enhancements & Optimization** - Refine the experience and introduce advanced capabilities.

*   **Timeline:** 3-6 months after MVP launch
*   **Features:**
    *   **Introductory Expert Videos:** Allow experts to upload short videos to their profiles (FR-5.2.2).
    *   **Client Feedback/Ratings:** Implement a system for users to rate and provide anonymous feedback on experts, displayed on profile pages (FR-5.2.4). Implement moderation queue for comments.
    *   **Advanced Filtering:** Introduce Price Tier filtering (if tiered pricing is rolled out separately), refine existing filters.
    *   **Smart Matching Suggestions:** Implement a basic algorithm that suggests experts based on user intake responses or Pathway progression.
    *   **Tiered Pricing Integration:** Allow experts (or OurRitual) to set different price points for different session lengths or based on experience level, reflected in the booking flow.
    *   **Enhanced "Switch Expert" Flow:** Provide more context and options when switching, including a brief survey to gather reasons for the switch.
    *   **Therapist-Specific Pathway Recommendations:** Experts can highlight specific Pathways they recommend for their clients.
*   **User Stories Covered:** 1 (full), 3 (full), 4, 6 (full).
*   **Success Metrics Focus:** Deeper reduction in Expert Switch Rate, increased ARPU (with tiered pricing), higher First Session Satisfaction, improved sentiment in reviews, sustained long-term engagement.

---
