Project: ProofLens
Category: Infrastructure
Developer: Raphael Pardamean (pael666)

Verification
github_username: "pael666"
discord_id: "pa3l"
timestamp: "2025-12-05"

Developer

Name: Raphael Pardamean

GitHub: @pael666

Discord: pa3l

Experience:
I’ve been exploring Web3 development and the idea of building tools that help people trust what they see online. I enjoy working on small prototypes, testing ideas quickly, and learning new frameworks along the way. Lately, I’ve been interested in systems that deal with verification and identity, especially as AI content becomes harder to distinguish. ProofLens is my attempt to create something useful and simple for creators and developers.

Project
Name & Category

Project: ProofLens

Category: Infrastructure

Description

It’s becoming harder every year to tell whether a piece of content truly comes from the person who claims to have created it. With the rise of AI-generated text and images, the internet is starting to feel full of things that look real but aren’t tied to any real creator.

ProofLens aims to provide a small, practical solution to that problem.
The idea is simple: let users prove that they created or own a specific piece of content — without needing to reveal the content itself.

A user uploads a text snippet or an image, the app turns it into a hash locally, and then Soundness Layer creates an attestation linking the user to that hash. The attestation can be verified by any other application later on.

It’s not meant to replace social platforms or marketplaces. Instead, ProofLens acts more like a building block — a small piece of infrastructure that developers can plug into their own apps when they want a reliable way to check if content really belongs to someone.

Soundness Layer Integration

Soundness Layer plays a central role in how ProofLens works:

Creating a trustworthy authorship proof
Instead of storing data in a centralized database, the attestation comes from SL.
This makes the authorship claim tamper-proof and independently verifiable.

Allowing verification without exposing the content
Only the hash is used.
Applications can confirm the attestation without ever accessing the original content.

Providing a neutral verification layer
No need to trust ProofLens itself.
The proof lives on SL, so any app can check it from there.

The SL essentially becomes the “trust backbone” of the system — the part that makes the attestation meaningful.

Technical
Architecture Overview

Frontend (React / Next.js)
A lightweight interface where users upload content.
The hashing happens locally, so the original file never leaves the browser.

Backend (Node.js or Rust)
Receives the hash and interacts with the Soundness Layer to create the attestation.
Only minimal data is stored — mostly for the user’s dashboard.

Soundness Layer
Generates and verifies all attestations.

Verification API
A simple endpoint that apps can call to check whether a specific content hash has a valid attestation.

Optional Storage (IPFS / WALRUS)
Only used if users want to permanently store their content, but not required for the core workflow.

Features

Local hashing for privacy

Attestation creation through SL

Dashboard to track all proofs created by the user

Public verification endpoint for third-party apps

Timeline
PoC: 2–4 weeks

Local hashing of content

First working attestation request to SL

Minimal UI to upload content and display proof

Simple verification endpoint

MVP: 4–8 weeks

Full dashboard for users

Public verification API

Support for multiple content formats

Basic UX polish and testing

Innovation

What makes ProofLens interesting isn’t that it’s a full platform — it’s that it tries to solve one problem cleanly:

“How do you prove you actually made something, without giving it away?”

Instead of fighting AI or building complex anti-bot systems, ProofLens leans on the idea of authorship as a cryptographic claim. Anyone can generate content, even AI — but being able to prove you were the one who submitted it first gives creators an advantage.

And because the entire proof system sits on the Soundness Layer, other apps don’t need to trust ProofLens. They can verify everything independently.

It’s a small piece of infrastructure, but one that can fit into social apps, marketplaces, creative platforms, identity systems, and even private communities where authenticity matters.

Contact

Preferred: Discord (pa3l)

Updates: GitHub (@pael666)
