# Amplitude & Time
- In the real world, sound is produced by vibrations which cause waves to travel through the air.
- To represent this digitally, a microphone’s transducer converts these sound waves into a voltage which is sampled a certain number of times each second. This is the ‘amplitude’ of the audio and the number of times a value is taken is referred to as the ‘sample rate’ of an audio recording.
- The sample rate is measured in Hz. In the screenshot above, the sample rate of the audio file is 96,000Hz which means each second there are 96,000 samples.

# Bit-Depth
-  The amplitude values are quantised by an analogue-to-digital converter—this means to make them fit between two minimum/maximum values. 
- The granularity available here is the ‘bit depth’ of the audio recording. The higher the bit-depth, the more faithful to the real frequency the recording will be. A 16-bit recording would be able to store 1 of 65536 (216) values each sample.

# Storage
Audio filetypes and codecs dictate the amount and type of compression used. The most ubiquitous music file format—*mp3*—is a [[Lossy]] format, while _flac_ is a popular format that is [[Lossless]].