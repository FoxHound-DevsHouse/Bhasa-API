# Bhasa-API
Powering Our Solution
```markdown
# API Endpoints

## 1. ASR (Automatic Speech Recognition)

### POST /asr

**Request Body:**

```json
{
  "sourceLang": "hi", // ISO 639-1 language code
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA" // Base64 encoded WAV audio file
}
```

## 2. NMT (Neural Machine Translation)

### POST /nmt

**Request Body:**

```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "text": "यह एक उदाहरण वाक्य है।"
}
```

## 3. TTS (Text to Speech)

### POST /tts

**Request Body:**

```json
{
  "sourceLang": "hi",
  "text": "यह एक उदाहरण वाक्य है।",
  "gender": "male" // or "female"
}
```

## 4. ASR + NMT (Speech to Text Translation)

### POST /asr_nmt

**Request Body:**

```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA"
}
```

## 5. NMT + TTS (Text Translation to Speech)

### POST /nmt_tts

**Request Body:**

```json
{
  "sourceLang": "en",
  "targetLang": "hi",
  "text": "This is an example sentence.",
  "gender": "female"
}
```

## 6. ASR + NMT + TTS (Speech to Speech Translation)

### POST /asr_nmt_tts

**Request Body:**

```json
{
  "sourceLang": "hi",
  "targetLang": "en",
  "base64Audio": "BASE64_ENCODED_AUDIO_DATA",
  "gender": "male"
}
```
```
