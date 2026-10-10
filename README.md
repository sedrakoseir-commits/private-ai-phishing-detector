# private-ai-phishing-detector
AI-powered phishing email detector built with Flowise and Ollama to analyze email content using a locally running language model.
[README.md](https://github.com/user-attachments/files/33288952/README.md)
# Private AI Phishing Detector

An educational cybersecurity project that uses Flowise and Ollama to analyze email content for potential phishing indicators with a locally running language model.

## Overview

Phishing emails can use misleading language, suspicious requests, and other signals to trick recipients. This project explores how a local AI workflow can help review email content and produce a structured assessment.

The project was built with Flowise to connect the workflow components and Ollama to run the language model locally, without relying on an external AI API for model inference.

## Tools and Technologies

- **Flowise** — visual builder for the AI workflow
- **Ollama** — runs the language model locally
- **Prompt engineering** — guides the model toward consistent, structured analysis

## How It Works

1. Provide the email content to the workflow.
2. The language model reviews the content for possible phishing indicators.
3. The workflow returns an assessment based on the instructions and model output.
4. Review the assessment as an aid to decision-making, not as a definitive verdict.

## Testing

The workflow was tested with two example emails:
- An email identified as spam.
- An email believed to be legitimate.

These examples were used to observe how the model responded to different email content. They are initial tests, not a comprehensive accuracy evaluation.

## Privacy Considerations

The model runs locally through Ollama, so model inference does not need to be sent to an external AI API. Privacy also depends on how the surrounding workflow is configured and whether inputs or outputs are logged, stored, or shared. Avoid testing with sensitive personal or confidential email content.

## Limitations

- AI output can be incorrect or inconsistent.
- An email marked as suspicious is not necessarily malicious, and a reassuring result does not prove an email is safe.
- This prototype does not replace email security products, header analysis, URL reputation checks, or human review.

## Possible Future Improvements

- Test with a larger, labeled collection of phishing and legitimate emails.
- Add email-header and URL analysis.
- Compare model outputs and measure false positives and false negatives.
- Improve the output format and add clearer explanations for each indicator.

## Disclaimer

This project is for educational and defensive cybersecurity purposes. Do not use it as the sole basis for deciding whether an email is safe.

## Author

Created as a cybersecurity learning project exploring local AI and phishing analysis.
