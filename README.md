#  Saki Client

**A custom Minecraft: Java Edition launcher — built on Fabric.**

Sign in with your own Microsoft account, pick your version, manage mods, and launch
Minecraft with a clean, modern interface.

</div>

---

## What is Saki Client?

Saki Client is a lightweight, custom launcher for **Minecraft: Java Edition**. It builds on
**Fabric Loader**, so all your favourite Fabric mods (Sodium, Lithium, Iris, …) work out of
the box, while adding a modern launcher experience on top.

It is a personal, community-driven project — not an official Mojang or Microsoft product.

## Features

- **Official Microsoft sign-in** — log in with your own Microsoft account via Microsoft's
  standard OAuth 2.0 flow. Play in online mode with your own valid license.
-  **Fabric mod support** — install and manage mods (Modrinth integration); external Fabric
  mods are first-class and load normally.
-  **Multiple Minecraft versions** — pick and switch between supported versions, each in its
  own isolated instance.
-  **Server browser & quick connect** — save servers, ping them, and jump straight in.
-  **Cosmetics & skins** — capes, custom cosmetics, and a live 3D skin preview.
-  **Built-in logs & instance monitor** — see what's happening while the game runs.

## How sign-in works

Saki uses the **standard Microsoft OAuth 2.0 authorization-code flow** (public client,
`consumers` tenant, `XboxLive.signin` scope) with a `localhost` loopback redirect. Each user
signs in locally with **their own** Microsoft account; tokens are stored securely in the
operating system's credential store and never shared or collected centrally.

## Tech stack

| Part      | Stack                                   |
|-----------|-----------------------------------------|
| Launcher  | Tauri 2 · Rust (backend) · React + TypeScript (UI) |
| Game mod  | Java 21 · Fabric · Gradle · Loom · Yarn |

## Status

Actively developed. Targeting **Minecraft 1.21.x** with Yarn mappings.

## Disclaimer

Saki Client is an unofficial, fan-made launcher. **Minecraft** is a trademark of **Mojang
Studios / Microsoft**. This project is not affiliated with, endorsed by, or associated with
Mojang or Microsoft. You must own a valid copy of Minecraft: Java Edition to play.
