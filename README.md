# ExamTopics JSON Cache

This repository hosts **easily accessible cached data** from the [ExamTopics](https://www.examtopics.com/) website in **raw JSON format**, auto-updated regularly.

## What is this?

- A structured JSON cache of ExamTopics exam questions.
- Automatically fetched and kept up to date.
- No HTML scraping or UI – just raw, structured data for programmatic use.

## Format

- Each exam (e.g., `az-900.json`, `aws-saa.json`) is a JSON file.
- Contains:
  - Question text
  - Options
  - Answer(s)
  - Explanations
  - Metadata like question ID, votes, tags (if available)

> Note: This repo currently only provides **raw JSON**. There is **no frontend** or web interface.

## 🛠 Parsing Tool

I also built a Go CLI tool called [`examtopics-downloader`](https://github.com/thatonecodes/examtopics-downloader) that **parses this JSON** and provides a terminal-based interface for:

- Viewing questions
- Filtering by tags or keywords
- Exporting to nicely formatted markdown file
