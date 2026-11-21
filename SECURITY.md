# Security policy

This repository publishes the release archives of **TitheKit**, proprietary software for macOS by RenaCode, and
their SHA-256 checksums. It contains no source code. This file is a short copy of the TitheKit security policy; the
terms below are the same as in the full policy.

The full public policy is **https://tithekit.com/en/security/**. Advisories are published on
**https://tithekit.com/en/advisories/**. If this file and the website ever differ, the website is the current
version.

## How to report

The only channel for security reports is e-mail to **contact@renacode.com**, subject "TitheKit security".
E-mail is not encrypted. Please do not open a public issue, pull request or discussion in this repository, and keep
the details private until a fixed release is published or for 90 days from the acknowledgement, whichever comes
first, as described under "Coordinated disclosure" below.

Please include:

- the TitheKit version (`tithekit --version` or the release tag) and the macOS version;
- the affected component or, for a release archive, its file name and checksum;
- steps to reproduce or a proof of concept, and the impact you expect;
- whether you know of the vulnerability being exploited in the wild.

Do not send passwords, license keys or other secrets. If a secret is needed to reproduce the vulnerability, say so
without sending it, and we will agree with you on how to proceed.

## What happens next

- **Acknowledgement:** within 3 working days of receipt, counting working days in Poland (Central European Time).
- **Initial assessment:** within 10 working days: whether we confirm the vulnerability, how severe we consider it and
  the planned next step.
- **Updates:** at least every 14 days until the report is closed.
- **Fix:** shipped in a new release (see "Supported versions"). Its release notes name the fixed vulnerability.

If a reported vulnerability is actively exploited, RenaCode notifies the competent CSIRT and ENISA as required by the
EU Cyber Resilience Act (Regulation (EU) 2024/2847, Article 14) and informs affected users of the risk and of the
mitigations they can apply.

## Coordinated disclosure

- Please keep the details private until a fixed release is published or for 90 days from the acknowledgement,
  whichever comes first. If a fix needs longer, we explain why and may ask for a short extension, never for an
  open-ended delay.
- Once a fixed release is published, you may publish your findings. We publish an advisory at the same time or
  earlier.
- There is no bug bounty programme: we do not pay for reports. Public credit is given in the advisory and the release
  notes, unless you ask not to be named.

## Safe harbour

We will not take legal action against good-faith research that follows this policy: it stays on machines and accounts
you own, or is non-invasive testing of the tithekit.com website and domain (no load or denial of service, no access to
other people's data, no mass automated scanning and no social engineering); it does not read or change other people's
data, does not degrade services for others, and you report promptly. The scope of the policy is described in full at
https://tithekit.com/en/security/.

## Supported versions

Only the **latest release** receives security fixes. All earlier releases in this repository are **unsupported**
and may contain unpatched vulnerabilities; they are kept only as a historical archive. Do not install them for
regular use.

Before reporting, please check that the vulnerability still occurs in the latest release: update with
`brew upgrade tithekit` (Homebrew) or download the latest release from this repository. Check every archive against
its `.sha256` file.

## Advisories

Advisories for vulnerabilities in TitheKit are published in English when the fixed release is out, or earlier with a
mitigation when users need to act before the fix. All advisories: https://tithekit.com/en/advisories/
