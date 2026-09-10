# Governance

**One thing it does well:** Consistently distinguishes confirmed data from unconfirmed
assumptions, holds that line even under direct pressure to state an estimate as fact (break-test
#2), and correctly handled a structural data trap — a repeated per-role constant that looks
summable but isn't — without being told the trap existed (break-test #6).

**One limit found in testing:** Testing did not surface a fabrication, but it also did not prove
the assistant is reliable on every possible query type — nine prompts, even adversarial ones,
cannot rule out failure modes that weren't tried (e.g., date-range calculations, cross-role
comparisons, or larger compound filters than the ones tested here). A clean testing record reduces
risk; it doesn't eliminate the need for spot-checks going forward.

**Data privacy:** The raw applicant dataset includes individually identifiable candidate
information (application dates, source, decision outcomes tied to Applicant_ID). This remains
inside the access-controlled ChatGPT project and is **not uploaded to this public repository**.
Public documentation here references aggregate findings only (role-level counts, rates, gaps).

**Accountability:** The assistant is a drafting and first-pass analysis tool, not a decision-maker.
Per the HW#3 brief's own decision-rights section, the HR Team Lead prepares and owns any
recommendation the assistant helps draft, and any pay-rate change still requires sign-off from the
Store #13 hiring manager and Finance. Given that this build has not yet been tested against every
possible query type, any number pulled from a multi-field or compound calculation should still be
spot-checked against the source sheet before it is used in a decision — particularly early in the
assistant's use, until a longer track record justifies more trust.
