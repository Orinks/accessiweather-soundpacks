# AccessiWeather Community Sound Packs

This folder seeds the new public repository Orinks/accessiweather-soundpacks, which will host community‑contributed sound packs for AccessiWeather.

- Main app: https://github.com/Orinks/AccessiWeather
- Purpose: Share, review, and distribute high‑quality, accessible notification sounds

## Sound Pack Structure

Each pack is a directory containing a pack.json file and the referenced audio files (WAV recommended).

Example directory:

```
my_pack/
├─ pack.json
├─ alert.wav
└─ notify.wav
```

Example pack.json (aligned with docs/SOUND_PACKS.md):

```json
{
  "name": "Display Name",
  "author": "Author Name",
  "description": "Description of the sound pack",
  "version": "1.0.0",
  "sounds": {
    "alert": "alert.wav",
    "notify": "notify.wav"
  }
}
```

Required fields:
- name: Human‑readable display name
- sounds: Map of sound keys to filenames

Optional fields:
- author, description, version

Supported sound keys today:
- alert, notify
- Some built‑in packs also include: error, success

## Contributing

See CONTRIBUTING.md for detailed guidelines. In summary:
1. Fork the repository
2. Create your pack under packs/<your_pack_id>/ with pack.json and audio files
3. Include license and attribution for all sounds
4. Open a Pull Request using the template

## Installation

AccessiWeather can install community packs from this repository. Until broadly available, you can copy a pack folder into your local sound packs directory as documented in AccessiWeather.

## License

Contributors must include licensing details for included audio. By submitting, you confirm you have the right to share these sounds under the specified license.

