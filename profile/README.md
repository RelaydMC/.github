<p align="center">
  <img src="https://raw.githubusercontent.com/RelaydMC/.github/main/assets/relayd.png" width="96" border-radius="14px" alt="Relayd" />
</p>

<h1 align="center">Relayd</h1>

<p align="center">
  Secure. Monitor. Relay.
</p>

<p align="center">
  A lightweight, self-hosted Minecraft server manager built for admins who want control without handing everything to a third-party panel.
</p>

---

## What is Relayd?

Relayd is a modern Minecraft server admin panel focused on simple, secure remote management.

It is built around a small local agent that runs beside your Minecraft server and exposes only carefully scoped actions, like starting, stopping, restarting, viewing logs, creating backups, and sending approved Minecraft commands.

No arbitrary shell.
No remote root terminal.
No unnecessary cloud dependency.

Just the tools you actually need.

---

## Why Relayd?

Most server panels are either too heavy, too hosting-provider-focused, or too broad.

Relayd starts smaller:

- Mobile-first server management
- Local-first by default
- Secure command allowlisting
- Live logs
- Simple backups
- Modded-server friendly workflows
- Designed for single-server and small-community admins first

---

## Project goals

Relayd is being built with a few core principles:

### Local-first

Your server data stays on your server.

The first versions of Relayd are designed to work without a hosted cloud backend.

### Secure by design

Relayd is not a web terminal.

The agent exposes a small set of safe actions instead of arbitrary system access.

### Minecraft-focused

Relayd is not trying to be a generic game hosting platform on day one.

The goal is to make Minecraft server management feel clean, safe, and easy.

---

## Roadmap

### v0.1

- Server status
- Start server
- Stop server
- Restart server

### v0.2

- Live logs

### v0.3

- Send allowed Minecraft commands

### v0.4

- Backups

### v0.5

- Mod uploads

### v0.6

- Users
- Audit log

---

## Architecture

```txt
Mobile app / Web app
        ↓
Relayd API / Agent
        ↓
systemd + tmux
        ↓
Minecraft server
