# Integrity Scanner Data Handling and Safety Disclosure

Effective Date: June 24, 2026

This disclosure summarizes the data handling and safety boundaries for Integrity Scanner by Srdjan Lopez LLC dba Trinix AI.

This document is meant to help users, operators, reviewers, and Store reviewers understand what the App does and does not do.

## 1. Product purpose

Integrity Scanner is a local Windows desktop utility for integrity and posture review workflows.

It creates local report packets for operator review. It also supports local report verification, signature checks, trusted public key handling, optional challenge review, and admin intake workflows.

## 2. What the App does

Integrity Scanner may:

- Run local integrity and posture review workflows.
- Read locally available Windows security posture context.
- Read passive anti-cheat ecosystem context where available.
- Review selected local file paths and metadata where the workflow requires it.
- Generate local report files.
- Generate or verify signature sidecar files.
- Use trusted public key registries for verification.
- Display policy, warning, and confidence context for operator review.
- Export local report bundles selected by the user.
- Verify report bundles provided by a user or operator.

## 3. What the App does not do

Integrity Scanner does not intentionally:

- Certify that a device is clean.
- Confirm cheating.
- Confirm malware.
- Remove malware.
- Ban users.
- Disable devices.
- Delete files, drivers, or folders.
- Modify Windows registry values.
- Install kernel drivers.
- Perform enforcement actions.
- Run background monitoring.
- Run cloud scanning.
- Upload telemetry to Trinix AI by default.
- Sell user data.

## 4. Local report data

Reports may include technical context such as:

- Device and operating system information.
- Windows security posture context.
- Passive anti-cheat ecosystem context.
- File paths, metadata, hashes, and inventory status for selected or declared paths.
- Report timestamp and package metadata.
- Warning, policy, verifier, and challenge status.
- Public key and signature metadata needed for verification.

Users should review reports before sharing them.

## 5. Report verification limits

Verification confirms whether a report and signature match according to the verifier workflow and trusted key registry.

Verification does not prove that:

- A player is clean.
- A system has never been modified.
- All cheating methods are absent.
- All malware is absent.
- A challenge mismatch proves tampering.

Challenge mismatch is a policy issue that should be reviewed manually.

## 6. Private key rule

Never share private keys, PFX files, passwords, tokens, or full key folders for normal report review.

Normal review should use report files, signature sidecars, and public key material only.

## 7. Operator review rule

Operators should treat Integrity Scanner output as review context. Operators should not use the App as the only basis for punitive decisions.

Human review, event policy, user notice, and independent evidence should be used where decisions affect users.

## 8. Support contact

Questions, privacy requests, and support requests can be sent to:

`support@trinix.gg`
