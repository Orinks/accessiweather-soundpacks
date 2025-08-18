# Contributing to AccessiWeather Community Sound Packs

Thanks for helping make AccessiWeather better! This guide explains how to create and submit a sound pack.

## Getting Started
- GitHub account and Git installed
- Audio editor (e.g., Audacity)
- Recommended format: WAV, 44.1kHz, 16‑bit; duration 1–3 seconds

## Sound Pack Requirements
- A pack.json at the root of your pack folder
- Audio files referenced by pack.json
- Clear, distinct, accessible sounds; normalized volume

### pack.json schema
Required:
- name (string)
- sounds (object mapping keys → filenames)

Optional:
- author (string)
- description (string)
- version (string)

Example:
```json
{
  "name": "Nature Sounds",
  "author": "Your Name",
  "description": "Peaceful nature sounds for notifications",
  "version": "1.0.0",
  "sounds": {
    "alert": "bird_chirp.wav",
    "notify": "water_drop.wav"
  }
}
```

Supported sound keys: alert, notify (some packs also include error, success). See AccessiWeather docs/SOUND_PACKS.md for full details.

## Submission Process
1. Fork Orinks/accessiweather-soundpacks
2. Create a branch (e.g., feature/my‑nature‑pack)
3. Add your pack under packs/<your_pack_id>/
4. Include license/attribution (e.g., LICENSE.txt in your pack folder)
5. Open a Pull Request and fill out the PR template

Commit style: single‑line summaries; concise and descriptive.

## Review Criteria
- Valid pack.json; referenced files exist
- Audio quality and accessibility
- Licensing/attribution provided

## Code of Conduct
Be respectful and constructive. Report issues via GitHub Issues.

