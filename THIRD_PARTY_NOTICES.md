# Third-Party Notices

SonarBun is proprietary software, but it uses third-party libraries and downloadable models that remain subject to their own licenses.

This notice identifies the principal components used by the current Windows build. Copyright notices and license terms belonging to those projects remain in force.

## Principal bundled components

| Component | Purpose | License | Project |
|---|---|---|---|
| PySide6 / Qt for Python | Graphical interface | LGPL-3.0-only OR GPL alternatives | https://www.qt.io/qt-for-python |
| Shiboken6 | PySide6 bindings support | LGPL-3.0-only OR GPL alternatives | https://www.qt.io/qt-for-python |
| faster-whisper | Local speech transcription | MIT | https://github.com/SYSTRAN/faster-whisper |
| CTranslate2 | Transformer inference | MIT | https://github.com/OpenNMT/CTranslate2 |
| SentencePiece | Tokenization | Apache-2.0 | https://github.com/google/sentencepiece |
| NumPy | Numerical processing | BSD-3-Clause | https://numpy.org |
| python-sounddevice / PortAudio | Audio input | MIT / PortAudio license | https://python-sounddevice.readthedocs.io |
| PyAudioWPatch / PortAudio | WASAPI loopback capture | Apache-2.0 / PortAudio license | https://github.com/s0d3s/PyAudioWPatch |
| WebRTC VAD | Voice activity detection | BSD-style / MIT wrapper | https://github.com/daanzu/py-webrtcvad-wheels |
| OpenAI Python library | Online API client | Apache-2.0 | https://github.com/openai/openai-python |
| Hugging Face Hub | Model downloads | Apache-2.0 | https://github.com/huggingface/huggingface_hub |
| ONNX Runtime | Runtime dependency | MIT | https://github.com/microsoft/onnxruntime |
| PyAV / FFmpeg libraries | Media processing dependency | BSD-3-Clause / applicable FFmpeg component licenses | https://github.com/PyAV-Org/PyAV |

The packaged application may include additional transitive dependencies. Their respective copyright notices and licenses continue to apply.

## Downloadable models

### NLLB-200 distilled 600M CT2 INT8

- Original model: Meta AI NLLB-200 distilled 600M
- CTranslate2 INT8 conversion: `osa911/nllb-200-distilled-600M-ct2-int8`
- License declared by the model package: CC BY-NC 4.0
- Intended for personal, non-commercial use
- https://huggingface.co/osa911/nllb-200-distilled-600M-ct2-int8

The model is not bundled in the standard SonarBun archive. It is downloaded only when requested by the user.

### Whisper models

Transcription models are downloaded on demand through faster-whisper/Hugging Face. Each model remains governed by the license and terms published by its model provider.

## Qt/LGPL note

The Windows distribution uses dynamically loaded Qt/PySide6 libraries. Users may replace compatible library files as permitted by the applicable LGPL terms. SonarBun does not claim ownership of Qt, PySide6, or Shiboken6.

## No endorsement

Third-party project names are used only to identify technical dependencies. Their inclusion does not imply endorsement of SonarBun by the respective authors or organizations.
