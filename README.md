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

`nexusswarm-suite-v4.tsx` is the verified source (73,722 B,
sha256 `479584ba69781bbfda4f73db241ee7e0751ba54f51c489ade4badd9f4093fd69`).
`bundle.js` is the built output of that file; `index.html` mounts it.
