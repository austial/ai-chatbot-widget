# Austial Chatbot Widget

A lightweight, customizable React chatbot component that seamlessly integrates with the [Austial platform](https://www.austial.com) for AI-powered customer conversations.

[![npm version](https://img.shields.io/npm/v/@austial/chatbot-widget.svg)](https://www.npmjs.com/package/@austial/chatbot-widget)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Chatbot Preview

<p align="center">
  <img src="https://www.austial.com/static/chatbot/chatbot-preview.png" alt="Chatbot Preview 1" width="500" />
</p>

## Dashboard Preview

<p align="center">
  <img src="https://www.austial.com/static/chatbot/chatbot-panel-preview.png" alt="Chatbot Panel Preview" width="500" />
</p>

## Features

- **Easy Integration** - Use as npm package or script tag
- **Cloud-Configured** - All settings managed via Austial dashboard
- **Responsive Design** - Works seamlessly on all devices
- **Secure** - API key authentication with configurable security settings

## Prerequisites

Before using this widget, you need to:

1. **Sign up at [Austial](https://www.austial.com)**
2. **Create a chatbot** in your Austial dashboard
3. **Get your credentials**:
   - Business ID
   - API Key

All chatbot configurations (appearance, behavior, knowledge base, AI instructions, etc.) are managed through the Austial dashboard.

## Installation

### NPM (React Applications)

```bash
npm install @austial/chatbot-widget
```

### Script Tag (Any Website)

```html
<script src="https://unpkg.com/@austial/chatbot-widget@latest/dist/austial-chatbot.iife.js"></script>
```

## Quick Start

### React Usage

```tsx
import { Chatbot } from '@austial/chatbot-widget'
import '@austial/chatbot-widget/dist/style.css'

function App() {
  return (
    <Chatbot
      config={{
        businessId: 'your-business-id',
        apiKey: 'your-api-key',
      }}
    />
  )
}
```

### HTML/JavaScript Usage

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>My Website</h1>

    <script src="https://unpkg.com/@austial/chatbot-widget@latest/dist/austial-chatbot.iife.js"></script>
    <script>
      window.AustialChatbot.init({
        businessId: 'your-business-id',
        apiKey: 'your-api-key',
      })
    </script>
  </body>
</html>
```

## Configuration

**The widget only requires two parameters:**

```typescript
{
  businessId: string // Your unique business identifier from Austial
  apiKey: string // Your API key from Austial dashboard
}
```

All other configurations are managed through your **[Austial Dashboard](https://www.austial.com)**:

### Dashboard Configuration Options

- **Business Information** - Name, description, branding
- **Chatbot Settings** - Bot name, avatar, welcome message, placeholder text
- **UI Interface** - Colors, position, themes, styling
- **Knowledge Base** - Upload files and documents for AI training
- **AI Instructions** - Custom prompts and behavior rules
- **Security** - Access control, rate limiting, domain restrictions
- **Analytics** - Conversation insights and performance metrics

## Austial Platform

The widget connects to the Austial platform to:

- Fetch your chatbot configuration automatically
- Process user messages with AI
- Store conversation history
- Apply your custom knowledge base
- Enforce security settings

**Visit [www.austial.com](https://www.austial.com) to:**

- Create and manage chatbots
- Configure appearance and behavior
- Upload knowledge base files
- Customize AI instructions
- View analytics and conversations
- Manage API keys and security

## Methods

### Initialize

```javascript
window.AustialChatbot.init({
  businessId: 'your-business-id',
  apiKey: 'your-api-key',
})
```

### Destroy

```javascript
window.AustialChatbot.destroy()
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## TypeScript

Full TypeScript definitions are included:

```typescript
import type { ChatbotConfig, Message } from '@austial/chatbot-widget'
```

## Support

- **Website:** [www.austial.com](https://www.austial.com)
- **Dashboard:** [www.austial.com/dashboard](https://www.austial.com/dashboard)
- **Documentation:** [GitHub Repository](https://www.austial.com/ai-chatbot)
- **Issues:** [GitHub Issues](https://www.austial.com)
- **Email:** info@austial.com

## License

MIT © [Austial](https://github.com/aayushsolanki40/chat.austial.com)
