# Exporting Minecraft Worlds — Bedrock Edition

## Method 1: In-Game Export (Recommended)

1. Open **Minecraft Bedrock Edition**
2. Go to **Settings → Storage**
3. Click on **Worlds** (shows total size and item count)
4. Select the world you want to export
5. Tap the **pencil/edit icon** on the world
6. Scroll down and click **Export World**
7. Choose a save location — exports as a `.mcworld` file

Alternatively, from the **Play** screen:
1. Click the **pencil icon** next to the world name
2. Scroll to the bottom of world settings
3. Click **Export World**

## Method 2: Manual File Access

Bedrock Edition worlds are stored locally at:

```
%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\minecraftWorlds
```

Each subfolder represents a world. To export manually:

1. Navigate to the path above in File Explorer
2. Copy the desired world folder
3. Compress it into a `.zip` file
4. Rename the `.zip` extension to `.mcworld`

> **Note:** If the `minecraftWorlds` folder is empty or missing, your worlds may be cloud-synced. Use the in-game export method instead.

## Importing a `.mcworld` File

- **Windows:** Double-click the `.mcworld` file — Minecraft will open and import it automatically
- **Mobile:** Open the file with Minecraft

## Converting Between Editions

Bedrock and Java Edition use different world formats. To convert:

- Use [Chunker](https://chunker.app/) — a free online world converter
- Upload your `.mcworld` file and export in Java format (or vice versa)

## Storage Info (This Device)

- **Total Worlds:** 27
- **Total Size:** 71.5 MB

## Pushing to GitHub

```bash
# Initialize git inside the project folder
cd minecraft_world
git init

# Stage and commit
git add .
git commit -m "Initial commit: Minecraft Bedrock world export guide"

# Rename branch to main
git branch -M main

# Add remote and push
git remote add origin https://github.com/YOUR_USERNAME/minecraft_world.git
git push -u origin main
```

> Replace `YOUR_USERNAME` with your GitHub username. Create the repo on [github.com/new](https://github.com/new) first — keep it empty (no README/`.gitignore`).

## Creating the GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `minecraft_world`
3. Leave it **empty** (no README, no `.gitignore`)
4. Click **Create repository**

Then add the remote and push:

```bash
git remote add origin https://github.com/debeerswang/minecraft_world.git
git push -u origin main
```