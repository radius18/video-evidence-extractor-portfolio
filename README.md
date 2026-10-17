# Video Evidence Extractor — Multimodal Evidence & QA Workflow

A portfolio case study for a Python-based workflow that converts long-form video into structured, reviewable evidence packages for learning, technical research, workflow reconstruction, and evidence-based analysis.

**Status:** Work in progress · June 2026–Present

## Project Overview

Video Evidence Extractor (VEE) goes beyond a simple transcript summary. It combines transcript/caption extraction, local-media handling, FFmpeg frame capture, OCR, visual evidence selection, provenance and uncertainty records, quality gates, and reader-facing reports.

The goal is to preserve enough source evidence to support analysis while making uncertainty, incomplete coverage, and extraction failures visible instead of silently presenting them as complete results.

## Operator Interface

![Video Evidence Extractor operator interface](Screenshot%202026-10-16%20225935.png)

*Main VEE workspace for configuring video evidence extraction, analysis depth, purposes, outputs, critique level, and final-report generation.*

## Real-Source Extraction Configuration

![Real-source extraction configuration](Screenshot%202026-10-16%20231428.png)

*Example configuration for a technical AI-infrastructure video. The run is set up for structured learning, workflow reconstruction, prompt/code extraction, and portfolio-oriented analysis with explicit evidence and uncertainty requirements.*

## What the Workflow Produces

A VEE run can create a structured package containing:

- captions and cleaned transcript material
- raw and selected video frames
- OCR results
- prompt, artifact, and workflow candidates
- source traceability records
- confidence and uncertainty registers
- quality-gate and dependency checks
- reader-facing DOCX and Markdown reports
- selected visual evidence and visual snippets
- technical logs and preserved system artifacts

![Structured multimodal evidence package](Screenshot%202026-10-16%20230320.png)

*Generated run structure separating final deliverables, raw frames, selected screenshots, transcripts, evidence reports, uncertainty records, and technical artifacts for traceable review.*

## Final Deliverables

![Final evidence and intelligence deliverables](Screenshot%202026-10-16%20230837.png)

*Reader-facing output package containing DOCX and Markdown reports, selected visual evidence, visual snippets, package manifest, and supporting documentation.*

## QA, Provenance & Failure Handling

A major part of the project is not just extraction, but deciding when an extraction is trustworthy enough to continue.

Testing and refinement have focused on cases such as:

- failed or partial video acquisition
- sparse browser fallback coverage
- missing or incomplete temporal coverage
- missing OCR or transcript evidence
- false-green release states
- uncertainty that should be surfaced instead of hidden
- preserving raw/intermediate evidence for later review

The workflow was tightened so materially incomplete evidence can fail closed or be routed for review rather than being treated as a successful extraction.

![System artifacts and technical QA evidence](Screenshot%202026-10-16%20230713.png)

*Technical evidence layer showing FFmpeg chunk records, OCR outputs, extraction logs, manifests, confidence/uncertainty records, and other QA/provenance artifacts retained behind the reader-facing package.*

## Representative Validation

A real-source validation run demonstrated:

- 258 expected frame timestamps and 258 captured frames
- 0 missing timestamps and 0 failed intervals
- 258 OCR rows
- 28 selected screenshots
- full early / middle / late temporal coverage
- successful transcript extraction
- report-build gate passed
- 0 blocking findings
- packaged reader-facing outputs

The project also maintains regression tests around acquisition fallback, browser recovery, release gates, workflow state, and evidence integrity.

## Intended Uses

VEE is designed for situations where the value lies in more than a short summary. Potential uses include:

- **Self-directed learning** — turn a long tutorial or course into a structured learning package with concepts, screenshots, evidence, and next steps.
- **Technical research** — extract and organize architecture, commands, configuration, code, diagrams, and implementation details when supported by the source.
- **Workflow reconstruction** — map demonstrated processes from input to output and preserve the evidence used to infer each step.
- **Evidence-based analysis** — keep source screenshots, OCR, transcript material, confidence, and uncertainty connected to conclusions.
- **Study-material creation** — produce reusable notes, checklists, glossaries, and implementation plans from long-form material.
- **Portfolio and project research** — identify reusable ideas and patterns while keeping source evidence separate from interpretation.

## Skills Demonstrated

- Python workflow automation
- Multimodal evidence handling
- Quality Assurance / UAT
- OCR and transcript processing
- FFmpeg-based media processing
- Data extraction and normalization
- Provenance and traceability
- Failure-state design
- Quality gates and release logic
- Technical documentation
- Workflow design
- Structured reporting

## Portfolio Scope

This repository is a portfolio presentation of the project rather than the complete working VEE codebase or private project archive. The screenshots show representative interface, configuration, output, and QA/provenance evidence from the ongoing system.