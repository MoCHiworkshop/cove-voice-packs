# MoCHi offline English voice packs

Optional model data for the native MoCHi Android app: Cove, Maple, Juniper and Ellen.
Each voice has FP32, INT8 and INT4 semantic-model options; waveform models stay FP32.
English only. Requires a 64-bit ARM phone. No account or API key is required for download or inference.

Assets named by SHA-256 are shared verified model objects, not executable plugins.
MoCHi pins their size and SHA-256 in the APK. Downloading additional voices reuses existing shared files.
Do not extract these objects into a random voice pack or substitute another voice's conditioning.
The accompanying catalog records immutable sources, exact model object pins and authenticated archive digests.
Each voice's notices.txt (stored as its catalog SHA asset) contains upstream notices/licenses.

Model source: https://huggingface.co/MoYoYoTech/tone-models/tree/198ceeac1c4d5b75072b6995af2e185e4559ec1d
Reference configuration: https://huggingface.co/MoYoYoTech/VoiceDialogue/blob/9dca1cb160672a194e5538670fbf2b60a048a916/src/voice_dialogue/tts/configs/moyoyo.py
Converted to ONNX with GPT-SoVITS V2; frontend uses the pinned g2p_en model and pronunciation dictionary.
Upstream tone-models repository metadata declares MIT; original license/notice terms are retained.

Native Android import and playback passed for all nine additional voice/precision combinations. See VERIFICATION.json. Download files are supplied through the releases listed in this repository.
