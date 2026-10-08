This directory is the public updater origin for the Nexus desktop app.

When a signed installer exists, publish these three files here:

  latest.json
  Nexus_<version>_x64-setup.exe
  Nexus_<version>_x64-setup.exe.sig

Rules:
- latest.json must be UTF-8 without BOM
- platforms.windows-x86_64.url must be
  https://arqca.me/updates/Nexus_<version>_x64-setup.exe
- Cache latest.json for minutes, not days
- Never publish a fake .exe
- Never put the Tauri updater private key here
