# ChordConnect
An onset-detection dataset based on [osu!]

There is great potential for using the choreograpy of osu! beatmaps to extract the underlying musicality of signals. Each playable osu! beatmap contains several semantically-rich pieces of data associated with a musical track (generally distributed at 16KHz). This can include metadata such as time signatures, tempo and timing changes, and onsets, all in millisecond-precision (as intended to be played by end-users).

This repository will host code to assemble a dataset using a beatmap mirror ([BeatConnect]), which will enable deep learning to be used to revolutionize this application in the same way it did in 2012, when AlexNet burst onto the scene and elevated image recognition accuracy from 40% to 90% on ImageNet-1k. 

The parallels are numerous: Natural photographs found in the wild are rife with noise, and the sheer volume of data associated with each sample can muddy the features intended to be extracted by classical algorithms. Thus it was inconceivable that a human could hand-design a signal processing algorithm for image detection which did not suffer from significant inaccuracies, and indeed, despite several domain-specific adaptations made specifically to attain higher performance on academic benchmarks (leaving aside the challenges of more representative real-world data), for many years, AI practitioners developed painstakingly hand-tailored feature extractors which could operate in the lab to emulate human judgments. 

Deep learning should instead be applied to design parametrized algorithms which perform the task of mapping noisy signals to semantically-rich, linearly-separable output, for all variety of potential applications! Amid promising new deep learning publications aimed directly at the [processing of raw audio waveforms][sashimi], This project hopes to enable modern sequence-transduction approaches to perform musical transcription, onset detection, and perhaps even automated choreography. 

[osu!]: https://github.com/ppy/osu
[beatconnect]: https://beatconnect.io/
[sashimi]: https://arxiv.org/abs/2202.09729
