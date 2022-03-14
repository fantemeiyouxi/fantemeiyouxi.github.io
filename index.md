---
layout: default
---
**Paper1**:This is the unofficial demo page for the paper [Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrogram Predictions](https://arxiv.org/abs/1712.05884)
## Abstract
This paper describes Tacotron 2, a neural network architecture for speech synthesis directly from text. The system is composed of a recurrent sequence-to-sequence feature prediction network that maps character embeddings to mel-scale spectrograms, followed by a modified WaveNet model acting as a vocoder to synthesize timedomain waveforms from those spectrograms. Our model achieves a mean opinion score (MOS) of 4.53 comparable to a MOS of 4.58 for professionally recorded speech. To validate our design choices, we present ablation studies of key components of our system and evaluate the impact of using mel spectrograms as the input to WaveNet instead of linguistic, duration, and F0 features. We further demonstrate that using a compact acoustic intermediate representation enables significant simplification of the WaveNet architecture.
- - -
### Ground truth  Tacotron2
- - -
#### *010001*
<audio src="010001.wav" controls preload></audio><audio src="010001.wav_synthesis.wav" controls preload></audio>
- - -
**Paper2**:This is the unofficial demo page for the paper [WaveGlow: A Flow-based Generative Network for Speech Synthesis](https://arxiv.org/abs/1811.00002)
## Abstract
In this paper we propose WaveGlow: a flow-based network capable of generating high quality speech from mel-spectrograms. WaveGlow combines insights from Glow and WaveNet in order to provide fast, efficient and high-quality audio synthesis, without the need for auto-regression. WaveGlow is implemented using only a single network, trained using only a single cost function: maximizing the likelihood of the training data, which makes the training procedure simple and stable. Our PyTorch implementation produces audio samples at a rate of more than 500 kHz on an NVIDIA V100 GPU. Mean Opinion Scores show that it delivers audio quality as good as the best publicly available WaveNet implementation. All code will be made publicly available online.
- - -
### Ground truth  WaveGlow
- - -
#### *010001*
<audio src="010001.wav" controls preload></audio><audio src="010001.wav_synthesis.wav" controls preload></audio>
#### *010002*
<audio src="010002.wav" controls preload></audio><audio src="010002.wav_synthesis.wav" controls preload></audio>
- - -
