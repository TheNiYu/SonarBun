# 🎧 SonarBun - by TheNiYu

<div align="center">

**English** | [日本語](README_JA.md)

</div>

A real-time audio transcription and translation tool for Windows.

SonarBun can listen to desktop/output audio or an input device such as a microphone, transcribe speech locally with Whisper, and translate it through an online API service or a local offline model.

---

## ⚙️ What it does

- 🎧 Captures Windows output/loopback audio
- 🎙️ Captures microphones, audio interfaces, and virtual inputs
- 📝 Transcribes speech locally with faster-whisper
- 🌐 Supports online translation through user-provided API keys
- 📴 Supports local offline translation after the model is downloaded
- 🌍 Lets you select source and target languages
- 📚 Supports editable glossary profiles and translation caching
- 📄 Writes the latest translation to `live.txt`
- 🖥️ Includes English and Japanese interface languages
- ✅ No installer required: extract the archive and run the `.exe`

---

## 🚀 How to use

1. Download `SonarBun-v1.0.0-win64.zip` from the [Releases](../../releases) section
2. Extract the entire archive to a normal folder
3. Run `SonarBunLiveTranslator.exe`
4. Select:
   - Output/browser audio or Input/microphone
   - Audio device
   - Source language
   - Target language
5. Choose Online or Offline translation in **Settings**
6. Click **Start**

Do not run the executable directly from inside the ZIP archive. The `_internal` and `glossaries` folders must remain next to the executable.

Detailed guides are available in [Italiano](docs/Guida_Utente_SonarBun_IT.pdf), [English](docs/SonarBun_User_Guide_EN.pdf), and [日本語](docs/SonarBun_User_Guide_JA.pdf).

---

## 🌐 Online mode

Online mode uses a personal API key supplied by the user. API keys are not included with SonarBun.

The key is encrypted locally with Windows DPAPI. During online translation, the locally transcribed text is sent to the selected API provider. Raw audio is not sent by SonarBun to the translation provider.

Provider availability, pricing, quotas, and data handling are controlled by the respective third-party service.

---

## 📴 Offline mode

Offline mode does not require an API service. Internet access is needed only to download the selected translation model the first time.

The currently available offline model is approximately 630 MB and is intended for personal, non-commercial use under its own license. Offline translation can be less contextual than online translation.

---

## 💻 Requirements

- Windows 10 or Windows 11, 64-bit
- Working audio input/output device
- Internet connection for model downloads and Online mode
- NVIDIA CUDA-compatible GPU is optional

CPU mode works without NVIDIA software. CUDA requires compatible NVIDIA hardware, drivers, and the runtime components described in the user guide.

---

## 🔐 Privacy

SonarBun does not include analytics, telemetry, advertising, or user accounts.

It creates local configuration, history, cache, model, and output files. See [PRIVACY.md](PRIVACY.md) for details.

---

## 🔐 File integrity (SHA-256)

**`SonarBun-v1.0.0-win64.zip` SHA-256:**

```text
57D0379B62CCD61F9CC9A3F4D4864D7AF6D26832B117CC2ABFBEF08C8C7D79E3
```

To verify an archive on Windows, open Command Prompt in the download folder and run:

```text
CertUtil -hashfile SonarBun-v1.0.0-win64.zip SHA256
```

Compare the result with the checksum shown on the Release page.

---

## 📜 License

SonarBun is proprietary freeware distributed in binary form. The source code is not publicly available.

Personal, non-commercial use is permitted. See [LICENSE.md](LICENSE.md) for the complete terms. Third-party components and downloadable models remain subject to their respective licenses; see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

---

## ⚠️ Disclaimer

Automatic transcription and translation can be inaccurate. Do not rely on SonarBun for emergencies, medical decisions, legal matters, or other situations requiring certified interpretation.

---

> **Made by [TheNiYu](https://github.com/theniyu)**  
> Support and contact: [@1pixeldot](https://x.com/1pixeldot)
