# WestHill RolePlay

Modern, community-driven FiveM server website for Los Santos roleplay.

## Features

✅ **Admin Dashboard** (Password: `westhill2026`)
- News management (add, edit, delete)
- Admin team management with avatars
- Faction management
- Server rules management
- Social media links
- Server configuration (IP, CFX code, slots)
- Gallery management (GitHub image support)

✅ **Real-time Sync with Firebase**
- Live database updates
- No page refresh needed

✅ **GitHub Integration**
- Images stored in `/img/` folder
- Automatic GitHub raw URL generation
- Easy image management

✅ **Multi-language Support**
- Hungarian (HU)
- English (EN)

## Structure

```
westhillroleplay/
├── index.html          (Main website)
├── README.md           (This file)
└── img/
    ├── gallery/        (Gallery images)
    ├── admins/         (Admin avatars)
    └── factions/       (Faction images)
```

## Firebase Setup

The website uses Firebase Realtime Database. Create this structure:

```json
{
  "westhillrp": {
    "config": {
      "cfxJoinCode": "6my47k8",
      "serverIP": "connect.westhillrp.hu:30120",
      "maxSlots": 128,
      "heroText": "Los Santosban, uram.",
      "gallery": ["1.jpg", "2.jpg", "3.jpg"]
    },
    "news": [],
    "admins": [],
    "factions": [],
    "rules": [],
    "social": {
      "discord": "https://discord.gg/...",
      "tiktok": "https://tiktok.com/...",
      "youtube": "",
      "instagram": ""
    }
  }
}
```

## Adding Images

1. **Create directories** in GitHub:
   - `img/gallery/` - Gallery images
   - `img/admins/` - Admin avatars
   - `img/factions/` - Faction images

2. **Upload images** to the appropriate folder

3. **In Admin Panel**, enter the filename (e.g., `1.jpg`)

4. **Images are automatically loaded** from:
   ```
   https://raw.githubusercontent.com/lakatosdavid060-cpu/westhillroleplay/main/img/gallery/1.jpg
   ```

## Usage

1. Click the **⚙️** button (bottom-left)
2. Enter password: `westhill2026`
3. Manage all website content in real-time

## Technologies

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Database**: Firebase Realtime Database
- **Storage**: GitHub
- **Hosting**: Any static hosting (GitHub Pages, Vercel, etc.)

## License

MIT License - Feel free to modify and use for your project.
