# ZITADEL startup program - Sourcey entity record

- **Pull request**: https://github.com/sourcey/startup-credits/pull/1276 adds one file, `entities/zi/zitadel.yaml`, with one new entity and exactly one offer. No code, no schema, no generated output, no unrelated files.
- **Offer**: Financial credits toward ZITADEL Cloud, all Cloud features and direct engineering sessions for the first 12 months.
- **Eligibility**: Less than $2M funding, no more than 2 years old, backed by an investor or accelerator.
- **Source**: https://zitadel.com/startup is the only cited source and is a page on the vendor's own domain. It was fetched and returned HTTP 200 on 2026-09-04. No directory or aggregator listing is cited.
- **Identity path**: the slug is `zitadel`, so the record sits at `entities/zi/zitadel.yaml`, shard and file name both derived from the slug. Fresh `ent_` and `off_` ULIDs, one file-local `source_id`.
- **Machine checks**: `sourcey/validation` success and `validate catalog change` success on the pull request head; the commit carries a DCO `Signed-off-by` line.
- **Local preflight**: the pinned Catalog Verifier reports `Sourcey verification passed (entities: 1, programs: 0, offers: 1)` against the repository root set and the live parent release.
- **sha256 of the entity file**: `f2f8788d4ad3782667a168c872a8aa2ae7b2f30cfb17e0ce426f0beb4d448a41`

## Entity YAML as committed

```yaml
schema_version: sourcey.entity-authoring/v1alpha1
entity:
  entity_id: ent_01m1nybq8qpz6bpzc6r7wtz2ct
  slug: zitadel
  slug_aliases: []
  name: ZITADEL
  domains:
    - value: zitadel.com
      role: primary
      valid_from: 2026-09-04T10:19:29.478Z
  category: auth-security
profile:
  description: ZITADEL is an identity and access management platform providing authentication, authorization, and multi-tenancy for developers as managed cloud or self-hosted software.
  links:
    site: https://zitadel.com
sources:
  - source_id: src_25f54f852ab833c8fb3ad75b9903c965461c2b5a37bdfee5ac45f75e18d0df41
    url: https://zitadel.com/startup
programs: []
offers:
  - offer_id: off_01m1nybq8q8qy5kjptseskndca
    offer_slug: zitadel-startup-program
    offer_slug_aliases: []
    title: ZITADEL Startup Program
    summary: Financial credits toward ZITADEL Cloud plus all Cloud features and direct engineering sessions for the first 12 months of an approved startup's participation.
    lifecycle:
      status: active
      effective_from: 2026-09-04T10:19:29.478Z
    economics:
      consideration:
        kind: unknown
        description: The source record did not establish separate consideration.
      benefits:
        - benefit_id: ben_primary
          description: Financial credits applied to a ZITADEL Cloud Team account, with all ZITADEL Cloud features available for the first 12 months
          kind: other
        - benefit_id: ben_support
          description: Direct engineering sessions with the ZITADEL team
          kind: other
    eligibility:
      rule:
        kind: manual
        criterion_id: cri_requirement_01
        statement: Company must have less than $2M in funding, be no more than 2 years old, and be backed by an investor or accelerator.
        reason: not-machine-evaluable
    roles:
      terms_authority_entity_id: ent_01m1nybq8qpz6bpzc6r7wtz2ct
      access_operator_entity_id: ent_01m1nybq8qpz6bpzc6r7wtz2ct
    access:
      availability: public
      method: form
      url: https://zitadel.com/startup
      instructions: Verify eligibility, register and submit the startup program form; ZITADEL assesses the application, sends details by email, and applies credits to the Team account.
    source_ids:
      - src_25f54f852ab833c8fb3ad75b9903c965461c2b5a37bdfee5ac45f75e18d0df41
```
