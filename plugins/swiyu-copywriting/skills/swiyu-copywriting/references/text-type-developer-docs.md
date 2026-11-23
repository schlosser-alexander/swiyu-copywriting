# Text type: developer documentation

Open this file for integration guides, API references, tutorials, code comments and release notes. The audience is `[DEV]`: people integrating swiyu, who want to finish a task and leave.
- The one text type where the plain-language rules (WRD-01, WRD-02) are relaxed: full technical vocabulary, each term introduced once, then assumed.
- Everything else in `SKILL.md` still applies, including SND-01, the gender rules, the glossary and claim checking.

---

## 1 Tone

**DOC-01 No marketing.** No benefit framing, no positioning lines, no *powerful* or *seamless*. The reader has already chosen swiyu.

---

## 2 Structure

**DOC-02 Each step ends with its expected result and carries its own failure modes.**
- State the expected result after each step that produces something visible. The reader needs to know whether to continue or to debug.
- Put the failure modes with the step that fails, not in a troubleshooting section at the end. A stuck reader does not scroll.

---

## 3 Code and identifiers

**DOC-03 Code samples run as written.** No pseudo-values that look real, no truncated payloads presented as complete, no placeholders the reader might paste unchanged.
- Mark placeholders unmistakably: `<your-client-id>`, not `abc123`.

**DOC-04 Prose around the code is translated; the code is not.** Identifiers, parameter names, error codes and field names are what they are in the API, in every language version. Comments inside samples stay in English.

---

## 4 Terminology

**DOC-05 Where the standard's term and the swiyu term differ, give both once,** then use the swiyu one. A reader from the specification needs the bridge; a reader working in swiyu needs consistency.

**DOC-06 Compound nouns are acceptable** where they are the established form in the field. WRD-03 protects general readers; it does not force *Eintrag im Vertrauensregister* into a schema description.

---

## 5 Claims

**DOC-07 OPS-04 applies, with a narrower source order:** for anything about a standard, the specification from the standards body settles it. Do not describe behaviour from memory of similar systems.
- Name the version or the date for anything that can change: endpoints, schemas, supported algorithms. Undated technical documentation ages invisibly.
- Do not document intended behaviour as current behaviour. Where something is planned, say so and say when it will be confirmed, or leave it out.
- Name the limits (VOI-05): what the API does not support, which algorithms are not accepted, which flows are out of scope. Developers discover these anyway; discovering them late is expensive.
