# Text type: UX copy

Open this file for buttons, labels, form fields, error messages, empty states, tooltips and notifications – anywhere the text is part of an interface rather than something the reader sits down to read.
- Read with the audience rules in `SKILL.md` §3. Website length budgets do not apply.
- Microcopy is where the gender ladder is hardest and where GEN-01 step 1 does most of the work: name the action, not the actor.
- Link labels follow the website file (BTN-02); abbreviations follow MEC-06.

---

## 1 Buttons

**UXC-01 Verb first, four words maximum, naming what happens next** – not what the reader is agreeing to in the abstract. *Jetzt loslegen*, *Nachweis prüfen*, *Registrieren*.
- ✅ *Nachweis senden* · 🚫 *Weiter*
- ✅ *Anfrage ablehnen* · 🚫 *Abbrechen*, where the action is a refusal rather than an exit
- A pair of buttons uses parallel verbs. *Senden* and *Abbrechen* are not parallel; *Senden* and *Nicht senden* are.

---

## 2 Fields

**UXC-02 Mark optional fields, not required ones,** where most fields are required. The shorter set of markers wins.

---

## 3 Error messages

**UXC-03 Three parts, in this order: what happened, why, what to do next.** Drop the middle part when the cause adds nothing the reader can act on.
- ✅ *Der Nachweis ist abgelaufen. Fordern Sie einen neuen an.* · 🚫 *Ein Fehler ist aufgetreten.*
- Name the recovery path even when it is thin: *Versuchen Sie es später erneut* is more than *Fehler 500*. Where the reader cannot act, say who can.

**UXC-04 Never blame the reader.** Passive is allowed here (SND-03): it keeps the fault off the reader.
- ✅ *Der Code konnte nicht gelesen werden.* · 🚫 *Sie haben einen ungültigen Code eingegeben.*

---

## 4 Empty states and confirmations

**UXC-05 An empty state says what belongs here and how to get it,** in two sentences at most.
- ✅ *Hier erscheinen Ihre Nachweise. Fügen Sie den ersten hinzu, sobald Sie ihn erhalten haben.*

**UXC-06 Confirmations state the outcome, not the process.**
- ✅ *Nachweis gesendet* · 🚫 *Ihre Anfrage wurde erfolgreich verarbeitet*

---

## 5 Notifications and tooltips

**UXC-07 A notification says what changed and whether the reader has to act.** If no action is needed, say so; silence reads as an obligation.

**UXC-08 A tooltip explains in one sentence; it never instructs.** Anything the reader must do goes in visible copy, because a tooltip may never be seen. If it needs two sentences, the interface needs a change, not a longer tooltip.

---

## 6 Tone

**UXC-09 No apologies, no congratulations, no *Oops*.** Fix the problem or state the outcome; do not perform regret or delight. No *Geschafft*, no *Super*.

---

## 7 Length

**UXC-10 Avoid truncation.** Shorten the text instead.
- Where unavoidable – user-generated content, a name of unknown length – use an ellipsis and expose the full text in a tooltip.

**UXC-11 Check the longest language before the layout is fixed** (WRD-09). A label that fits in English may not fit anywhere else.
