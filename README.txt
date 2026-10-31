VANCE AI STARTER — HTML/CSS/JavaScript + Vercel serverless API

FILES
- index.html: website interface
- api/chat.js: AI chat endpoint using Runware textInference
- api/image.js: image generation endpoint using Runware imageInference

IMPORTANT
1. Keep your Runware API key private. Never paste it into index.html or commit it to GitHub.
2. This starter requires a text model AIR ID from Runware for chat. Add it in Vercel as RUNWARE_TEXT_MODEL.
3. Optional: set RUNWARE_IMAGE_MODEL to a supported image model AIR ID. If omitted, the starter uses runware:400@1; change it if that model is not available to your account.
4. Set these under Vercel > Project > Settings > Environment Variables:
   RUNWARE_API_KEY = your secret Runware API key
   RUNWARE_TEXT_MODEL = AIR ID of a text/LLM model in Runware
   RUNWARE_IMAGE_MODEL = AIR ID of an image model (optional)
5. After changing environment variables, redeploy the project.
6. API usage may cost credits/money depending on your Runware account and model. Check pricing/credits before testing.

DEPLOYMENT
Import this project into a GitHub repository, then in Vercel choose Add New > Project and import that repository. The root directory should be the folder containing index.html and the api folder. No build command is needed for this plain HTML + Vercel Functions project.

Official docs:
Runware API authentication: https://runware.ai/docs/models-api/authentication
Runware API overview: https://runware.ai/docs/models-api/introduction
Runware compatible APIs: https://runware.ai/docs/tools/compatible-apis
