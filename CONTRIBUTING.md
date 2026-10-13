# Contributing to Kryoto

Thanks for helping. This guide applies to every Kryoto-Dev repository unless the repository has
its own `CONTRIBUTING.md`.

## Set up

Most repositories expect their siblings next to them, so clone into one folder:

```bash
mkdir kryoto && cd kryoto
gh repo clone Kryoto-Dev/kryoto-desktop
gh repo clone Kryoto-Dev/kryoto-messaging
gh repo clone Kryoto-Dev/kryoto-padmap
# ...and whichever others you work on
```

Each README has the same sections: **Quick start**, **Layout**, **Checks** and how it ships.

## Making a change

1. Branch from `main` (or `master`), keep the change focused, and match the code around it.
2. Run the repository's **Checks** locally.
3. Open a pull request. CI must pass. Never push straight to `main`: on some repositories a push
   to `main` deploys or releases.
4. A change players will notice gets an entry in the kryo.to changelog (it also covers Desktop,
   dl.kryo.to and the Discord bot).

## Never commit

Secrets, tokens, private keys, `.env` / `.env.local` / `.dev.vars` files, logs, game files, or paths
from your own machine (`C:/Users/...`). Configuration goes in the git-ignored env file; each repo
ships an `.env.example`. If you committed a secret by accident, tell a maintainer straight away;
deleting the file is not enough, the secret has to be replaced.

## Questions

Ask in the Kryoto Discord, or open a draft pull request and ask there.
