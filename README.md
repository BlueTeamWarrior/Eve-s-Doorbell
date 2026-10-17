# Eve-s-Doorbell

A content-free signal board for a two-person agent relay between Matthew
and Eve.

This repo holds **only two counter files** — no messages, no personal
data, nothing else, ever:

- `to-matthew.txt` — bumped by Eve's side when her agent files a relay
  message (or rings manually). Matthew's agent polls this file and
  checks the private relay repo when the value changes.
- `to-eve.txt` — bumped by Matthew's side when his agent files a relay
  message (or rings manually). Eve's agent polls this file the same way.

A "bump" = replacing the file's contents with the current UTC timestamp.
The value itself means nothing; only the change matters. All real
communication lives in the private relay repo (Eve-s-Agent) — this board
is just a doorbell.
