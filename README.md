## Dev locally

```
npm i
env-cmd npx functions-framework --target=openai-4
```

## Deploy

```
gcloud functions deploy openai-4 \
--allow-unauthenticated \
--runtime=nodejs18 \
--update-env-vars OPENAI_API_KEY=PASTE_KEY_HERE \
--trigger-http
```
