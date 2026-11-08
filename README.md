# NexusSwarm

Multi-agent collaboration suite, v2.0 [VFS INDEXEDDB].

Three agents — Nexus-Architect, Builder-Prime, Inquisitor-QA — run in rounds
on a Prime Directive task, sharing a canvas and a workspace filesystem
backed by IndexedDB. Also includes an Agents roster and a Viz analytics tab.

## Run

Open the deployed site (or serve this directory statically) and type a
Prime Directive, then Initialize Swarm Sequence.

## API key

The app calls the Gemini API directly from the browser. It needs your own
Gemini API key (free from Google AI Studio), pasted into the API Key field
in the app. The key lives only in memory while the page is open. The
Canvas Preview version of this app used Google's environment-injected auth;
that does not exist outside Canvas.

## Source

`nexusswarm-suite-v5.tsx` is the verified source (81,542 B,
sha256 `25f064a7c83c4c7399abc693ec410116ccd9e2b20829d056a918bfed6d56f229`).
`bundle.js` is the built output of that file; `index.html` mounts it.
v5 adds sandboxed JavaScript code execution: agents can run a `.js`
workspace file through an `executions` field, and the Workspace tab has
a Run button plus a RUN OUTPUT panel (Web Worker runner, 5s timeout).
