Clutch Arena - go live in 3 steps

1. Upload index.html to Netlify (drag and drop) or Vercel. It must be opened from the
   hosted link, not inside a chat app preview, or the server (Supabase) will not connect.
2. Supabase project "Clutch Arena": Authentication > Providers > Email > "Confirm email"
   must be OFF (already done).
3. Open the live link. The badge on the home page should say "Live". Register a test
   account, book a slot, scan the UPI QR and send a test receipt.

Admin: to confirm payments and UIDs, open Supabase > Table Editor > registrations and set
payment_status to "paid" and uid_status to "verified". Screenshots are in Storage:
"receipts" (payment) and "profiles" (game profile, optional for players).

database/ = the base setup SQL (tables, rules, buckets). The live Clutch Arena project
already has it, plus later admin functions. Do NOT run these files again on that project.
Use them only to build a new Supabase project from scratch.
