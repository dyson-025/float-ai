# Architecture

## Overview

Float AI is a desktop AI assistant built around a lightweight floating interface.

The application consists of a desktop client, backend services, and an AI provider.

```text
┌──────────────────────────────┐
│        Desktop Client        │
│                              │
│   Tauri + React + TypeScript │
│                              │
│  • Floating Bubble           │
│  • Assistant UI              │
│  • Keyboard Shortcuts        │
│  • Clipboard Integration     │
└──────────────┬───────────────┘
               │
               │ HTTPS
               ▼
┌──────────────────────────────┐
│           Backend            │
│            FastAPI           │
│                              │
│  • API                       │
│  • Authentication            │
│  • AI Service                │
│  • Application Logic         │
└──────────────┬───────────────┘
               │
        ┌──────┴───────┐
        ▼              ▼
┌──────────────┐ ┌──────────────┐
│   Database   │ │  AI Provider │
│ PostgreSQL   │ │    LLM API   │
└──────────────┘ └──────────────┘