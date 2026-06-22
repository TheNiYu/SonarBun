# Privacy Notice

Last updated: 22 June 2026

SonarBun is a local Windows desktop application. It does not include analytics, advertising, telemetry, user accounts, or a developer-operated cloud service.

## Audio and transcription

Audio selected by the user is processed locally by faster-whisper to produce a text transcript. SonarBun does not intentionally upload raw captured audio to an online translation provider.

## Online translation

When Online mode is enabled, the transcript and relevant translation instructions, including applicable glossary entries, are sent to the API provider selected by the user. The provider processes that data under its own terms and privacy policy.

The user is responsible for choosing a provider and for ensuring that the transmitted content is appropriate for that service.

## Offline translation

After the required models have been downloaded, Offline mode performs transcription and translation locally. Normal offline translation does not send transcripts to an external translation API.

## API keys

API keys are supplied by the user and encrypted locally using Windows Data Protection API (DPAPI). They are not stored in `sonarbun_config.json` and are not transmitted to the SonarBun developer.

## Local files

Depending on configuration and use, SonarBun may create:

- `sonarbun_config.json`: non-secret application settings
- `live.txt`: latest translated text
- `history.txt`: local transcript and translation history
- `translation_cache.json`: cached translations
- `models/`: downloaded transcription and translation models
- `%LOCALAPPDATA%/SonarBunLiveTranslator/*.dpapi`: encrypted API credentials

Users may delete these files when SonarBun is not running. Deleting configuration, cache, credentials, or models may require the related settings or downloads to be recreated.

## Contact

Questions can be sent to [@1pixeldot](https://x.com/1pixeldot).
