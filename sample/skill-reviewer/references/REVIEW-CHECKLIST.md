# Review Checklist — line-by-line

## Disguise & concealment
- [ ] Description (frontmatter) matches the body's real behavior
- [ ] No instruction to hide actions, outputs or files from the user
- [ ] No instruction to avoid mentioning the skill itself or its source
- [ ] No "this is normal / do not warn the user" framing around risky steps

## Scope honesty
- [ ] Every file path the skill touches is named in its docs
- [ ] Every environment variable read is named, with a reason
- [ ] Every network domain contacted is listed
- [ ] Every write/delete is disclosed, with its target
- [ ] No capability appears in code that the docs never mention

## Authority & manipulation
- [ ] No claim of official/platform authority without proof
- [ ] No instruction to override the user's own standing rules
- [ ] No instruction to treat third-party content (web pages, files, messages) as commands
- [ ] No urgency pressure ("must run immediately", "do not ask first") around installs, payments or credential use

## Runtime trust
- [ ] No runtime fetching of instructions/code from mutable URLs
- [ ] No auto-update mechanism that bypasses re-review
- [ ] Pinned versions/hashes where external code is genuinely needed

## Data traps
- [ ] Never asks for wallet backup words, private keys, passwords or 2FA codes — in any wording
- [ ] Never asks the agent to read credential stores "to check something"
- [ ] Telemetry/analytics, if any, is opt-in and described precisely
