

# This file describe how to split videos with FFMPEG 

	---------Definition---------
FFmpeg is an open source video and audio converter that works at high speed.
You can use it to accomplish many tasks of decoding, encoding, transcoding, 
multiplexing, streaming, among others. Nevertheless, it is command-based, 
so you need to set the command line arguments correctly.


	---------Video-splitiing---------
For splitting video ou need to specify the path for the input video after the "-i" argument and then specify  the start second and the duration,
at the end mention the output file name. 

	#If the video is in its raw format, you need to specify:
1- The pixel-format
2- The video size
3- The framerate
of the input and output video.

	---------Exemple-command---------
	
		$ sudo apt install ffmpeg
		$ ffmpeg -i input/video/path/name -ss 00:14 -t 00:10 output/video/path/name

The "-ss" argument is for the split option, the "00:14" is the start second, the "-t" option is for 
the duration and its argument is "00:10", so the splitted video will last 10 seconds.
	
	
	
