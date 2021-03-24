# OBS-Studio_for_ATEM_Streaming_Bridge

# change flv-mux.c to connect to ATEM Streaming Bridge
obs-studio/plugins/obs-outputs/flv-mux.c

# Reason
There are some differences between OBS-Studio and ATEM Streaming Bridge at RTMP protocol @setDataFrame().

## OBS-Studio
verbose] RTMP_ClientPacket, received: notify 387 bytes
[verbose] (object begin)
[verbose] Property: <Name:           no-name., STRING:    onMetaData>
[verbose] Property: <Name:           no-name., ECMA_ARRAY>
[verbose] (object begin)
[verbose] Property: <Name:           duration, NUMBER:    0.00>
[verbose] Property: <Name:           fileSize, NUMBER:    0.00>
[verbose] Property: <Name:              width, NUMBER:    1920.00>
[verbose] Property: <Name:             height, NUMBER:    1080.00>
[verbose] Property: <Name:       videocodecid, NUMBER:    7.00>
[verbose] Property: <Name:      videodatarate, NUMBER:    2500.00>
[verbose] Property: <Name:          framerate, NUMBER:    25.00>
[verbose] Property: <Name:       audiocodecid, NUMBER:    10.00>
[verbose] Property: <Name:      audiodatarate, NUMBER:    160.00>
[verbose] Property: <Name:    audiosamplerate, NUMBER:    48000.00>
[verbose] Property: <Name:    audiosamplesize, NUMBER:    16.00>
[verbose] Property: <Name:      audiochannels, NUMBER:    2.00>
[verbose] Property: <Name:             stereo, BOOLEAN:    TRUE>
[verbose] Property: <Name:                2.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                3.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                4.0, BOOLEAN:    FALSE>
[verbose] Property: <Name:                4.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                5.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                7.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:            encoder, STRING:    obs-output module (libobs version 26.1.0)>
[verbose] (object end)
[verbose] (object end)

## ATEM Streaming Bridge
[verbose] RTMP_ClientPacket, received: notify 371 bytes
[verbose] (object begin)
[verbose] Property: <Name:           no-name., STRING:    onMetaData>
[verbose] Property: <Name:           no-name., ECMA_ARRAY>
[verbose] (object begin)
[verbose] Property: <Name:                2.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                3.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                4.0, BOOLEAN:    FALSE>
[verbose] Property: <Name:                4.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                5.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:                7.1, BOOLEAN:    FALSE>
[verbose] Property: <Name:      audiochannels, NUMBER:    2.00>
[verbose] Property: <Name:       audiocodecid, STRING:    mp4a>
[verbose] Property: <Name:      audiodatarate, NUMBER:    64.00>
[verbose] Property: <Name:    audiosamplerate, NUMBER:    48000.00>
[verbose] Property: <Name:    audiosamplesize, NUMBER:    16.00>
[verbose] Property: <Name:           duration, NUMBER:    0.00>
[verbose] Property: <Name:            encoder, STRING:    Blackmagic Design AVC Encoder>
[verbose] Property: <Name:           fileSize, NUMBER:    0.00>
[verbose] Property: <Name:          framerate, NUMBER:    60.00>
[verbose] Property: <Name:             height, NUMBER:    1080.00>
[verbose] Property: <Name:             stereo, BOOLEAN:    TRUE>
[verbose] Property: <Name:       videocodecid, STRING:    avc1>
[verbose] Property: <Name:      videodatarate, NUMBER:    9000.00>
[verbose] Property: <Name:              width, NUMBER:    1920.00>
[verbose] (object end)
[verbose] (object end)


# OBS-Studio setting
Screenshot_1.png
Screenshot_2.png
Screenshot_3.png
