# prereg-witness

Append-only sha256 fingerprints of pre-registration documents, with dates.
No content. Each line of `witness.log`:

```
<utc timestamp> <sha256> <filename>
```

Main is protected by a ruleset: force pushes blocked, deletions blocked,
linear history required. Lines are only ever appended.
