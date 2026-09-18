# Frantic #120 - Hanko Startup Plan

One new vendor and one new offer contributed to `sourcey/startup-credits` as a
data-only pull request, merged and live on the Sourcey catalog.

- **Merged pull request, authored by the claimant.** [PR #1280](https://github.com/sourcey/startup-credits/pull/1280)
  was merged into `main` on 2026-09-18T08:46:27Z (head `b852abfc`, merge commit `6b3be107`),
  authored by GitHub user `codeboost-tr`, the claimant's verified GitHub identity.
- **One new vendor, one new offer, data only.** The merge adds exactly one file,
  [`entities/ha/hanko.yaml`](https://raw.githubusercontent.com/sourcey/startup-credits/6b3be107/entities/ha/hanko.yaml)
  (`sha256:066ad0fe5ac5c876928ba0838c7c6c532c6812875b6eb97bad44f6ebdb90b35c`), whose path
  follows the identity-derived shard rule (slug `hanko` -> `entities/ha/hanko.yaml`). It carries
  one entity and exactly one offer, with fresh `ent_`/`off_` ULIDs and one file-local `source_id`.
  No documentation, workflow or code file is touched.
- **Genuinely useful, currently available, startup-specific offer.** The Hanko Startup Plan gives
  one million free monthly active users on a Hanko Cloud organization (Free plan or Pro
  subscription), free consulting and setup support, and backlinks from Hanko's case study page,
  held for life or until the startup passes $500k ARR or raises more than $1M in VC funding.
  It is not a generic free tier or an ordinary trial: the Free tier's MAU limit is raised to
  1 million only for startups accepted onto the plan, which is applied for through a form.
- **First-party source, verified live.** The only cited source is
  <https://www.hanko.io/startup-plan>, on the vendor's own domain - not an aggregator, directory
  or affiliate listing. Refetched at HTTP 200 on 2026-09-18 with every figure in the record still
  present on the page.
- **CI, verifier and DCO all green.** On head `b852abfc`: `sourcey/admission` success
  ("Sourcey admission passed"), `sourcey/validation` success, `validate catalog change` success.
  Every commit carries `Signed-off-by: codeboost-tr <codeboost.tr@gmail.com>`.
- **Live on the Sourcey surface.** <https://sourcey.com/c/hanko> returns HTTP 200 and renders the
  record - Hanko, "Auth and security", www.hanko.io, 1 offer "Hanko Startup Plan" - with
  provenance "observed 18 Sept", entity revision `sha256:01de679c2c3a...` and offer revision
  `sha256:84e89d170d04...`.
- **Evidence review findings were fixed, not argued around.** Admission returned "needs revision"
  twice. The first run flagged `claim_unsupported` and `entity_summary_required`: `profile.summary`
  was missing, `consideration` declared `kind: unknown` with a description conceding the source did
  not establish it, two distinct source bullets were merged into one benefit, and the
  `free-service` named a service string that does not appear on the page. Those were corrected in
  commit `d1964b87`, taking supported claims from 20/30 to 28/32. The second run flagged
  `claim_contradicted` on the remaining benefit; its bound source range hashes to the sentence
  "Backlinks from our case study page to your domain to help with SEO", so commit `b852abfc` made
  the description quote that sentence. The third run admitted every fact.
