# Contributing

Thanks for helping improve the Superhero developer docs.

## Before you open a pull request

1. `pnpm install` and `pnpm dev` to preview at http://localhost:3000.
2. Run `python3 scripts/lint-mdx.py`. It must report 0 issues. MDX errors break the whole build.
3. Every fact (an address, an endpoint, a fee, a parameter) must trace to source: the
   `superhero-com/superhero` web app, `superhero-com/superhero-agent-skill`,
   `superhero-com/superhero-api`, or the live API at `api.superhero.com`. For chain-level
   behavior, use the relevant æternity protocol, Sophia, SDK, AEX or middleware source listed
   in [README.md](./README.md#where-the-content-comes-from). Link the source and its release or
   commit in your pull request, and distinguish upstream behavior from production behavior.
4. New pages go in the right folder and in that folder's `_meta.json`.

## Writing style

- Plain, precise English. Short sentences. Second person ("you") is fine.
- Say what something does, not how impressive it is. No marketing language.
- No em dashes in prose; use a comma, colon or full stop.
- Code, addresses and endpoints go in backticks.

## What not to put here

- Security vulnerabilities. Report them privately; see [SECURITY.md](./SECURITY.md).
- Secrets, private keys or seed phrases, even test ones that hold funds.
- Speculation about prices or returns.

## Pull requests

Keep each pull request to one topic. CI builds the site and runs the linter on every pull
request; a maintainer reviews and merges to `main`, which deploys to developer.superhero.com.
