# Design a Live Video Streaming platform e.g. YouTube Live, Twitch etc.


## RTMP : Real time messaging protocol
Real-Time Messaging Protocol (RTMP) is a communication protocol for streaming audio, video, and data over the Internet.

RTMP is a widely-used protocol for video streaming that YouTube Live has accepted since the service began.

## RTMPS :
RTMPS is a secure extension to RTMP. RTMPS is a regular RTMP (RealTime Messaging Protocol) video stream tunneled through an SSL connection. RTMPS benefits both content creators and viewers by preventing man-in-the-middle attacks on the ingestion side of livestreams. This ensures that all of a creator's live streaming data — including video, audio, and control signals — is securely transmitted to YouTube's servers, protecting it from tampering or interception in transit.

## HLS (HTTP Live Streaming) and DASH (Dynamic Adaptive Streaming over HTTP):
The HLS and DASH ingestion protocols are also encrypted, like RTMPS. They also support codecs that RTMP and RTMPS do not. Next-generation video codecs such as VP9 and HEVC can offer much better compression relative to H.264, allowing users to either stream with higher quality for a given bitrate or stream with the same quality while using a lower bitrate, which could decrease buffering. This makes HLS or DASH ingestion a good choice for premium content that requires higher quality and higher resolution, albeit at a relatively higher latency. Note that HLS and DASH ingestion typically incur greater latency than RTMP because HLS and DASH are segment-based.









# References :
1. ByteByteGo : https://www.youtube.com/watch?v=7AMRfNKwuYo

2. YouTube Live : https://developers.google.com/youtube/v3/live/guides/ingestion-protocol-comparison
