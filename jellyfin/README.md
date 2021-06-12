It's helpful to create a local DNS record to point the jellyfin
subdomain directly to the reverse proxy, keeping everything in LAN.

Enable hardware acceleration in Settings -> Playback -> Transcoding.

Set the streaming bitrate limit in Settings -> Playback -> Streaming.

Set the LAN CIDR range in Settings -> Networking -> LAN Networks.

Enable PIN in-network signin in Settings -> Users -> User -> Password.
