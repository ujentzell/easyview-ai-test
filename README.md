# AI download test feed

A personal public sandbox for testing a model catalogue and text-only instruction updates.
This is not an application release repository or an official product feed.

## Files

- `instructions.json`: a versioned bundle of generic, draft measurement interpretation instructions.
- `models.json`: one small download-test model, linked to its original publisher at a fixed revision,
  with the publisher's byte size and SHA-256. Model weights are not stored here.

The linked [Qwen3 0.6B GGUF model](https://huggingface.co/Qwen/Qwen3-0.6B-GGUF) is published under
Apache-2.0. Its model card and licence remain with its publisher. The catalogue's memory figure
is a conservative test estimate, not a measured requirement. This small model has not been
qualified for Swedish measurement analysis; it exercises catalogue and download plumbing.

## Updating the test instructions

Edit the text in `skills`, increase that instruction's `version`, then increase the bundle's
`revision`. Keep the JSON valid. The app retains its last valid publication if a later one is
malformed, and keeps personal instructions separately. `status: draft` means the text is awaiting
review. This repository contains generic test text only.

## Publication boundary

Only this README, `models.json`, and `instructions.json` belong in this repository. Do not add
application source code, installers, application binaries, application-update manifests, private
measurement data, credentials, company instructions, or private repository history. Application
updates are outside this test feed. No GitHub Actions or deployment workflow is installed.

Raw feed addresses:

- https://raw.githubusercontent.com/ujentzell/easyview-ai-test/main/models.json
- https://raw.githubusercontent.com/ujentzell/easyview-ai-test/main/instructions.json
