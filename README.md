# J.A.R.V.I.S. v4.0 — Smart Automation Edition

## What's new
- Refined holographic mobile dashboard and animated assistant face
- AI chat through a private server endpoint (API key stays on the server)
- Browser voice input and text-to-speech where supported
- Tasks, notes, and harmless saved preferences
- Date/time reminders (alerts only while the page remains open)
- One-tap Study, Break, Organize, and Daily Check-in routines
- Focus timer, calculator, quick actions, and live system overview

## Run on a computer
Requires Node.js 18 or newer.

1. Extract this ZIP.
2. Open a terminal in the extracted `JARVIS_v4` folder.
3. Run `npm install`.
4. Copy `.env.example` to `.env`.
5. Add your API key and a model name available to your API project in `.env`.
6. Run `npm start`.
7. Open `http://localhost:3000`.

Example `.env`:
```
OPENAI_API_KEY=your_private_key_here
OPENAI_MODEL=your_available_model_name
PORT=3000
```

Do not put the API key in `public/index.html`, GitHub, screenshots, or messages. Ask a parent or guardian before enabling paid API usage. Model names and API availability depend on your API account.

## Android
For use on your phone, the server must run on a computer or hosted service that your phone can reach. Open the server's HTTPS address on Android. Opening `public/index.html` directly as a local file will not connect to `/api/chat`. Browser microphone recognition usually requires HTTPS and microphone permission.

## Important limits
- Reminders alert only while the webpage is open and active; they are not Android background notifications.
- A webpage cannot control Android settings or silently perform device actions.
- Tasks, notes, reminders, preferences and recent chat are stored in this browser's local storage.
- When AI is enabled, chat content is sent to your server and configured AI provider.
- Do not save passwords, contact details, payment information, or sensitive personal information.
