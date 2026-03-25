# Folder Watcher Agent (Observer Agent)

The Folder Watcher is a simple observer agent that monitors a specific folder for new text files. When a new file appears, it triggers a workflow to summarize the contents using a local LLM.

## Purpose

- Demonstrate the full agent → model → workflow → runtime pipeline.
- Provide a simple, explainable example of an observer agent.
- Act as the first “vertical slice” of R3@TH3 OS.

## Responsibilities

1. Monitor a folder for new `.txt` files.
2. Read the file contents.
3. Send the text to the Model Layer for summarization.
4. Save the summary to an output folder.
5. Log the action locally.

## Agent Type

- **Observer Agent**
- Runs on a predictable interval (e.g., every 5 seconds).
- No autonomous actions beyond its defined scope.

## Workflow Triggered

**Summarize File Workflow**

- Input: raw text file
- Output: summary file
- Model: local LLM (GPU accelerated)
- Storage: local-only

## Why This Agent First

- Safe
- Local-only
- Easy to test
- Demonstrates the entire OS pipeline
- Matches your philosophy of explainable, modular agents
