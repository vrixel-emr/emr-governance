# Security policy

This repository is public. It holds governance: the product's manifest, constitution, context,
architecture decisions, roadmap and postmortems. It holds no code, credentials or data.

## Reporting a vulnerability

Do not open a public issue. Use **Security > Report a vulnerability** on this repository
(GitHub private vulnerability reporting). Include what you found and the impact you expect. We
acknowledge reports within two business days.

## What never goes here

- Secrets of any kind: tokens, keys, passwords, connection strings. Push protection blocks the
  ones GitHub recognizes; the rest are on you.
- Patient or cardholder data, including in examples, postmortems and screenshots. Describe
  incidents with record ids and counts, never with the records themselves.
- Internal hostnames, IP addresses and account ids that would help an attacker.

## How changes are made

Pull requests only, reviewed by the code owners in `CODEOWNERS`. The Vrixel agentic SDLC tool
reads this repository and opens pull requests to it (new repos, architecture decisions, roadmap
records, postmortems); people approve them.
