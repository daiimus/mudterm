# MUDTERM.IO

Universal MUD client. PWA. Runs in any browser. Installable to home screen.

## mudstandards.org WebSocket Compliance

- gmcp.mudstandards.org (TEXT = ANSI, BINARY = GMCP)
- terminal.mudstandards.org (TEXT = ANSI only)
- telnet.mudstandards.org (BINARY = full telnet stream)
- extended.mudstandards.org (TEXT = ANSI, BINARY = telnet subneg)
- json.mudstandards.org (TEXT = ANSI, BINARY = JSON envelope)

## Telnet Options

- ECHO (1) -- password masking
- SGA (3) -- suppress go ahead
- TTYPE (24) -- MTTS chain: MUDTERM, XTERM-256COLOR, MTTS 137
- EOR (25) -- end of record prompt markers
- NAWS (31) -- window size with auto-resize
- MSDP (69) -- key-value game data with nested tables and arrays
- MSSP (70) -- server status metadata
- GMCP (201) -- JSON game data via subnegotiation
- IAC escaping in all subnegotiation (send and receive)
- Negotiation loop prevention via local/remote state tracking

## GMCP Packages

- Core.Hello, Core.Supports.Set
- Char, Char.Vitals, Char.Status, Char.Items
- Room, Room.Info
- Comm, Comm.Channel

## Features

- xterm.js terminal
- Connection manager with saved connections
- Direct WebSocket and Bridge (telnet proxy) connection types
- Auto-negotiate or manual subprotocol selection
- Profile system with auto-login sequences
- Aliases (regex to command substitution)
- Triggers (regex to action on incoming text)
- Timers (interval-based commands)
- Lua scripting (Fengari in-browser VM)
- Draggable widgets (gauges, direction pad, buttons, map, room info)
- Command history
- Local echo toggle
- Session logging with export
- localStorage persistence
