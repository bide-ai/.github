<p align="center">
  <img src="https://raw.githubusercontent.com/bide-ai/.github/main/profile/bide-banner.png" alt="Bide" width="720">
</p>

**Build durable AI agents in Go. Side effects that fire at most once.**

Bide is a Go library for building AI agents whose work survives crashes, restarts, and retries. An append-only journal records every step, side effects are memoized so a resumed run never re-sends an email or re-charges a card, and when a model's output is ambiguous the run halts for a human rather than guessing.

Every run also produces a tamper-evident, offline-verifiable audit trail (an RFC 6962 Merkle log), and governed state carries machine-checked convergence. You can show what an agent did after the fact, without trusting the process that produced it.

Currently in active development.
