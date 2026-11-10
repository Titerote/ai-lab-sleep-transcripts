# ai-lab-sleep-transcripts

Raw session transcripts, shipped by hooks, filed `<project>/<session_id>/`:

```
<project>/<session_id>/
  main.jsonl          the user's session
  subagents/          agent-<id>.jsonl per subagent run
  probe/              hook probe logs copied from the project
  manifest.json       remote, commit, branch, cwd, host, first/last shipped, last event
```

Nothing here is edited by hand or by the dreamer; it reads, and
`dream-state.json` in `ai-lab-sleep-user` records what it consumed.
Retention: not yet; add a Mac launchd job that tars sessions older than N
days once the lab is done.
