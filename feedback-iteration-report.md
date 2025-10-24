# Feedback Iteration Report

## Summary of Identified Issues & Recommendations

| # | User Feedback | Proposed Improvement | Potential Constraints | Priority |
|---|----------------|----------------------|------------------------|-----------|
| **1** | After selecting “Login with Apple,” the screen stays on the previous page instead of moving forward. | Automatically transition to a loading screen with a “Logging you in…” message. | Requires integration changes with Apple login API flow; minor development effort. | **High** |
| **2** | The “Allow notifications” screen is confusing because it shows a screenshot of a notification rather than the system permission prompt. | Replace screenshot with a clear, native permission prompt and a brief explanation of benefits. | Might need design changes and alignment with iOS/Android notification permission UI rules. | **High** |
| **3** | The “What do you want to improve?” question feels like a big ask early on; users expect to first understand how the app can help. | Reframe as “Here’s how we can help you improve…” followed by examples or guided choices. | Requires copy and flow adjustments; minimal development cost. | **Medium** |
| **4** | Clicking “Open Focus Bear” from the YouTube locked screen sometimes triggers a notification rather than opening the app directly. | Clarify expected behavior in UI and ensure predictable app response, or remove that option. | Could require debugging notification triggers; moderate effort. | **High** |
| **5** | “You have earned your screen time” message may feel awkward for adults. | Personalize language based on user profile (e.g., age group, goal type). | Needs personalization logic; moderate complexity. | **Medium** |
| **6** | Habits are limited; users can’t easily add their own. | Allow custom habit creation during setup and in settings. | Higher development effort; may require database changes. | **Medium** |
| **7** | Onboarding feels too long. | Combine steps and offer an option to skip non-essential parts. | Must balance business need for data collection vs. user impatience. | **High** |
| **8** | Privacy policy reading step is long; most users won’t read it. | Add a small checkbox acknowledging the policy in the main flow to reduce extra steps. | Legal team approval needed; minimal technical effort. | **Low** |

## Prioritization Rationale

- **High Priority:** Immediate usability issues disrupting flow or causing confusion (Items 1, 2, 4, 7).  
- **Medium Priority:** Improvements to tone, personalization, and flexibility that enhance experience but don’t block usage (Items 3, 5, 6).  
- **Low Priority:** Efficiency improvement constrained by legal requirements (Item 8).


## Balancing Feedback with Constraints

- **Business Goals:** Maintain essential onboarding data for engagement and retention.  
- **Technical Feasibility:** Avoid large refactors for minor gains.  
- **User Value:** Prioritize fixes that directly reduce friction and confusion.

## Next Steps

1. Implement quick wins first — Items **1, 2, 4, and 7** offer high impact with relatively low effort.  
2. Collaborate with PMs and developers to explore feasible solutions for habit customization and personalized messaging.  
3. Test revised flows with users to confirm improvements before release.

## Reflection

### If a UX change helps users but conflicts with business goals
I would start by showing how the change supports long-term business success, using real user quotes or quick data points. Then, I’d look for a middle ground—such as phasing the change gradually or adjusting the approach to serve both users and business needs.

### Working with PMs and Developers to Find Compromises
It’s important to collaborate early and be transparent about constraints. I’d present a few design options with pros, cons, and effort levels so the team can select the most balanced solution. Often, starting small and iterating later is the most practical approach.

### Risks of Making Too Many Small UX Changes Too Quickly
Frequent small changes can confuse returning users, create inconsistency, overload developers, and make it harder to measure the impact of any single change.

---

