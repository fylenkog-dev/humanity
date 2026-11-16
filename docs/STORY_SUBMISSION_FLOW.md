# HUMANITY — Story submission experience

_Status: product design specification; no submission functionality is implemented._

## Goal

Let a person prepare a story without pressuring them to disclose identifying or sensitive details. The author must understand the publication choice before any story can become public.

## Proposed journey

1. **Start with expectations**
   - Explain what HUMANITY is and what happens after a story is submitted.
   - State clearly whether the form is a private draft, a moderated submission, or a public post.
   - Never imply instant publication if editorial review is required.

2. **Write the story**
   - Required: story text.
   - Optional: title, display name, broad location, language, and topic.
   - Do not request legal name, exact address, phone number, date of birth, workplace, or identity documents for ordinary story sharing.
   - Give a reminder to remove details that could identify the author or another person unless sharing them is necessary and consented to.

3. **Choose attribution**
   - Suggested choices: display name, pseudonym, or anonymous to readers.
   - Explain that anonymous-to-readers does not necessarily mean technically unidentifiable to the service if operational data is collected.
   - Do not promise anonymity until the technical design and data practices can support that promise.

4. **Choose visibility**
   - Proposed pilot default: **private submission for review**, not public publication.
   - The author sees the exact visibility choice and can withdraw the submission before publication.
   - Public, unlisted, or community-only modes should not be offered until their access rules are implemented and tested.

5. **Review consent**
   - Show a preview of the exact text and attribution.
   - Separate consent to publish from acceptance of community rules.
   - Explain that publication may involve editing for safety or clarity; material edits should be approved by the author.
   - Never make consent to optional marketing or analytics a condition of submitting a story.

6. **Submit and confirm**
   - Provide a clear confirmation and a reference number if a real system is later built.
   - Explain the review process and realistic response expectations.
   - Provide a way to request withdrawal or deletion.
   - Do not claim a story was submitted, stored, or reviewed unless the backend confirms it.

## Suggested form fields

| Field | Requirement | Notes |
|---|---|---|
| Story text | Required | Set a reasonable limit only after usability testing |
| Title | Optional | Author-controlled |
| Display name | Optional | Pseudonym or anonymous-to-readers option |
| Language | Optional / inferred only with disclosure | Let the author correct it |
| Topic | Optional | Avoid sensitive profiling |
| Broad location | Optional | Country or region only; no precise location |
| Visibility | Required choice | Private review is the proposed pilot default |
| Publication consent | Required for publication | Separate, explicit, revocable before publication |
| Contact method | Not required by default | If needed for review, explain purpose and retention before collection |

## Validation and error states

- Preserve the draft locally only if the user has been told that it is stored on their device; otherwise do not imply persistence.
- Show errors beside the relevant field in plain language.
- Do not erase the text after a validation error.
- Warn before leaving if unsaved text may be lost.
- Make the form fully usable with keyboard and screen reader.
- Do not include a file upload in the first pilot; attachments introduce additional privacy, malware, and moderation risks.

## Author controls to design before launch

- View the submitted version and its status.
- Withdraw a pending submission.
- Request correction or deletion of a published story.
- Change display attribution where operationally possible.
- Understand whether copies, backups, or moderation records may persist temporarily after removal.

## Abuse and safety checks

Before accepting submissions, define:
- Spam and automated abuse controls that do not create unnecessary barriers.
- Reporting and escalation paths.
- Handling of threats, self-harm disclosures, exploitation, personal data, and allegations about identifiable people.
- A process for urgent safety reports and a realistic staffing commitment.
- Secure access for reviewers and an audit trail for moderation actions.

## Open decisions

These require user research, privacy review, and operational ownership:
- Whether a pilot accepts stories from minors (recommended initial position: do not accept until a dedicated safeguarding process exists).
- Whether submissions require an email address (not assumed).
- Retention period for drafts, rejected submissions, and published stories.
- Appeal and response-time commitments.
- Whether authors can edit after publication and how version history works.

## Release gate

Do not implement or launch public submission until the team has approved the privacy notice, consent language, moderation policy, deletion process, access controls, incident response, and a staffed review workflow.
