# CHRONICLES Version 4.2 — arrival video and marketplace ambience

## Upload this update

Unzip CHRONICLES_v4_2_Arrival_and_Ambience.zip. In the existing GitHub repository, select Add file → Upload files. Upload all SIX extracted files at the repository root, then Commit changes:

- index.html
- app.js
- styles.css
- marketplace-arrival.mp4
- marketplace-ambience.mp3
- AUDIO_CREDITS.md

The existing history.js and four background JPEGs remain required. This is an update for Version 4/4.1, not a standalone package. Wait for GitHub Pages to publish, then refresh with Command+Shift+R.

## Behavior

Begin investigation starts the short marketplace arrival once when entering at the marketplace. Learners can opt out of sound before beginning, pause/play the clip, skip it, replay it from the marketplace, and toggle ambience on/off. The clip ends on the still marketplace with working hotspots. People who request reduced motion in their device/browser skip automatic video playback and can explicitly choose Replay arrival.

Ambience continues quietly during marketplace exploration, pauses while any dialog is open, resumes on closing it, and stops in other locations or when the page is hidden. No audio plays before the learner begins. Saved case progress is preserved. Returning learners whose saved location is elsewhere resume that location without an arrival clip.

The video is muted by the page and its original music/audio stream has also been removed from the file. The separate MP3 supplies the optional ambience. It is intentionally quiet. If audio playback is blocked, the sound control allows another user-initiated attempt. If video playback fails, the learner can continue with the still scene; an initial load timeout provides a fallback.

## Media provenance

Video: supplied by Kelli Youngblood, generated in Mage from the CHRONICLES marketplace artwork. Source upload: 79a4d34b8d80cb55bf281af91ddd2d00.mp4. Derivative preserves the video stream and removes its complete original audio stream. Duration approximately three seconds; 854 × 478 at 30 fps. No visual enhancement or invented extra frames were added.

Ambience: “Busy Market Crowd Murmur Walla 75” from SFXMint.
Source: https://sfxmint.com/sounds/crowd-murmur-75
Downloaded MP3: https://sfxmint.com/dl/crowd-murmur-75.mp3
License stated by the publisher: CC0 1.0 Universal, permitting modification and redistribution, including commercial use.
License: https://creativecommons.org/publicdomain/zero/1.0/
Source/licensing checked November 13, 2026.

The publisher identifies this effect as synthetic/AI-generated crowd murmur. It is atmosphere, not a field recording or a reconstruction of ancient Egyptian language. Adaptation: high-pass at 160 Hz, low-pass at 3600 Hz, quiet loudness normalization around −30 LUFS, short edge fades, MP3 encoding at 128 kbps. The page applies an additional playback volume setting of 0.7. No music was added.

## Validation

JavaScript syntax check passed. FFprobe confirmed that marketplace-arrival.mp4 contains a video stream only. Browser tests verified user-started playback, pause/play, automatic completion into the still scene, replay, skip, mute, ambience pause when a conversation opens, resumption after closing it, silence in the workshop, and restart back to the opening. Reduced-motion and media-failure fallbacks are implemented but were not browser-emulated in this walkthrough. Physical-device audio balance and mobile playback still need review on the user's device.
