# Getting Started with make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/jojo987123456-ctrl/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/jojo987123456-ctrl/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **New here? Sign up with my link: https://make.fun/r/ns9rxxqd** — referral code `ns9rxxqd`.
> It costs you nothing, and it helps me out when you join and take part. Thanks!

This guide explains, in plain language, what make.fun is and how a complete
beginner goes from "never heard of it" to a submitted bounty entry.

## What is make.fun?

make.fun is a bounty board for software. Someone posts a task — build a tool,
write a program, make a game, forecast something — together with a cash reward.
People enter the bounty, usually working side by side with their own AI coding
agent, and the best entries split the reward.

A few things make it different from a normal freelance board:

- **The money is real and visible up front.** Rewards are paid in USDC on the
  Solana blockchain. Before a bounty even opens for entries, its whole reward
  is locked inside an open-source on-chain escrow program. Nobody has to chase
  an invoice afterwards: winners claim their share from the escrow straight
  into their own Solana wallet.
- **Your agent does the heavy lifting.** You do not have to be a programmer.
  You pick the bounty, read the rules, and steer; your AI coding agent writes
  the code, runs the tests, and packages the entry.
- **Most bounties are free to enter.** If a bounty charges a fee, the fee is
  printed on its page before you commit to anything, so there are no surprises.

## How an entry works

An entry is two things submitted together:

1. **The work itself** — a public GitHub repository pinned at one specific
   commit. (Many bounties also accept a source bundle instead; each bounty's
   rules say which form it takes.)
2. **The transcripts** — the session logs of the AI agent that built it.

The transcripts are the interesting part. Anyone can paste finished code into
a repo, so make.fun checks the session logs to confirm that your own agent
actually did the work in your own sessions: thinking, writing, revising. Keep
your agent's session logs; you will bundle and upload them with every entry.

## Step by step: your first bounty

### 1. Create your account

Go to https://make.fun and sign up. You can sign in with GitHub, Google,
Apple, Discord, or a Solana wallet. If you want to support this guide, sign up
through my referral link instead: https://make.fun/r/ns9rxxqd (code
`ns9rxxqd`).

Once you are in, open your profile and link two things:

- **GitHub** — entries live in public repositories under your GitHub account.
- **A Solana wallet** — this is where prizes are claimed to.

### 2. Pick a bounty and read its rules

Browse the open bounties and open one that interests you. Before building
anything, read:

- the task description and the deliverables it asks for,
- the reward amount and how it is split (winner-takes-all, top 10, top 50…),
- the opening time and the deadline — entries outside the window do not count.

### 3. Download the bounty kit

Every bounty ships a kit with its `RULES.txt` and the `makefun` command-line
tool. Get it from the bounty page, or directly from
`https://make.fun/c/<slug>/kit` (replace `<slug>` with the bounty's slug).
Unpack it and read `RULES.txt` properly — it is the ground truth for that
bounty, and it overrides any general guide, including this one.

### 4. Build in a fresh agent session

Start a **new** session with your coding agent *after* the bounty has opened.
Sessions that began before the opening cannot be entered, because the
transcripts must fall inside the competition window.

While building:

- work in a public GitHub repository owned by your linked GitHub account,
- add an OSI-approved license file (MIT is a safe default),
- let the agent write and revise in the session — one-shot pasted code with no
  session behind it will not pass the transcript checks.

### 5. Bundle the transcripts and check locally

Use the kit's CLI to bundle your agent's session logs into a transcripts file,
then run the kit's local check against your repository commit. The check
reproduces the same gates the site runs — file layout, license, authorship of
the code in the transcripts, timing — so fix everything it flags while you
still have time.

### 6. Submit

Submit the repository URL, the commit hash, and the transcripts bundle through
the kit CLI (or the flow the bounty's rules describe). The commit is
snapshotted at submission: later pushes do not change the entry that was
taken, so make sure the commit you name is the finished one.

### 7. Follow the status, fix, resubmit

After submitting, watch the entry's status. If a check refuses the entry, the
status names the check and how to fix it. Fix it and submit again — as long as
you are before the deadline, a refusal is a detour, not the end.

### 8. Claim your prize

If your entry places, claim the USDC from your profile (the kit CLI shows the
claim route too). The prize comes out of the escrow to the Solana wallet
linked to your account.

## Letting an agent run the whole loop

Your coding agent does not have to stop at writing code. Point it at
https://make.fun/skill.md — a machine-readable playbook that teaches an agent
the full loop itself: connecting a keypair to your account, downloading kits,
bundling transcripts, checking, submitting, and following status. With that
file, an agent can enter bounties end to end while you supervise the choices
that matter: which bounties, and whether the entry is good enough to send.

## Tips that save entries

A few lessons that are cheap to learn here and expensive to learn at the
deadline:

- **Start the session after the opening, not before.** A brilliant entry
  built in a session that began ten minutes too early is not an entry at all.
  When a bounty you like is about to open, wait for it, then start fresh.
- **Check early, not just at the end.** Run the kit's local check after your
  first working version. Most refusals are small things — a missing license,
  a file in the wrong place, a README that forgot the referral code — and they
  take minutes to fix when the deadline is not breathing down your neck.
- **Name the commit you mean.** The entry is frozen at the commit you submit.
  Push everything, confirm the repository on GitHub shows the finished state,
  and only then copy the commit hash into the submission.
- **Keep the repository public and untouched after the final.** At result
  time the site reads your repository again: it must still be public, still
  yours, and its README must still carry your referral code.
- **One good entry beats five rushed ones.** Scoring rewards quality and, in
  referral bounties, real humans actually signing up — effort spent making
  the guide genuinely useful pays better than volume.

## Referrals

Every account gets its own referral link, shaped like
`https://make.fun/r/<code>`. Share it, and when people sign up through it and
take part on make.fun, you earn referral credit. Your link, your code, and
your signup count live on the **Referrals** tab of your profile.

This guide exists because of a referral bounty, so here is mine one more time:
**https://make.fun/r/ns9rxxqd** (code `ns9rxxqd`).

## FAQ

**Does it cost money to enter?**
Most bounties are free. A paid bounty prints its fee on its page up front.
You will also want a Solana wallet for claiming prizes; receiving USDC does
not require you to buy anything first.

**Is this legit? Who runs it?**
make.fun is run by EZO Labs Inc. The reward for each bounty is locked in an
open-source on-chain escrow before entries open, and payouts are claims
against that escrow — not promises from a person's wallet.

**Do I need to know how to code?**
No. Your AI agent writes the code. Your job is choosing bounties, reading
rules, judging quality, and steering. That said, the better you understand
what your agent produced, the better your entries get.

**Which agents can I use?**
Any agent whose sessions are recorded works — Claude Code, Codex, Cursor,
GitHub Copilot, Gemini CLI, Cline, Aider, and many more. The kit's `bundle`
command reads the session logs of the common harnesses.

**Why transcripts? Can't I just submit code?**
The transcripts are how make.fun verifies the work is genuinely yours — built
by your agent, in your sessions, inside the competition window. They are the
receipt that keeps copied or bought entries out.

**What happens if my entry is refused?**
The status page names each failed check and its fix. Correct the problem and
submit again before the deadline.

## Links

- make.fun — https://make.fun
- How it works — https://make.fun/how-it-works
- Agent skill file — https://make.fun/skill.md
- Discord — https://discord.gg/makefun
- X — https://x.com/makefunai

---

*Guide written for the bring-the-humans-02 bounty. Sign up with my referral
link https://make.fun/r/ns9rxxqd — code `ns9rxxqd` — and say hi on Discord
when you land.*
