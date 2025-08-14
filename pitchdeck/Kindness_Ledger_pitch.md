# Kindness Ledger pitch deck
**Updated** August 15, 2025

## Slide 1  Title
Kindness Ledger  
A public memory for acts of kindness

## Slide 2  What it is
An open schema and a small SDK on the Ethereum Attestation Service that turn acts into portable signals.  
Media is stored with IPFS and Filecoin so content is addressable and easy to verify.  
The goal is a calm and useful public record that people can trust and reuse.

## Slide 3  How it works  data flow
Step one  a person records an act and captures optional media.  
Step two  the file is hashed and added to IPFS and can be replicated on Filecoin.  
Step three  the SDK creates an attestation on EAS that references the media by digest and stores time and a coarse location cell.  
Step four  a light read path or tiny index lists recent attestations and feeds a simple map and a curated stream.  
Step five  people can share their acts across apps which invites others to do something similar in their own way and at their own pace.

## Slide 4  Open schema and attestations
We use a compact schema for cost aware attestations.  
Fields include a media digest with codec info, time, a coarse grid cell, a category, an optional verifier and an optional campaign reference.  
The SDK hides the details and accepts a CID as input and returns a transaction hash and the schema UID.

## Slide 5  Storage and retrieval
Hash and upload produce a CID that never changes for the same content.  
Replication policies can pin on IPFS and place deals on Filecoin.  
Retrieval is verified through public gateways with a simple byte check and can be measured over time.

## Slide 6  Privacy and consent
Faces and real names are stored only with informed consent and a recorded consent reference.  
People can choose a public profile, a pseudonym or a private contribution.  
Location defaults to a coarse grid unless someone requests precision.

## Slide 7  Developer experience
One command demo that registers a schema or uses an existing one and creates a live attestation on a public test network.  
A simple read path that prints structured fields for recent attestations.  
Clear environment templates and short verification guides so reviewers can test in minutes.

## Slide 8  Scope and public good
This work focuses on open tools that others can reuse.  
Partners and sponsors are optional and come later and people never pay fees.  
All outputs are public and documented with proofs that anyone can verify.

## Slide 9  Milestones and budget
ESP total 24,000 USD across four milestones after activation.  
Filecoin total 36,000 USD across four milestones after agreement.  
Payments are milestone based and each deliverable is backed by public proof.

## Slide 10  Next steps after acceptance
ESP M1  fresh public run that yields a new schema UID and a new attestation transaction with a tagged release.  
Filecoin F1  hash upload and retrieval with a tagged release and a short verification note.  
Both repositories include STATUS and MILESTONES files and a folder for proofs.
