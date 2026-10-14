# Fix subtitles that start late or slowly drift out of sync

A caption file can be perfectly readable and still feel wrong. The useful first question is whether the timing error stays the same throughout the clip or grows as playback continues.

This guide uses [Cueforge](https://cueforge-subtitles.foggyibis16.chatgpt.site/), First Fold's free SRT and WebVTT workbench. It edits existing captions; it does not transcribe speech, translate text, or burn captions into a video.

## 1. Keep the original and identify two moments

Save your original subtitle file unchanged. Open a working copy in Cueforge. If your browser supports the video's codec, use **Open local video** to compare captions with playback.

Choose an unmistakable moment near the start and another near the end. A clearly spoken phrase is better than a vague pause. Write down both the caption timestamp and the moment that phrase actually belongs in the video.

Here are two fictional cases:

| Case | First caption / correct moment | Later caption / correct moment | Likely approach |
| --- | --- | --- | --- |
| Constant delay | 00:00:12.000 / 00:00:10.000 | 00:01:02.000 / 00:01:00.000 | Shift all cues by −2 seconds |
| Growing delay | 00:00:10.000 / 00:00:10.000 | 00:01:10.000 / 00:01:07.000 | Two-point drift correction |

In the first case, both captions are two seconds late. In the second, the beginning is aligned but a later caption is three seconds late. A single offset cannot align both moments.

## 2. Apply a constant offset when the error is stable

In **Timing**, enter the shift in seconds:

- Positive values move captions later.
- Negative values move captions earlier.

For the constant-delay example, enter **−2**, then choose **Preview offset**. Read the preview before applying it.

An earlier shift can move the first cue below zero. The option to move negative-start cues to zero keeps their duration, but it can change their relationship to neighboring cues. Review those early captions individually instead of assuming the fix is harmless.

Check at least the beginning, middle and end after applying the change. If the beginning now looks good but the end does not, revisit your diagnosis.

## 3. Use two well-separated anchors for gradual drift

Under **Two-point drift correction**, enter the two subtitle moments and their correct video moments. Both pairs must increase.

For the growing-delay example:

- Subtitle A: **00:00:10.000** → video A: **00:00:10.000**
- Subtitle B: **00:01:10.000** → video B: **00:01:07.000**

The elapsed interval shrinks from 60 seconds to 57 seconds. A subtitle moment halfway between the anchors, at 40 seconds, maps to 38.5 seconds. This is an arithmetic illustration, not a promise that all spoken words between those points line up.

Preview the correction. Cueforge applies a linear timing change to starts and ends. It can help with steady drift, but an edit that inserted or removed a scene creates a discontinuity. Correct those sections manually rather than forcing the entire file through one stretch.

## 4. Review readability separately

Timing alignment and reading comfort are different checks. Open **Quality** and inspect fast text, short durations and overlaps.

The thresholds are editable heuristics. Two speakers may intentionally overlap. Automatically trimming every overlap can make a caption too short; equal-start overlaps need manual attention. Rewrapping can also alter inline markup, so inspect the proposed batch changes.

Preview the repaired file with the actual video. Literal tags or positioning instructions may look different in the destination player because the workbench does not render advanced subtitle styling.

## 5. Export the format your player expects

Export SRT or VTT and keep a JSON backup if you want to return to the project. SRT cannot carry WebVTT metadata and cue settings. If those matter, retain VTT and inspect the result in the intended player.

Before replacing a published caption track:

- Check the first and last spoken lines
- Check the two anchors and at least one moment between them
- Review any cue moved to zero
- Check intentional overlapping speakers
- Confirm the exported format and language track

Cueforge accepts UTF-8 SRT/VTT up to 2 MiB and 5,000 cues. Browser video-codec support varies. Keep your original file and your exported result; an in-memory session is not a backup.

---

Published by First Fold, the maker of Cueforge. Features are free; support is optional. [Explore all 30 tools](https://first-fold-launch.foggyibis16.chatgpt.site/crypto-toolkit). Product instructions checked against the available workbench implementation on October 14, 2026.
