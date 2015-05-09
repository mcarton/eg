# ffmpeg

get information on an audio or video file

    ffmpeg -i file

extract 42 seconds of audio, starting from 13 minutes and 37 seconds

    ffmpeg -i input.mp4 -vn -acodec libvorbis -ss 00:13:37 -t 42 output.ogg


