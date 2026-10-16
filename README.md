# nexus-anchors

Daily chain heads of the Nexus conflict ledger (`gold.conflict_events`): one JSON line per asset per day with `anchored_at`, `asset`, `seq`, `chain_length` and `row_hash`. Written by `scripts/anchor_host.py` on the Nexus VPS after `verify_chain` recomputes the full hash chain; an invalid chain writes nothing. Entries up to 2026-09-30 were committed from the operator Mac before the VPS cutover. Rewriting ledger history now requires rewriting these git objects too.
