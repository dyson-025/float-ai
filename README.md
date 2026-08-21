# Float AI

A lightweight floating AI assistant for desktop that provides quick AI-powered help without requiring users to switch applications.

## Overview

Float AI lives as a small floating bubble on the desktop. Users can open it using the bubble or a keyboard shortcut and perform AI-powered actions on text or through normal chat.

The goal is to make AI accessible wherever the user is working.

## Planned Features

- AI chat
- Improve English and grammar
- Translate text
- Summarize content
- Explain text
- Generate better/professional responses
- Clipboard-based text actions
- Global keyboard shortcut
- Floating desktop interface

## Tech Stack

### Desktop
- Tauri
- React
- TypeScript

### Backend
- FastAPI
- Python

### Data
- PostgreSQL

### AI
- LLM API

## Project Structure

```text
apps/
├── desktop/    # Tauri + React desktop application
└── backend/    # FastAPI backend

docs/            # Project documentation
tests/           # Tests