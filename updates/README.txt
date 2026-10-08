This directory is the public updater origin for the Nexus desktop app.

Publish here:

  latest.json   (UTF-8, no BOM)

Do not commit the Windows installer into this git tree. The .exe and .sig
live on a public GitHub Release of satvik-vinoth/Arqca. latest.json's
platforms.windows-x86_64.url must be that Release asset, for example:

  https://github.com/satvik-vinoth/Arqca/releases/download/v0.1.1/Nexus_0.1.1_x64-setup.exe

Rules:
- Never publish a fake .exe
- Never put the Tauri updater private key here
- Cache latest.json for minutes, not days
- Keep the Download button on the landing page pointing at the same URL
