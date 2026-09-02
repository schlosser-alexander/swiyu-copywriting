# Text type: developer documentation

Open this file for integration guides, API references, tutorials, code comments and release notes. The audience is `[DEV]`: people integrating swiyu, who want to finish a task and leave.
- The one text type where the plain-language rules (WRD-01, WRD-02) are relaxed.
- Everything else in `SKILL.md` still applies, including SND-01, the gender rules and claim checking.

---

## 1 Tone

**DOC-01 Precise and short.** Documentation is read mid-task. Every sentence that does not help the reader finish costs them time.

**DOC-02 Full technical vocabulary is allowed,** and preferred where the plain word would be less exact. *Endpoint*, *credential*, *issuance*, *presentation*, *claim* are the right words here.

**DOC-03 Introduce each term once,** at first use, in half a sentence. Then assume it. Never re-explain a term on the same page.

**DOC-04 No marketing.** No benefit framing, no positioning lines, no *powerful* or *seamless*. The reader has already chosen swiyu.

**DOC-05 Address the reader as *you*; use the imperative for steps.** *Send a request to …*, not *The developer sends …* or *One should send …*

---

## 2 Structure

**DOC-06 Prerequisites first.** What must exist before step 1 works: an account, a registration, a key, an environment.

**DOC-07 One task per page.** A page that covers issuance and verification covers neither well.

**DOC-08 Steps are numbered; each is a single action.** A step containing an *and* is probably two steps.

**DOC-09 State the expected result after each step** that produces something visible. The reader needs to know whether to continue or to debug.

**DOC-10 Put the failure modes with the step that fails,** not in a troubleshooting section at the end. A stuck reader does not scroll.

---

## 3 Code and identifiers

**DOC-11 Code samples run as written.** No pseudo-values that look real, no truncated payloads presented as complete, no placeholders the reader might paste unchanged.

**DOC-12 Mark placeholders unmistakably:** `<your-client-id>`, not `abc123`.

**DOC-13 Do not translate identifiers, parameter names, error codes or field names.** They are what they are in the API, in every language version.

**DOC-14 Prose around the code is translated; the code is not.** Comments inside samples stay in English.

**DOC-15 Name the version or the date** for anything that can change: endpoints, schemas, supported algorithms. Undated technical documentation ages invisibly.

---

## 4 Terminology

**DOC-16 The glossary applies here too,** including the checking-versus-verification split (WRD-07).

**DOC-17 Where the standard's term and the swiyu term differ, give both once,** then use the swiyu one. A reader from the specification needs the bridge; a reader working in swiyu needs consistency.

**DOC-18 Compound nouns are acceptable** where they are the established form in the field. WRD-03 protects general readers; it does not force *Eintrag im Vertrauensregister* into a schema description.

---

## 5 Claims

**DOC-19 OPS-04 applies, with a narrower source order:** for anything about a standard, the specification from the standards body settles it. Do not describe behaviour from memory of similar systems.

**DOC-20 Do not document intended behaviour as current behaviour.** Where something is planned, say so and say when it will be confirmed, or leave it out.

**DOC-21 Name the limits** (VOI-05): what the API does not support, which algorithms are not accepted, which flows are out of scope. Developers discover these anyway; discovering them late is expensive.
