CALLING PARAMETERS FOR 'ENCODE TO MP3'   
====================================
 - You can use this shortcut as an helper function from your shortcuts.  
  
INPUT:  
=====
 - You must pass a Dictionary (or a file .json) as the shortcut parameter.  
 - The Dictionary entries should be the following ones:  
 -  
 - KEY = 'input_folder'  
 - Type = Text
 - VALUE = path to the folder containing the audio files to convert.  
           Must be a folder under the 'Shortcuts' folder (on iCloud Drive).
		   You must omit the Shortcuts part (i.e. 'iCloud Drive/Shortcuts/your_sc_folder/input/' must be written: '/your_sc_folder/input/').
-  
- KEY = 'output_folder'
- Type = Text
- VALUE = path to the folder where the converted audio files will be saved.  
           Must be a folder under the 'Shortcuts' folder (on iCloud Drive).  
		   You must omit the Shortcuts part (i.e. 'iCloud Drive/Shortcuts/your_sc_folder/output/' must be written: '/your_sc_folder/output/').  
 -   
 - KEY = 'arguments'  
 - Type = Dictionary  
 - VALUE = A Dictionary  
 -  
 - Content of the 'arguments' sub Dictionary:  
 - KEY = 'output_format' ('arguments.output_format' in dot notation)  
 - Type = Text
 - VALUE = (one of the following:)  
 -         'CBR320' : Convert to 320k constant bit rate  
 -         'CBR320_NORM' : Convert to 320k constant bit rate and Normalize   
 -         'CBR270' : Convert to 270k constant bit rate   
 -         'CBR270_NORM' : Convert to 270k constant bit rate and Normalize   
 -         'CBR192' : Convert to 270k constant bit rate  
 -         'CBR192_NORM' : Convert to 192k constant bit rate and Normalize  
 -         'VBR190' : Convert to 190-250 variable bit rate  
 -         'VBR190_NORM' : Convert to 190-250 variable bit rate and Normalize
 -         'TRY_REMUX' : Try stream copy to remux audio (no re-encoding)
 -         'TRY_REMUX_NORM' : Try to remux audio (no re-encoding) and Normalize
 -         'LOSSLESS' : Convert to lossless format (i.e. FLAC)  
 -         'LOSSLESS_NORM' : Convert to lossless format (i.e. FLAC) and Normalize  
 -
 -  
 -  
 - KEY = 'container' ('arguments.container' in dot notation)  
 - Type = Text  
 - VALUE = (one of the following:)   
 -         'mp3' : Convert to mp3 (LAME mp3 codec)   
 -         'm4a' : Convert to m4a (AAC mp4 codec)  
 -         'flac'  :  Convert to FLAC (lossless compression)  
 -  
 -  
 - KEY = 'skip_mp3' ('arguments.skip_mp3' in dot notation)  
 - Type = Boolean  
 - VALUE = (one of the following:)  
 -         true : the mp3 files will not be reencoded.  
 -         false : the mp3 file will be reencoded.  
 -  
 - KEY = 'skip_mp4' ('arguments.skip_mp4' in dot notation)  
 - Type = Boolean  
 - VALUE = (one of the following:)  
 -         true : the mp4 files (.mp4,.m4a,.m4b,.m4r) will not be converted.  
 -         false : the mp4 files (.mp4,.m4a,.m4b,.m4r) will be converted to mp3.  
 -  
 -  NOTE: The last 2 keys ('skip_mp3', 'skip_mp4') are not implemented yet. Do not use them.
 - 
 -  
 OUTPUT:  
 ======
 - The shortcut returns the same 'output_folder' path as passed by the calling shortcut.  
 - But when it returns, the 'output_folder' shall contain only the newly encoded MP3 files.  
   



  
 