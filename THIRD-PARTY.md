# Third-party components — 0.4.0

- Tesseract4Android 4.9.0 and Tesseract 5.5.1: Apache-2.0. Leptonica 1.85.0: BSD-2-Clause. libpng 1.6.48: libpng license. libjpeg 9f: IJG license. Full notices bundled in app/src/main/assets/licenses.
- Russian/English OCR models: tesseract-ocr/tessdata_fast, Apache-2.0.
- sherpa-onnx v1.13.8: Apache-2.0, https://github.com/k2-fsa/sherpa-onnx/tree/v1.13.8 . Android library includes ONNX Runtime (MIT) and Kotlin standard library (Apache-2.0); license texts bundled.
- Russian speech model: sherpa-onnx-small-zipformer-ru-2024-09-18, derived from alphacep/vosk-model-small-ru, Apache-2.0. Model card: https://huggingface.co/alphacep/vosk-model-small-ru . Distribution: https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-small-zipformer-ru-2024-09-18.tar.bz2 . Included files: encoder.int8.onnx, decoder.onnx, joiner.int8.onnx, tokens.txt. Used with modified beam search, four active paths, CPU, entirely offline. Apache-2.0 text in licenses/SherpaOnnx.txt applies also to model.
- Illustrations generated with OpenAI ImageGen for this project.

Vosk Android/JNA and the older Kaldi small-ru-0.22 model from versions 0.3.x are no longer application dependencies. Their historical license texts remain in assets for reference.

Synthetic Russian WAV files in androidTest/assets are locally generated test fixtures and are not shipped in the application APK. All inference models are bundled; the application does not download models or transmit recognition data.