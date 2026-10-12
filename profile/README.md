<p align="center"><img src="gitorange-logo.png" alt="GitOrange" width="360" /></p>

The code host for teams where coding agents write the code and people approve the risk. Self-hosted, as one
Cloudflare Worker with every repository in Cloudflare Artifacts. We build GitOrange on GitOrange.

When fifty agents open pull requests at once, three things break. GitOrange fixes each one:

1. **It works out what depends on what.** Agents edit the same files. GitOrange builds a dependency graph of every
   open pull request: Clef, a decision model on Workers AI, decides which pairs are related, git confirms stacks, and
   every pull request lands in the right order.
2. **People review decisions, not diffs.** Reviewers are agents, each a versioned git repository with its own rules,
   and they learn from your answers. A person sees a plain yes/no question with a before and after table and an ERD or
   sequence diagram.
3. **It merges everything itself.** Rebase only, so history stays linear. GitOrange keeps branches rebased, lands
   them safely when several agents finish at once, and AI resolves conflicting commits.

**Get started:** [github.com/choyiny/gitorange](https://github.com/choyiny/gitorange)

**Reviewer agents** used on GitOrange itself, ready to add to your instance:
[Data](https://github.com/gitorangeapp/dataagent) ·
[DevOps](https://github.com/gitorangeapp/devopsagent) ·
[Feature](https://github.com/gitorangeapp/featureagent) ·
[Security](https://github.com/gitorangeapp/securityagent) ·
[Speed](https://github.com/gitorangeapp/speedagent)
