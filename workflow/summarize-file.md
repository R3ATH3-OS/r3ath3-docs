# Summarize File Workflow

This workflow is triggered by the Folder Watcher Agent when a new `.txt` file appears in the watched folder.

## Purpose

- Provide a simple, local-first example of a workflow.
- Demonstrate how agents call models.
- Show how outputs are stored and logged.

## Inputs

- Raw text file path
- File contents

## Steps

1. Read the file contents.
2. Send the text to the Model Layer for summarization.
3. Receive the summary from the local LLM.
4. Save the summary to an output folder.
5. Write a log entry describing the action.

## Output

- A new `.summary.txt` file containing the generated summary.

## Model Used

- Local LLM (GPU-accelerated)
- Small, fast model recommended for this workflow

## Why This Workflow Matters

- It demonstrates the full agent → model → workflow pipeline.
- It is safe, predictable, and explainable.
- It becomes the template for future workflows.
