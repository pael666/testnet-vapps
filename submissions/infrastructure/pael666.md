# vApp Submission: ProofLens

## Verification
```yaml
github_username: "pael666"
discord_id: "pa3l"
timestamp: "2025-12-05"
Developer

Name: Raphael Pardamean

GitHub: @pael666

Discord: pa3l

Experience:
I’ve been experimenting with Web3 development by building small prototypes and exploring tools related to verification, identity, and content authenticity. Lately I’ve been interested in how creators can prove authorship in a simple and privacy-friendly way, which led me to build ProofLens.

Project
Name & Category

Project: ProofLens

Category: infrastructure

Description

It’s becoming harder to know whether someone genuinely created a piece of content, especially with AI tools everywhere. ProofLens gives users a simple way to prove authorship of text or images without exposing the content itself. The app generates a local hash, then uses the Soundness Layer to create an attestation that links the user to that hash. Other apps can verify this proof independently.

SL Integration

ProofLens relies on the Soundness Layer to produce verifiable authorship attestations. The SL allows users to create proofs that are tamper-proof and can be validated without needing the original content. Third-party apps can check these attestations directly through SL, making the authorship claim portable and trustworthy.

Technical
Architecture

The flow is straightforward:

The frontend handles content upload and hashing locally.

The backend receives the hash and interacts with the Soundness Layer to generate the attestation.

A verification endpoint lets other apps confirm whether a hash has a valid proof attached.
Optional storage (like WALRUS/IPFS) can be used if users want to store their content, but it isn’t required.

Stack

Frontend: React / Next.js

Backend: Node.js

Blockchain: SL

Storage: WALRUS / IPFS (optional)

Features

Local content hashing for privacy

Authorship attestation through SL

User dashboard to view proofs

Timeline
PoC (2-4 weeks)

 Basic functionality

 SL integration

 Simple UI

MVP (4-8 weeks)

 Full features

 Production ready

 User testing

Innovation

ProofLens focuses on a practical problem: proving content ownership in a world filled with AI-generated material. Instead of trying to detect AI or block automation, it gives creators a way to show, “I made this, and here’s verifiable proof.” It’s small, simple, and something many applications can build on.

Contact

Preferred contact: Discord (pa3l). Updates will be shared through GitHub (@pael666).
