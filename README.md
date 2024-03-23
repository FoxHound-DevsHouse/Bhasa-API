

## Supported Languages and ISO Codes

- **English (en)**
- **Hindi (hi)**
- **Urdu (ur)**
- **Bengali (bn)**
- **Marathi (mr)**
- **Gujarati (gu)**
- **Punjabi (pa)**
- **Tamil (ta)**
- **Telugu (te)**
- **Kannada (kn)**
- **Malayalam (ml)**

These ISO codes can be used to specify the source and target languages in the request bodies for ASR, NMT, and TTS endpoints.

## ASR (Automatic Speech Recognition)

**Endpoint:** `POST /asr`

**Body:**
```json
{
  "sourceLang": "hi",
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA"
}
```

## NMT (Neural Machine Translation)

**Endpoint:** `POST /nmt`

**Body:**
```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "text": "यह एक उदाहरण वाक्य है।"
}
```

## TTS (Text to Speech)

**Endpoint:** `POST /tts`

**Body:**
```json
{
  "sourceLang": "hi",
  "text": "यह एक उदाहरण वाक्य है।",
  "gender": "male"
}
```

## ASR + NMT (Speech to Text Translation)

**Endpoint:** `POST /asr_nmt`

**Body:**
```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA"
}
```

## NMT + TTS (Text Translation to Speech)

**Endpoint:** `POST /nmt_tts`

**Body:**
```json
{
  "sourceLang": "en",
  "targetLang": "hi",
  "text": "This is an example sentence.",
  "gender": "female"
}
```

## ASR + NMT + TTS (Speech to Speech Translation)

**Endpoint:** `POST /asr_nmt_tts`

**Body:**
```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA",
  "gender": "male"
}
```

This README outlines the different endpoints and corresponding request bodies for the specified functionalities along with the supported languages and their ISO codes. You can use this as a reference for integrating your application with the Fireworks AI API.
