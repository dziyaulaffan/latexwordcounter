# LaTeX Word Counter

A browser-based LaTeX word counter built for academic writing with strict word limits.

## Why This Exists

Existing word counting solutions fail LaTeX documents. General text editors count commands and preamble as words. Compiling to PDF and running `texcount` is accurate but cumbersome for quickly checking against a word limit.

This tool provides a fast, transparent alternative that runs entirely in your browser.

## Features

- **Single-pass parsing** of LaTeX source with no compilation required
- **Selective counting** - choose which elements to include (body text, footnotes, captions, etc.)
- **Colour-coded verbose view** showing exactly how each part of your document was classified
- **Handles LaTeX structure properly** - recognises preamble, citations, math environments, tables, figures, bibliography entries
- **Complete privacy** - all processing happens client-side, nothing is uploaded or stored

## Usage

Open the HTML file in any browser, paste your LaTeX source, and get an accurate word count instantly. Toggle element types to match your assignment's counting rules.

## Technical Details

Pure HTML/CSS/JavaScript implementation with no external dependencies or server requirements. The parser performs structural analysis of `.tex` files, assigns typed tokens to each element, and computes counts based on user-selected categories.

Built to solve a real problem: trusting a word count tool with binding submission limits for coursework.

## Privacy

No LaTeX source is transmitted, uploaded, or stored. The tool is a self-contained HTML file with zero external connections.
