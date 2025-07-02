# Canopy UI Helm Chart

A Helm chart for deploying the Canopy UI frontend application.

## Description

This chart deploys a web-based frontend interface for Canopy, an AI-powered text summarization application. The UI runs on port 8501 and can be configured to connect to various language model endpoints.

## Installation

```bash
helm install canopy-ui ./chart
```

## Configuration

The following table lists the configurable parameters and their default values:

| Parameter | Description | Default |
|-----------|-------------|---------|
| `LLM_ENDPOINT` | Language model endpoint URL | `""` |
| `SYSTEM_PROMPT` | Default system prompt for the model | `"Summarize this text."` |
| `MODEL_NAME` | Name of the model to use | `"tinyllama"` |

## Components

- **Deployment**: Runs the Canopy UI container
- **Service**: Exposes the application on port 8501
- **Route**: Provides external access to the application

## Chart Information

- **Version**: 0.0.5
- **App Version**: 0.2
- **Image**: `quay.io/rlundber/canopy-ui:0.2`