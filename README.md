# Humanizer Skill for Gemini CLI

This is a port of the [blader/humanizer](https://github.com/blader/humanizer) skill for Gemini CLI.

## Overview
Bored of doing shallow work? Make it fun with your favorite AI partner!

The Humanizer is a specialized writing editor designed to remove the "statistical average" feel of AI-generated text. It identifies and fixes 29 distinct "AI-isms" across content, language, style, and communication patterns.

## Contents

- `humanizer.skill`: The packaged skill file ready for installation.

## Installation

To install this skill in your Gemini CLI:

1.  Open your terminal in the directory where the `.skill` file is located.
2.  Run the installation command:
    ```bash
    gemini skills install humanizer.skill --scope user
    ```
    *(Use `--scope workspace` if you only want it for a specific project folder)*
3.  In your active Gemini CLI session, reload your skills:
    ```bash
    /skills reload
    ```

**Or just tell it this simple message : I want to use EfeAtesh/humanizer-GeminiCLI github repo with you.**

## How to Use

Once installed and reloaded, the skill will automatically trigger when you ask Gemini to "humanize" or "rewrite" text.

### Examples

- **Basic Humanization:**
  > "Please humanize this text: [Paste AI-generated text here]"

- **Voice Calibration:**
  > "Here is a sample of my writing style: [Paste your sample]
  > Now, humanize this text to match my voice: [Paste AI-generated text]"

- **Specific Pass:**
  > "Run a humanizer audit on this draft and fix any lingering AI tells."

## Key Features

- **29 Detection Patterns:** Targets specific vocabulary (e.g., "delve", "tapestry"), structural tropes (rule of three), and style artifacts (em dash overuse).
- **Multi-Pass Audit:** Performs calibration, rewriting, and a final "AI-goggles" pass to ensure quality.
- **Voice Matching:** Adapts rhythm, vocabulary, and punctuation to match a user-provided sample.
