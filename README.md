# 🌎 PLUTO TV PLAYLISTS

![Auto Update](https://img.shields.io/badge/Token-Auto%20Updated-brightgreen)

---

# Pluto TV Playlists

This repository provides an automatically updated Pluto TV M3U playlist with EPG.  
**Important:** Each user must use their own unique `client_id` (UUID) to avoid stream conflicts on Pluto TV servers.

---

## Step 1: Fork This Repository

1. Click the **Fork** button on the top right of this repo.  
2. You now have your own copy of the repo in your GitHub account.

---

## Step 2: Generate Your Client ID (UUID)

You need a unique client ID for Pluto TV:

- Go to [https://www.uuidgenerator.net/](https://www.uuidgenerator.net/) and generate a new UUID.  
- Example: `9a1cce51-2d2f-4b6c-9f8e-1e2d0a3b4c5d`
- Copy the UUID.

---

## Step 3: Edit `config.json`

Open the `config.json` file in your fork and replace the default client_id with your UUID:

```json
{
  "client_id": "YOUR_UNIQUE_UUID_HERE"
}
```

### Step 4: Run GitHub Actions

After editing `config.json`:

1. Go to the **Actions** tab in your fork.
2. Select **All workflows** the click **Auto Pluto Update**.
3. Click **Run workflow**.
4. Wait for the workflow to finish. The playlist will now be updated with your unique client ID.

---

### **⚡ Automatic Token Update**

This repository uses GitHub Actions to automatically refresh the Pluto TV session token and regenerate the M3U playlist.

No manual intervention required.

---

## 📺 EPG Links
```text
https://raw.githubusercontent.com/matthuisman/i.mjh.nz/refs/heads/master/PlutoTV/all.xml
```

## Credits

This project is based on pluto_tv_scraper by 4v3ngR.

Original project:  
https://github.com/4v3ngR/pluto_tv_scraper

Some modifications and customization were made for this repository.

EPG data provided by [Matt Huisman](https://github.com/matthuisman)  
Source: https://github.com/matthuisman/i.mjh.nz
