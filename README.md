Most of my work lives in private repos, so this is how I build rather than what
I have pushed.

**Money state is derived, never typed.** Paid, underpaid and refunded are
computed from the payment records in integer centavos. Nobody sets a status by
hand, so nobody can set it wrong.

**Payment history is append-only.** The event log throws on update and delete.
Current state stays indexed and queryable; the narrative stays immutable. Both
halves are deliberate.

**Tests gate the deploy, not the commit.** A commit is a save point. The deploy
script reads the diff, decides which checks the change earns, runs them, and
refuses to push on red.

**Migrations are additive.** No dropped columns, no data rewritten in the same
change that ships a feature. Every migration is rehearsed against a restored
production dump before it runs for real.

**Comments explain why, not what.** A guard's docblock carries the incident that
created it and the date the rule changed. Delete the comment and the next person
deletes the guard.

---

**Stack** · PHP 8 · Laravel · Tailwind · JavaScript · MariaDB · SQLite · Pest · GitHub Actions

**Also** · embedded C — CAN bus, ISO-TP, UDS, ESP32 / RP2040

**Languages** · English · Filipino · Japanese (JLPT N4)
