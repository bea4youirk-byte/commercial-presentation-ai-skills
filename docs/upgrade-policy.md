# Upgrade policy

Use semantic versioning for each skill.

- Patch: wording, trigger clarity, QA precision, or compatibility note without changing the workflow contract.
- Minor: new reference module, new supported deck type, or additional QA gate that remains backward compatible.
- Major: changed task boundary, protected-content contract, evidence policy, or output expectations.

Before release:

1. Re-read current official Agent Skills documentation for supported hosts.
2. Validate every `SKILL.md` frontmatter and linked reference path.
3. Test trigger separation: translation, creation, upgrade, and audit must not invoke each other's destructive behaviors.
4. Forward-test at least one realistic request per materially changed skill.
5. Verify no private customer data, secrets, proprietary template code, or fabricated examples entered the repository.
6. Update `skills-manifest.json` with version and review date.

Never replace a working skill solely because a newer model exists. Upgrade only when the host format, tool boundary, observed failure mode, or business requirement changes.
