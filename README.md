# Fireworks AI API Endpoints and Request Bodies

This document outlines the various endpoints and request body structures for interacting with the Fireworks AI API for different tasks including Automatic Speech Recognition (ASR), Neural Machine Translation (NMT), and Text to Speech (TTS) functionalities.

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

Feel free to adjust and expand this README file according to your specific project requirements and documentation standards.

--- 

This README outlines the different endpoints and corresponding request bodies for the specified functionalities. You can use this as a reference for integrating your application with the Fireworks AI API.
