# KAAM DAAR — Master Visual & Functional Reference

Status: APPROVED BY USER — use the uploaded 14-screen KAAM DAAR reference board as the source of truth.

## Non-negotiable design direction
- Match the user's reference board closely in both visual appearance and product flow.
- Keep the KAAM DAAR identity: rich natural green, white/off-white surfaces, charcoal text, yellow construction accents, real Indian worker photography/illustrations, polished phone-first UI.
- The reference is not a loose inspiration for a generic redesign. Do not replace it with a simplified landing page, generic cards, a different palette, or a CSS-only refresh.
- Keep the user's already-approved green preview's general palette unless the reference requires a specific adjustment.
- Do not change layout, copy, buttons, navigation, or established workflows without explicit approval.
- No emoji worker character as the main graphic. Prefer high-quality, consistent worker imagery/illustration that looks close to the reference.
- Animations must be visible and purposeful: splash/onboarding transitions, subtle landscape/worker motion, notification bell/pulse/countdown, button feedback, and screen transitions. Respect reduced-motion settings.
- Mobile-first; target the visual density, spacing, hierarchy, icons, bottom navigation and card treatment shown in the reference board.

## Required 14-screen product flow
1. Splash screen — KAAM DAAR logo, slogan, worker hero visual, short intro transition.
2. Onboarding — nearby work, trustworthy workers, clear next action.
3. Login (OTP) — Indian phone number entry and OTP flow. Do not claim real SMS works until a provider is configured and tested.
4. Role selection — Worker and Contractor cards with clear photography/illustrations and role labels.
5. Worker dashboard — greeting/profile completion, nearby pilot location/radius, notifications, quick navigation, available jobs.
6. Worker job details — job photo, pay/day, location/distance, date, requirements, details, apply action.
7. New-job notification — prominent alert, job summary, countdown/response window, accept/decline actions.
8. Contractor dashboard — post new job CTA, my jobs, applicant/assignment status, quick navigation.
9. Post job — title, skill type, number of workers, daily pay, date, district/location, description, submit action.
10. Nearby workers — map/list switch, worker cards, skills, rating, distance and contact/request action. Map must be labelled as demo if no real map/location service is active.
11. Worker profile — photo, skill, rating, verification status, experience/location, contact/request actions.
12. In-app chat — conversation UI, timestamps, composer and send action. Mark demo if messages are not persisted.
13. Earnings & history — weekly/monthly/all-time totals and recent work history; demo data must be labelled.
14. Bottom navigation — persistent Home, Work, Chat, Earnings, Profile navigation with active states.

## Functional expectations
- Worker and Contractor are separate roles and dashboards.
- Buttons must perform the action their labels promise; no decorative/inert controls.
- Job posting, applications, acceptance/decline, assignments, chat and earnings must be connected to real backend persistence before being described as production-ready.
- Demo-only features/data must be clearly labelled. Never imply OTP, notifications, maps, database persistence or matching are live when they are not.
- Preserve existing Supabase configuration and data; do not change DASTAVEZ production settings.
- Pilot remains 100% free: do not activate paid services, add billing, or introduce charges.
- Do not merge preview changes into production/main without the user's explicit approval.

## Implementation workflow
1. Treat the user's uploaded 14-screen board as the master acceptance reference.
2. Inspect the current app and map each existing screen/feature to the 14-screen flow before coding.
3. Implement in small, reviewable preview-branch changes. Keep approved colors/layout/buttons unchanged unless a specific reference mismatch needs correction.
4. Verify mobile layout and real button behavior; check browser output and deployment status before sharing a preview.
5. Describe exactly what changed and what remains demo-only. Do not call a deployment “complete” until its state is READY and the preview has been checked.
