# For demonstration regarding Vegas self renderer/ffmpeg/Voukoder

Original file: https://test-videos.co.uk/bigbuckbunny/mp4-h264 (1080p, 30MB)

**Exported to: 360p/bitrate 0.768k**

- Vegas settings: Ref=2, AVC, CBR
- ffmpeg settings: ```-c:v libx264 -x264-params "nal-hrd=cbr" -b:v 768k -minrate 768k -maxrate 768k``` (Also see https://trac.ffmpeg.org/wiki/Encode/H.264)
- Voukoder settings: ```b=768000 opencl=1 preset=medium rc=abr x264-params=ref=2``` (Is utmost simulation ATM, unable to customize setting)
 
Did not use any hardware acceleration (CUDA, NVENC, etc...) in the process

