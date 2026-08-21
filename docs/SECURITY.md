# Security

Security is a core consideration in Float AI because the application may process user-provided text, clipboard content, conversations, and AI requests.

## Secrets

Never commit secrets to the repository.

This includes:

- API keys
- Database credentials
- Authentication secrets
- Tokens
- Private keys

Secrets must be stored in environment variables or an appropriate secret-management system.

Use `.env.example` to document required variables without exposing their values.

## API Keys

AI provider API keys must not be exposed to the desktop client when they can be kept securely on the backend.

The preferred flow is:

```text
Desktop Client
      │
      │ Request
      ▼
   Backend
      │
      │ API Key
      ▼
  AI Provider