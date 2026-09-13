# Charter — philanthropisch

> **Status: DRAFT.** Only §4 is written. Everything else waits on the listening
> probe, because what this venture *does* should come from what people need.
> Leg 1 of 3. Template: [CHARTER](https://github.com/bcroner/RZN_AI_PATENT_PORTFOLIO_TRIFECTA_OPTIMAL_AUTOPILOT/blob/main/templates/CHARTER.template.md).

Delete no headings — an empty section is information.

---

## 1. Thesis

**One sentence.** What this venture is, for whom, and why it should exist.

> [FILL]

**The test:** if an agent can read this sentence and still build the wrong
thing, it is not specific enough yet.

**Evidence of need:** none yet. The first listening probe is in design:
[needs/food-insecurity/PROBE.md](needs/food-insecurity/PROBE.md).

Both answers are legitimate. The second one simply means this Charter carries
an untested assumption, and the first probe worth running is the one that tests
it.

---

## 2. Outcome — what "a running, working company" means here

Not aspiration. The observable state at which this venture is *done being built*
and is merely being operated.

| Dimension | Target | How it is observed |
|---|---|---|
| Customers | [FILL] | [FILL] |
| Revenue | [FILL] | [FILL] |
| Uptime / service level | [FILL] | [FILL] |
| Operating cost ceiling | [FILL] | [FILL] |
| Hours of operator attention per week | [FILL] | [FILL] |

The last row is the one that matters most. If it does not trend toward zero,
this venture is a job, not an asset (Principle 9).

---

## 3. Definition of Shipped

The acceptance criteria the Judge will enforce. Write these so a machine can
check them. Anything a machine cannot check belongs in §7 instead.

- [ ] [FILL: e.g. "All flows in `test/e2e/` pass against a production-like env"]
- [ ] [FILL]
- [ ] [FILL]

**Rule:** if a criterion cannot be phrased as a command that exits 0 or 1, it is
not a shipping criterion. It is a taste judgment — move it to §7.

---

## 4. Non-negotiables — what this venture will never do

A Charter that forbids nothing has not been written yet. These are absolute and
outrank every other instruction, including a later instruction from the
operator that arrives mid-run.

### Help carries no strings

The people this venture serves owe it nothing. That is the whole of the rule;
the list below is how it is kept.

- **Never** make help conditional on attendance, membership, faith, belief,
  conversion, or sitting through religious or any other messaging.
- **Never** ask the people served to repay, volunteer, or give anything in
  exchange for help.
- **Never** require anyone to share their story, photo, or name for fundraising
  or publicity. Sharing is only ever by separate, freely given, revocable
  consent, and declining changes nothing about the help they receive.
- **Never** sell or share information about the people served, or use it for
  fundraising, marketing, or anything other than delivering help.
- **Never** give donors a say in which individuals are helped, or any way to learn
  who they are.
- **Never** ask the people served for public thanks or recognition.
- **Never** measure success by how much people use the help. Measure need met
  (Principle 11: meet needs, never manufacture wants).
- **Never** decide what a community needs without asking it (Principle 12: offer,
  never impose).

### "No expectation of return" means the people served, not the people serving

Everyone has bills to pay. Staff, hosts, listeners, interpreters, and partner
organizations are **paid fairly** for their work, and the budget says so. Volunteers
are welcome, but no core role depends on unpaid labor, and no one's generosity
is taken for granted.

An agent that finds itself required to violate one of these must halt (§8), not
find a clever way around it.

---

## 5. Constraints

| | |
|---|---|
| Stack / platform | [FILL] |
| Monthly budget ceiling | [FILL] |
| Legal & regulatory regime | [FILL: jurisdictions, licences, data-protection law] |
| IP posture | [FILL: default is RZN AI proprietary — see repository LICENSE] |
| Brand voice | [FILL, or link to the voice playbook] |
| Dependencies that must not be added | [FILL] |

---

## 6. Blast radius — the golf clause

This section is what lets the operator leave. Be conservative: every expansion
must buy its way in with a reason.

**The fleet MAY, unattended:**
- [FILL: e.g. "open branches and PRs in `<repo>`"]
- [FILL: e.g. "deploy to the `staging` environment"]
- [FILL]

**The fleet MAY NOT, ever, without a morning gate:**
- Touch production data or production infrastructure
- Move money, incur charges beyond the §5 ceiling, or alter billing
- Contact a customer, publish publicly, or send on the operator's behalf
- Rotate, read, or exfiltrate credentials
- Alter this Charter, the Harness, the Judge, or the repository LICENSE
- [FILL: venture-specific additions]

**Credentials available to the fleet:** [FILL — least privilege; name each and
what it can reach. If a credential can do something in the MAY NOT list, it is
the wrong credential.]

---

## 7. The eligibility sort

Per Principles — the sort is most of the engineering. Classify the *kinds* of
work this venture generates.

**Autopilot-eligible** — machine-checkable done, runs overnight:
- [FILL: e.g. "feature implementation against a written spec"]
- [FILL: e.g. "test coverage, migrations, dependency upgrades, infra as code"]

**Cockpit-required** — the operator decides, briefly, in the two hours:
- [FILL: e.g. "is this the right feature at all"]
- [FILL: e.g. "pricing, positioning, anything a customer reads"]

**Default when unclear:** cockpit-required. Misrouting *up* costs ten minutes of
operator time. Misrouting *down* costs a night and, worse, buys false trust.

---

## 8. Halt protocol

When an agent does not know, it stops and asks. It does not improvise
(Principle 7). A night that halts with a good question is a successful night.

Questions land in: `instances/<venture>/QUESTIONS.md`

**Halt immediately on:** a §4 non-negotiable in the way · an ambiguity in §3
that changes what gets built · anything requiring a §6 gate · a third
consecutive failure of the same approach.

---

## 9. Open questions

Carried between nights. The operator burns these down in the cockpit hours.

| # | Question | Raised | Blocking? | Answer |
|---|---|---|---|---|
| 1 | [FILL] | [date] | yes/no | |

---

## 10. Revision log

Every change records its *why*, so an inheritor can tell which rules are load-
bearing and which were circumstantial (Principle 10).

| Date | Change | Why |
|---|---|---|
| 2026-09-12 | Charter created with §4 non-negotiables only | Operator: serve others without any expectation of return from those served, while paying those who do the work |
