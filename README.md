# PrepStar GH — Supabase-connected starter v3

This starter has been configured with the PrepStar GH Supabase project URL and its public publishable key. It includes a responsive dashboard, starter lesson cards, a practice quiz, account sign-up/sign-in UI, an empty non-fictional leaderboard, and WhatsApp share button.

## Use it
1. Extract this ZIP.
2. Host `index.html` on an HTTPS static host to test it on your phone. Opening a local file may not be enough for auth redirects or WhatsApp invitations.
3. In Supabase Authentication settings, set the allowed site URL and redirect URLs to your published site.
4. Try account registration with your own email and a strong, unique password. Confirm the email if prompted. Never share your password in chat.

## Security
The browser contains only the Supabase public publishable key, which is designed for client-side use. Never put a Supabase secret/service-role key in frontend code. Row Level Security remains essential.

## Current limitations
- Auth is configured in this file, but it must be tested from a hosted HTTPS URL.
- Profile creation relies on the `on_auth_user_created` trigger in the existing database.
- Quiz scores are not yet written to `learning_activity`, and the leaderboard intentionally shows no student names until a secure leaderboard policy/query is implemented.
- Lessons and quiz questions are starter examples, not a complete verified NaCCA curriculum. Have a teacher review content before public launch.
- Because students may be minors, involve a parent/guardian when setting up public hosting and review privacy, consent, and moderation before inviting other students.
