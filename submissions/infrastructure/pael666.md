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
I’ve been learning and experimenting with Web3 development, mostly by building small prototypes and testing new ideas. Recently I’ve been interested in tools that focus on verification and authenticity, especially as AI-generated content becomes harder to trust. ProofLens is a project where I want to explore how verifiable authorship can be made simple enough for anyone to use.

Project
Name & Category
Project: ProofLens

Category: infrastructure

Description
The idea behind ProofLens comes from a simple problem: it’s getting harder to know whether someone actually created the content they post. With AI tools everywhere, almost anyone can generate convincing text or images, and there’s no easy way to prove who made what.

ProofLens gives users a way to generate proof of authorship for their content. The app takes a piece of text or an image, turns it into a hash locally, and then asks the Soundness Layer to create an attestation linking the user to that hash. Other apps can later verify this proof without needing access to the original content.

It’s meant to be a small but useful building block that creators and developers can rely on when they need a trustworthy way to show that something actually came from them.

SL Integration
ProofLens uses the Soundness Layer to generate authorship attestations that are verifiable and tamper-proof.
The SL makes it possible to:

Create authorship proofs tied to a user without relying on a centralized database

Let third-party apps verify the proof independently

Validate ownership using a hash instead of the original content, keeping the user’s data private

The Soundness Layer essentially acts as the trust anchor that makes these claims meaningful and easy to verify anywhere.

Technical
Architecture
The system is built around three simple pieces:

Frontend: Users upload content, and the hashing happens locally so nothing sensitive leaves the device.

Backend: Receives the content hash and requests the attestation from the Soundness Layer.

Verification API: Lets other applications check whether a given hash matches a valid attestation.

Optional storage (like IPFS or WALRUS) may be used only if users want to persist their files, but it's not required for the core authorship proof.

Stack
Frontend: React / Next.js

Backend: Node.js

Blockchain: Soundness Layer

Storage: WALRUS / IPFS (optional)

Features
Local content hashing for privacy

Attestation creation through the Soundness Layer

Dashboard for users to view their proofs

Public verification endpoint for third-party integrations

Timeline
PoC (2–4 weeks)
 Basic hashing and attestation flow

 Initial SL integration

 Simple UI to upload content and display proofs

MVP (4–8 weeks)
 Full dashboard

 Public verification API

 Support for more content formats

 User testing and UX refinement

Innovation
ProofLens focuses on a problem that’s becoming more relevant every day: proving authorship in a world full of AI-generated content. Instead of trying to fight AI, ProofLens provides creators with a way to say, “Yes, I made this — and here’s the proof.”
It’s lightweight, private by design, and flexible enough for other developers to embed into their own apps.

Contact
Preferred contact: Discord (pa3l)
Updates will be shared on GitHub (@pael666)

Checklist before submitting:

 All fields completed

 GitHub username matches PR author

 SL integration explained

 Timeline is realistic
