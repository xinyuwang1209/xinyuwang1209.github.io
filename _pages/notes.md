---
layout: archive
title: "Engineering Notes"
permalink: /notes/
author_profile: true
---

Short notes on practical systems debugging, open-source patches, and reliability work around ML systems and coding-agent infrastructure.

## Codex Memory-Fix Fork

**Context:** Codex Desktop stores local session history as rollout JSONL files. Very large files can create memory pressure when startup metadata backfill or full history loading reads too much into memory at once.

**What I changed:** I maintain a small unofficial fork that streams rollout metadata extraction line by line, reuses legacy snapshot filtering, and adds a 512 MiB guard for full thread-history loads.

**Why it matters:** The patch is intentionally narrow, but it captures a reliability boundary that appears in local agent infrastructure: large local state, startup backfills, memory blowups, and platform-specific packaging constraints.

**Caveat:** This is not an official Codex distribution. Patched macOS Desktop builds may not preserve OpenAI's Developer ID signature, which can affect Computer Use helpers in local builds.

[GitHub repo](https://github.com/xinyuwang1209/codex-memory-fix){: .btn}
