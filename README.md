# Prabhat Samgiita Content

This repository contains the songs and background images used by the
[ps.clerk.am](https://ps.clerk.am) web application.

## Layout

```
.
├── songs/      # MDX song files (XXXX.mdx)
└── images/     # Background JPEGs (ps-XXXX.jpg)
```

## Notes on Content

- **Lyrics, music, and translations** are by Shrii Prabhat Ranjan Sarkar and protected by the original copyright. They are reproduced here for educational and devotional purposes only.
- **Background images in `images/`** are AI-generated illustrations (created with ChatGPT) inspired by each song. They are not original artworks.

## Quick Start

### Adding a new song

Create a new file `songs/XXXX.mdx` (e.g., `songs/0693.mdx`):

```mdx
---
title: Song title (first line in original language)
number: 693
date: '1982-10-16'
language: bengali
theme: Theme or category
music_style: Musical style information
place: Composition location
source_url: https://sarkarverse.org/wiki/Song_title
audio_recordings:
- url: https://app.psbot.eu/play_audio/693/
  source: https://www.youtube.com/@Gunavati
  singer: Gunavati
ai:
  mood: devotional
  intensity: 8
  emotions:
  - yearning
  - devotion
  spiritual_themes:
  - divine-guidance
  - surrender
  keywords:
  - light
  - darkness
---

## Roman Script

Original text in Roman transliteration
Line 1
Line 2

Empty lines between stanzas are preserved

## Bengali

Bengali script version (if applicable)

## English Translation

English translation here

## Russian Translation

Russian translation here
```

## Structure Details

### Frontmatter Fields

**Required:**
- `title` - Song title (usually first line)
- `number` - Song number (1-5018)
- `date` - Composition date in 'YYYY-MM-DD' format (quoted string)
- `language` - Original language (bengali, english, sanskrit, hindi, urdu, etc.)

**Optional:**
- `theme` - Thematic category
- `music_style` - Musical style information
- `place` - Where it was composed
- `source_url` - Link to Sarkarverse or other source
- `audio_recordings` - Array of audio recordings with url, source, and singer
- `ai` - AI-generated metadata. Common subfields: `mood`, `intensity`, `emotions`, `spiritual_themes`, `keywords`, `ai_tags`, `key_symbols`, `image_prompt`, `primary_colors`, `visual_mood`, `time_of_day`, `setting`

### Content Sections

**Section names:**
- `## Roman Script` - Original text in Roman transliteration (always present)
- `## Bengali` - Original in Bengali script (if applicable)
- `## English Translation` - English translation (if original is not in English)
- `## Russian Translation` - Russian translation (optional)

**Notes:**
- If the original song is in English, the "English Translation" section should be omitted
- Section order matters for proper display
- All text content preserves line breaks and formatting

## Example: Complete Song Entry

```mdx
---
title: Bandhu he niye calo
number: 1
date: '1982-09-14'
language: bengali
theme: (Shiva) Enlightenment
music_style: Ajay valley+ Italy,Kaharva
place: Madhumanika, Deoghar
source_url: https://sarkarverse.org/wiki/Bandhu_he_niye_calo
audio_recordings:
- url: https://app.psbot.eu/play_audio/1/
  source: https://www.youtube.com/@Gunavati
  singer: Gunavati
ai:
  mood: devotional
  intensity: 8
  emotions:
  - yearning
  - devotion
---

## Roman Script

BANDHU HE NIYE CALO
ÁLOR OI JHARŃÁDHÁRÁR PÁNE
BANDHU HE NIYE CALO

## Bengali

বন্ধু হে নিয়ে চলো
আলোর ওই ঝর্ণাধারার পানে
বন্ধু হে নিয়ে চলো

## English Translation

Oh Abiding Friend, take me with.
Toward yon streaming fountain of effulgence,
Oh Abiding Friend, take me with.

## Russian Translation

О верный Друг, веди меня.
Веди к источнику
ослепительного сияния.
О верный Друг, веди меня.
```

## Resources

- [Sarkarverse Song List](https://sarkarverse.org/wiki/List_of_songs_of_Prabhat_Samgiita)