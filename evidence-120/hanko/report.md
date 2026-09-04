# Hanko startup program - Sourcey entity record

- **Pull request**: https://github.com/sourcey/startup-credits/pull/1280 adds one file, `entities/ha/hanko.yaml`, with one new entity and exactly one offer. No code, no schema, no generated output, no unrelated files.
- **Offer**: One million free monthly active users for a Hanko Cloud organization, plus free consulting and setup support.
- **Eligibility**: For life or until the startup passes $500k ARR or raises more than $1M in VC funding.
- **Source**: https://www.hanko.io/startup-plan is the only cited source and is a page on the vendor's own domain. It was fetched and returned HTTP 200 on 2026-09-04. No directory or aggregator listing is cited.
- **Identity path**: the slug is `hanko`, so the record sits at `entities/ha/hanko.yaml`, shard and file name both derived from the slug. Fresh `ent_` and `off_` ULIDs, one file-local `source_id`.
- **Machine checks**: `sourcey/validation` success and `validate catalog change` success on the pull request head; the commit carries a DCO `Signed-off-by` line.
- **Local preflight**: the pinned Catalog Verifier reports `Sourcey verification passed (entities: 1, programs: 0, offers: 1)` against the repository root set and the live parent release.
- **sha256 of the entity file**: `09e27a98ccf0fd6604910407ba955d1180808cfea232d82f19992dfc67750cb2`

## Entity YAML as committed

```yaml
schema_version: sourcey.entity-authoring/v1alpha1
entity:
  entity_id: ent_01m1nybq8qvtar05tbggk70yye
  slug: hanko
  slug_aliases: []
  name: Hanko
  domains:
    - value: hanko.io
      role: primary
      valid_from: 2026-09-04T10:19:29.478Z
  category: auth-security
profile:
  description: Hanko provides passkey-first authentication infrastructure with hosted login flows, user management, and an identity API for web and mobile applications.
  links:
    site: https://www.hanko.io
sources:
  - source_id: src_cc26ce4582876cab63a36fd6e38a0435fc7d85f16a459af1f85ccac2d0c9497e
    url: https://www.hanko.io/startup-plan
programs: []
offers:
  - offer_id: off_01m1nybq8q5c6ygc8m7tc6pgm0
    offer_slug: hanko-startup-plan
    offer_slug_aliases: []
    title: Hanko Startup Plan
    summary: One million free monthly active users on a Hanko Cloud organization, held for life or until the startup passes $500k ARR or raises more than $1M in VC funding.
    lifecycle:
      status: active
      effective_from: 2026-09-04T10:19:29.478Z
    economics:
      consideration:
        kind: unknown
        description: The source record did not establish separate consideration.
      benefits:
        - benefit_id: ben_primary
          description: One million free monthly active users for a Hanko Cloud organization on the Free plan or a Pro subscription
          kind: free-service
          service: Hanko Cloud monthly active users
        - benefit_id: ben_support
          description: Free consulting and setup support, plus a backlink from Hanko's case study page
          kind: other
    eligibility:
      rule:
        kind: manual
        criterion_id: cri_requirement_01
        statement: Applies for life or until the startup generates more than $500k in ARR or receives more than $1M in VC funding.
        reason: not-machine-evaluable
    roles:
      terms_authority_entity_id: ent_01m1nybq8qvtar05tbggk70yye
      access_operator_entity_id: ent_01m1nybq8qvtar05tbggk70yye
    access:
      availability: public
      method: form
      url: https://www.hanko.io/startup-plan
      instructions: Submit the startup plan form with name, email, company website, message, and the Hanko Cloud organization ID when one already exists.
    source_ids:
      - src_cc26ce4582876cab63a36fd6e38a0435fc7d85f16a459af1f85ccac2d0c9497e
```
