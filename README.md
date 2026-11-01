# Keepline

Keep what your agent's session actually needs. Compact the rest.

**Status: early development.**

## Why

AI agents re-read their entire history on every turn. In long sessions, most of that history is bulk such as tool output, logs and abandoned attempts, so the cost climbs with every turn and answers get worse as the context fills with noise.

The usual fixes are blunt. Truncating drops things the agent still needed. Summarizing everything blurs exact details like names, numbers and error messages, and rewriting history can break prompt caching, so the bill sometimes goes up instead of down.

What is missing is a reliable way to tell what a session still needs, and to compact the rest without losing it.

## What Keepline does

1. **Compacts long sessions.** Keeps what the agent still needs and condenses the rest, so every turn is cheaper and the context stays clean.
2. **Loses nothing.** Original turns stay stored and can be recalled when the agent needs them.

