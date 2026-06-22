# SonarBun v1.0.0

First public binary release of SonarBun Live Translator for Windows 64-bit.

## Included

- Windows output/loopback and input/microphone capture
- Local faster-whisper transcription
- Online translation using a user-provided API key
- Optional NLLB offline translation model download
- CPU and optional NVIDIA CUDA processing
- Source and target language selection
- English and Japanese GUI languages
- Editable glossary profiles
- Local translation cache
- `live.txt` output and `history.txt` session history
- User guides in Italian, English, and Japanese

## Installation

No installer is required. Download `SonarBun-v1.0.0-win64.zip`, extract the complete archive, and run `SonarBunLiveTranslator.exe`.

Do not remove the `_internal` or `glossaries` folders.

## Notes

- Whisper and offline translation models are downloaded separately when requested.
- API keys are not included and must be supplied by the user.
- CUDA is optional; CPU mode works without NVIDIA software.
- The Windows executable is currently unsigned and may trigger a SmartScreen warning.

## Privacy and license

SonarBun contains no developer-operated telemetry or user account system. Read `PRIVACY.md`, `LICENSE.md`, and `THIRD_PARTY_NOTICES.md` before distribution.

## SHA-256

```text
57D0379B62CCD61F9CC9A3F4D4864D7AF6D26832B117CC2ABFBEF08C8C7D79E3
```
