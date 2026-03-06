# MUDTERM.IO

Browser-based MUD client.

## Features

- Multi-session — open multiple connections simultaneously, switch between them via tabs
- Cloud sync — connection configs and profiles sync across devices when logged in
- Auth — Google, GitHub, Discord login via OAuth
- Connection types — direct WebSocket or bridge/proxy (Telnet over WebSocket)
- Protocol support — auto-negotiate, GMCP, MCCP2, extended, telnet, terminal, JSON
- Per-connection profiles — separate auto-login and automation per character
- Automation — aliases, triggers, timers, scripts per profile
- Widget system (in progress)  — button grids, vital gauges, direction pad, multi-pane layouts, dockable zones
- Display settings — font family, size, line height, letter spacing, scrollback per connection
- Input settings — local echo, command history, command separator per connection
- MUD directory — browse and connect to MUDs via a relay server
- Session logging
- PWA — installable, service worker, works offline

## Known Issues

- MCCP2 compression not working
- Echo foreground and background color settings not implemented
