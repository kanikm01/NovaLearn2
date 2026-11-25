# NovaLearn — Complete AI learning app

## Features
- Responsive dashboard with the NovaLearn learning sections
- Animated page transitions, custom vector artwork, hover states and mobile navigation
- Grade 6–9 topic lists, lessons, worked examples, tips, progress and rewards
- AI Tutor connected to the OpenAI Responses API through the Express backend
- Topic-specific AI quiz generation with five multiple-choice questions per set
- Recent question tracking in the browser to reduce repetition
- Clear backend/API connection status in the AI Tutor

## Run in GitHub Codespaces
1. Extract this ZIP into your Codespace project folder.
2. Open the terminal in the folder containing `server.js`.
3. Run `npm install`.
4. Create a file named `.env` in the same folder.
5. Add your API key to `.env`:
   ```
   OPENAI_API_KEY=your_real_api_key
   OPENAI_MODEL=gpt-5-mini
   PORT=3000
   ```
6. Run `npm start`.
7. Open the forwarded port 3000 in Codespaces.

## Test the backend
Open `/api/status` on the forwarded port. It should contain `server: "running"` and `aiConfigured: true`. Then test AI Tutor and Practice Quiz.

## Important
- Keep `.env` private. Never paste the key into `index.html` or commit it.
- A ChatGPT subscription is not the same as API usage access. The API key must be valid and the API account must have available usage/billing access.
- Profile, XP, progress, rewards and recent quiz history are stored in that browser's local storage; they are not synced across devices.
- This package does not claim to provide real email verification or password reset. Those require a configured authentication provider and email delivery service.
- The app runs without a key, but live AI chat and AI-generated quizzes require one.
