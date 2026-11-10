# remote-pc releases

Release binaries of **remote-pc**, a low-latency remote desktop for Linux.

- **rpc-host**: the host. It streams a private virtual desktop (headless
  sway with XFCE) that follows the viewer's size and scale, or a desktop
  already running on the machine (X11, or a wlroots compositor such as
  sway). It encodes on the GPU (VA-API, H.264 or H.265) and serves native
  clients over UDP and browsers over WebSocket.
- **rpc-client**: the native Linux viewer.

The browser viewer is Perch's Remote Desktop extension, which downloads
`rpc-host` from this repository's releases.

Each release lists its files with their SHA-256 sums. The source code is
kept in a private repository.
