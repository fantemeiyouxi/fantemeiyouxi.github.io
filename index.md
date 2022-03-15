---
layout: default
---
# Tibetan speech synthesis 藏语语音合成
## Tacotron2 基于端到端的语音合成系统
**Paper1**:This is the unofficial demo page for the paper [Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrogram Predictions](https://arxiv.org/abs/1712.05884)
## Abstract
This paper describes Tacotron 2, a neural network architecture for speech synthesis directly from text. The system is composed of a recurrent sequence-to-sequence feature prediction network that maps character embeddings to mel-scale spectrograms, followed by a modified WaveNet model acting as a vocoder to synthesize timedomain waveforms from those spectrograms. Our model achieves a mean opinion score (MOS) of 4.53 comparable to a MOS of 4.58 for professionally recorded speech. To validate our design choices, we present ablation studies of key components of our system and evaluate the impact of using mel spectrograms as the input to WaveNet instead of linguistic, duration, and F0 features. We further demonstrate that using a compact acoustic intermediate representation enables significant simplification of the WaveNet architecture.
- - -
### Tacotron2&Waveglow合成音频
- - -
#### 010021	ཁོ་རའི་གང་ཟེར།ཀྲུ་མ་ཀྲུ་འདི།
<audio src="010021_synthesis.wav" controls preload></audio>
#### 010041	འན་ད་ཁོ་ཚོས་ནུའུ་ཟེ།
<audio src="010041_synthesis.wav" controls preload></audio>
#### 010061	ཁོ་ཚོས་ཁོ་ཚོར་སྤྲས་ཡག་གི་གླུ།
<audio src="010061_synthesis.wav" controls preload></audio>
#### 010282	གང་ལྟར་དེ་འདྲས་བྱེད་དུས་ཙམ་པ་མ་གཞི་དེ་ད་མ་ཞི་པ་ནང་བཞིན་ཞེད་སྣང་ཞེད་སྣང་སེ་ཡོ་མ་རེད་དེ།
<audio src="010282_synthesis.wav" controls preload></audio>
#### 010422	དེ་ཚོ་བཙལ་ནི་ད་སོ་སོ་དི་འདྲ་ད་འཚར་ལོངས་བཟོ་ར་ཡོང་གི་སྤྱི་ཚོགས་ཐོག་ལ་ད་ང་ཚོ་ད།
<audio src="010422_synthesis.wav" controls preload></audio>
#### 010662	ལ་རྦེད་ལ་རྦེད།དེ་ནས་ཁྱེད་གཉིས་སློབ་གྲྭ་གཅིག་རུ་རེད་ཀྱང་སློབ་གྲྭ་གཞན་དག་རེད།སློབ་གྲྭ་ཐད་ཐད་རེད།
<audio src="010662_synthesis.wav" controls preload></audio>
#### 030777	དེའི་རྗེས་ནས་ཡར་ནང་ལ་ཕར་ལོག་ངས་ཕ་མར་ཡར་འོ་ཕ་འདྲས་སེ་བྱས་བཤད་པ་ཡིན་པར།ཨ་ནི་ཕ་མས་འགྲོ་མི་དགོས་ཟེར།
<audio src="030777_synthesis.wav" controls preload></audio>
#### 210540	སྟོད་དབུས་གཙང་ཆོས་སྒེར་སོན་པོའི་མན་ཆད་ནས་སྨད་རྒྱ་ཡུལ་ཁྲིམས་སྒོ་དམར་བོའི་ཡན་ཆད་འདིར་ཀླུ་བདུད་བཙན་གསུམ་གྱི་ཁ་གནོན་དུ་མངགས་ཏེ།
<audio src="210540_synthesis.wav" controls preload></audio>
- - -
## Waveglow 基于glow的声码器
**Paper2**:This is the unofficial demo page for the paper [WaveGlow: A Flow-based Generative Network for Speech Synthesis](https://arxiv.org/abs/1811.00002)
## Abstract
In this paper we propose WaveGlow: a flow-based network capable of generating high quality speech from mel-spectrograms. WaveGlow combines insights from Glow and WaveNet in order to provide fast, efficient and high-quality audio synthesis, without the need for auto-regression. WaveGlow is implemented using only a single network, trained using only a single cost function: maximizing the likelihood of the training data, which makes the training procedure simple and stable. Our PyTorch implementation produces audio samples at a rate of more than 500 kHz on an NVIDIA V100 GPU. Mean Opinion Scores show that it delivers audio quality as good as the best publicly available WaveNet implementation. All code will be made publicly available online.
- - -
### 原始音频	                                              WaveGlow合成音频（原始音频→梅尔谱图→音频）
- - -
#### 010001	ཡང་ལུས་སྦྱོང་གཞན་དག་དེ་འདྲ་རྩེད་ཡག་ཡིན་ནའི་རེད།འདིའི་ནང་།འདིར་ཕྱིན་བྱས།ཡང་ཐང་བདེ་ཞིག་ཡོད་འབའ།སློབ་གྲྭའི་འདི།
<audio src="010001.wav" controls preload></audio><audio src="010001.wav_synthesis.wav" controls preload></audio>
#### 010002	རྦད་དེ་ཁོ་ར་ཨ་མའི་འགྲམ་ཤོར་འགྲོ་གི་རེད།
<audio src="010002.wav" controls preload></audio><audio src="010002.wav_synthesis.wav" controls preload></audio>
#### 010003	ཁོང་ཚོ་དོ་དགོངས་ནས་ནང་ལ་སླེབས།
<audio src="010003.wav" controls preload></audio><audio src="010003.wav_synthesis.wav" controls preload></audio>
#### 010004	མངར་མོ་ཞེད་པོ་གཏོང་ཉིན་དྲོ་གི་མིན་འདུག་ལ་ཁོ་མངར་མོ་གཅིག
<audio src="010004.wav" controls preload></audio><audio src="010004.wav_synthesis.wav" controls preload></audio>
#### 010005	ད་འདི་ཚོ་ལ་ཡའ་ཁ་ཤས་འདི་ཚོ་ལ་ཡའ་འདི་བྱེད་དགོས་རེད་དའ།
<audio src="010005.wav" controls preload></audio><audio src="010005.wav_synthesis.wav" controls preload></audio>
- - -
