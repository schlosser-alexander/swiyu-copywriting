# Text type: UX copy

Open this file for buttons, labels, form fields, error messages, empty states, tooltips and notifications – anywhere the text is part of an interface rather than something the reader sits down to read.
- Read with the audience rules in `SKILL.md` §3. Website length budgets do not apply.
- Microcopy is where the gender ladder is hardest and where GEN-01 step 1 does most of the work: name the action, not the actor.

---

## 1 Buttons and actions

**UXC-01 Verb first, four words maximum.** *Jetzt loslegen*, *Nachweis prüfen*, *Registrieren*.

**UXC-02 The label names what happens next,** not what the reader is agreeing to in the abstract.
- ✅ *Nachweis senden* · 🚫 *Weiter*
- ✅ *Anfrage ablehnen* · 🚫 *Abbrechen*, where the action is a refusal rather than an exit

**UXC-03 A pair of buttons uses parallel verbs.** *Senden* and *Abbrechen* are not parallel; *Senden* and *Nicht senden* are.

**UXC-04 One primary action per screen.**

**UXC-05 No *Mehr erfahren* as a standalone label** (BTN-02). Where the design forces a short label, the heading above it carries the destination.

---

## 2 Labels and fields

**UXC-06 Field labels are nouns, not questions or instructions.** *Geburtsdatum*, not *Wann sind Sie geboren?*

**UXC-07 Label the field, not the format.** Format guidance goes in helper text below the field.

**UXC-08 Helper text says what is needed and why,** in one line, present tense.

**UXC-09 Mark optional fields, not required ones,** where most fields are required. The shorter set of markers wins.

---

## 3 Error messages

**UXC-10 Three parts, in this order: what happened, why, what to do next.** Drop the middle part when the cause adds nothing the reader can act on.
- ✅ *Der Nachweis ist abgelaufen. Fordern Sie einen neuen an.* · 🚫 *Ein Fehler ist aufgetreten.*

**UXC-11 Never blame the reader.** Passive is allowed here (SND-03): it keeps the fault off the reader.
- ✅ *Der Code konnte nicht gelesen werden.* · 🚫 *Sie haben einen ungültigen Code eingegeben.*

**UXC-12 No apologies, no exclamations, no *Oops*.** Fix the problem; do not perform regret.

**UXC-13 Name the recovery path even when there isn't one.** *Versuchen Sie es später erneut* is thin, but it is more than *Fehler 500*. Where the reader cannot act, say who can.

**UXC-14 Never expose an internal identifier as the whole message.** A code may accompany the message for support; it never replaces it.

---

## 4 Empty states and confirmations

**UXC-15 An empty state says what belongs here and how to get it,** in two sentences at most.
- ✅ *Hier erscheinen Ihre Nachweise. Fügen Sie den ersten hinzu, sobald Sie ihn erhalten haben.*

**UXC-16 Confirmations state the outcome, not the process.**
- ✅ *Nachweis gesendet* · 🚫 *Ihre Anfrage wurde erfolgreich verarbeitet*

**UXC-17 Confirmations do not congratulate.** No *Geschafft*, no *Super*.

---

## 5 Notifications and tooltips

**UXC-18 A notification says what changed and whether the reader has to act.** If no action is needed, say so; silence reads as an obligation.

**UXC-19 Tooltips explain, they do not instruct.** Anything the reader must do goes in visible copy; a tooltip may never be seen.

**UXC-20 A tooltip is one sentence.** If it needs two, the interface needs a change, not a longer tooltip.

---

## 6 Length and truncation

**UXC-21 Avoid truncation.** Shorten the text instead.
- Where unavoidable – user-generated content, a name of unknown length – use an ellipsis and expose the full text in a tooltip.

**UXC-22 Check the longest language before the layout is fixed** (WRD-09). A label that fits in English may not fit anywhere else.

**UXC-23 Never abbreviate to make something fit.** Rewrite it (MEC-06).
