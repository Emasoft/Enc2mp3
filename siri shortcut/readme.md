# ENCODE TO MP3

*ENCODE TO MP3* is a shortcut to convert multiple audio files from any format into MP3 or M4A files with the LAME or AAC Encoder.  
  
  
How to use it
===========
 - Just select the audio files you want to convert to MP3 (or M4A) from the Files app (using multiple selection, mixing multiple formats is fine), and then use the share menu to send them to the shortcut.  
 - The shortcut will open the a-Shell mini app and will do the conversion using ffmpeg.  
 - You can convert to **MP3** using the **Lame MP3 encoder** at the best quality (320k constant bit rate) or at a quality optimized for file size (variable bit rate 190-250k).  
 - Or you can convert to **M4A** (the audio only version of MP4) using the **AAC MP4 encoder** at the best quality (270k constant bit rate) or at a quality optimized for file size (192k constant bit rate).  
 - You can choose to just **copy the audio streams** in the new container format, without re-encoding. This is called '**remuxing**'. But since not all codecs are supported by all formats, this conversion can fail. **WARNING**: Be sure to check if the source file audio codec is supported by the output container format before trying to remux.  
 - You will also be asked if you want to **normalize** the volume of the files.  
 - Wait the shortcut to end all the processing, without touching anything, and after a while you will be asked where to save the resulting MP3 / M4A audio files.  
 - To avoid confusion, a suffix '(was xxx)', where xxx is the previous file extension, will be added to the file names.  
 - If you select **video files** they will be converted **to audio only** MP3/M4A files.  
 
 
Calling it from other Shortcuts  
=========================
 - From version 1.0.2 you can use ENCODE TO MP3 as an helper function in your shortcuts.  
 - For the details and the parameters, just read the comment inside the shortcut source.  
  

Supported audio formats:
=====================
AAC, AC3, AIFF, ASF, AVI, CAF, DFF, DSF, DTS, F4V, FLAC, FLV, HEVC, M4A, M4B, M4R, MAUD, MKA, MKV, MOV, MP2, MP4, MPEG, MPG, OGA, OGG, OPUS, TS, TTA, VOB, VOC, W64, WAV, WEBM, WMA, WMV, 3GP.  
  
Some Background On Audio Quality
==============================
Bitrate is not the only thing to consider when it comes to codecs.  
  
Frequency response range is also very important.  
  
|**Codec**|**Format**|**Transparency**|**File Size** (at Transp.)|**Frequency Response** (at 192 kbit/s)|
|:-|:-|:-|:-|:-|
|MP3|.mp3|250 kbit/s|1.87 MB/minute|0-16 kHz|
|AAC|.mp4|220 kbit/s|1.65 MB/minute|0-18 kHz|
|Opus|.ogg, .webm|190 kbit/s|1.42 MB/minute|0-20 kHz|
|WAV|.wav|lossless|10.58 MB/minute|0-22 kHz|
  
 **Glossary**:  
  
  - ***Transparency*** : *"A transparency threshold is a given bitrate value at which audio transparency is reached. Transparency is the result of lossy data compression accurate enough that the compressed result is perceptually indistinguishable from the uncompressed input for the **average** listener."*  
  - ***Frequency Response*** : *"The analysis of the frequency spectrum of each song shows how well each code compression algorithm works in comparison to WAV and each other. Its shows when frequency cross-section of the codec leads to the loss of high-frequency part of the sound. Then codec with the biggest frequency range is the codec that provides the nearest reproduction value of the full frequency spectrum in comparison to non- compressed WAV with the range of approximately 22 kHz."*  
  
  
Source:  
  
 - Zhurakovskyi, Bohdan, Nataliia Tsopa, Yevhenii Batrak, Roman Odarchenko and Tetiana Smirnova. *“Comparative Analysis of Modern Formats of Lossy Audio Compression.”* CybHyg (2019).  
  
  

REQUIREMENTS
=============
 - You need the [**a-Shell Mini**](https://apps.apple.com/ao/app/a-shell-mini/id1543537943) app installed. The version must be **1.9.4 or greater**.  The 'Mini' version of a-Shell only sizes at 340Mb.  
  

ACKNOWLEDGEMENTS
===================
 - I wish to thank his excellency [**Nicolas Holzschuch**](https://github.com/holzschu) (*the genius developer of a-Shell*) for the port of the Lame mp3 encoder in a-Shell and the early access to the beta.  
  
INFO
====
 - First Release: 2022-07-13 	v1.0.0   
 - Latest: 2022-08-17 	v1.1.1  
 - Author: [u/fremenmuaddib](https://www.reddit.com/user/fremenmuaddib/)   
 - This shortcut is canonically available on RoutineHub at https://routinehub.co/shortcut/12550/  
  
   
