Echoes of Sikkim - Prototype

1) Backend
cd backend
cp .env.example .env
edit .env with MONGODB_URI and GOOGLE_MAPS_API_KEY
npm install
npm run seed
npm run dev

2) Frontend
Open http://localhost:4000/
Language select -> main UI

3) Add assets
Place panorama JPGs in frontend/assets/panoramas/
Place images in frontend/assets/
Place audio in frontend/assets/audio/

4) Keys
Set GOOGLE_MAPS_API_KEY for Maps/Places/Directions
Set RAZORPAY_KEY_ID and RAZORPAY_KEY_SECRET to enable payments
Set OPENAI_API_KEY to enable AI responses

Notes
Service worker caches assets on first fetch. Use Download Tour to explicitly cache large panorama/audio files.
Routes are crowd-saved in the backend. When a user downloads a route online it is saved centrally for others.
