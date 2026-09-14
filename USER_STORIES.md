# Prismark — User stories

**Product:** [PRODUCT.md](./PRODUCT.md)


### Smart-contract developer

- As a Solidity developer, I want to submit bytecode from CI and get multi-label bug results before merge-to-main, so that I do not discover compiler defects after deployment.
- As a Solidity developer, I want findings mapped to specific bug families, so that I know which compiler upgrade or code rewrite to attempt first.
- As a Solidity developer, I want scans to work without uploading full private source when legal blocks it, so that security gates still run on bytecode artefacts.

### Security engineer

- As a security engineer, I want to batch-scan an entire release set and see a roll-up severity, so that I can decide go/no-go without opening dozens of tickets.
- As a security engineer, I want to override a false positive with a written rationale, so that the gate does not block a known-benign pattern forever.
- As a security engineer, I want model version pinned per project, so that a new model cannot silently change last week’s clearance.

### Release manager

- As a release manager, I want a single clearance certificate for the deploy, so that operations has an auditable artefact alongside the transaction hash.
- As a release manager, I want low-confidence results to block rather than pass, so that ambiguity never masquerades as safety.

### External auditor

- As an auditor, I want an export of prior automated findings and overrides, so that human review starts from machine triage instead of a blank page.
- As an auditor, I want to dispute a label and see it enter the vendor’s review queue, so that systematic errors get corrected upstream.

### Platform administrator

- As a platform administrator, I want to promote a new model only after family-level precision/recall thresholds pass, so that customers are not degraded by an unvalidated release.
- As a compliance officer, I want tenant isolation attested for pre-launch bytecode, so that we can answer enterprise security questionnaires.
