# Deadwire

Windows desktop manager for Project Zomboid clients and local servers, written in C#.

[Download the latest Windows x64 release](https://github.com/FatRambo/deadwire/releases/latest)

Extract the ZIP into a writable folder and run `Deadwire.exe`. The .NET runtime is bundled. First-run setup links your game, selects workspace storage and prepares SteamCMD when needed. Steam permissions and an installed WebView2 browser runtime are required for their respective features.

Deadwire manages separate instances, local Workshop mods, pinned revisions, dependencies, mod lists, settings, backups and rescue restores. Game/mod files, user data and development files are excluded from app release ZIPs. Full personal instance backups may contain private server data and mod files; keep them private unless you have permission to distribute their contents.

## App updates

Starting with v0.7.3, new workspaces use this signed update feed and a publisher key embedded in the app:

`https://github.com/FatRambo/deadwire/releases/latest/download/latest.json`

Existing custom or disabled sources stay unchanged. Choose **Settings → Use Deadwire GitHub updates** to switch an older workspace. Check for updates, download an offered version, stop instance games/servers and downloads, then restart to install. The previous app is retained for rollback. Update sources remain configurable.

Release assets contain the app ZIP, signed `latest.json` feed and `publisher-public.pem` public key. The private signing key is never uploaded. The executable is not Authenticode signed; feed signatures provide separate publisher verification.

Project Viewpoint integration and the final multiplayer modpack require in-game validation. There is no claim of universal automatic mod conversion. Source and development work are maintained separately from this download repository.
