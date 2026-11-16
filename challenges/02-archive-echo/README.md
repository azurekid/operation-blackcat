# Operation Archive Echo

**Difficulty:** Medium  
**Format:** Closed-world OSINT / digital forensics  
**Flag format:** `BC{public_landmark}`

## Briefing

A volunteer team preparing a fictional Seattle-area history walk has misplaced a **replica exhibit card**. Your team has preserved image metadata, staged public-record excerpts, and synthetic device logs showing activity around familiar public places in Seattle and Redmond.

The setting uses real, publicly accessible landmarks to make the route recognizable. The event, people, accounts, item, and movement records are fictional; no real person or organization is implicated, and no item is actually hidden. Work only with the evidence in [`evidence/`](evidence/). Do not identify real people, search for live profiles, contact anyone, or visit a location.

## Team task

1. Extract the photographer fragment, timestamp, and location from [`evidence/photo_metadata.txt`](evidence/photo_metadata.txt).
2. Correlate the fragment with the staged records in [`evidence/public_records.md`](evidence/public_records.md). Identify the fictional account and the replica item.
3. Use [`evidence/district_guide.csv`](evidence/district_guide.csv), [`evidence/device_events.csv`](evidence/device_events.csv), [`evidence/gps_tracks.csv`](evidence/gps_tracks.csv), and the detailed [`case_a.gpx`](evidence/case_a.gpx) and [`case_b.gpx`](evidence/case_b.gpx) tracks to reconstruct the public-landmark visits and scheduled return.
4. Submit the flag and a short evidence-based timeline. Cite filenames and timestamps; distinguish direct evidence from inference.

## Evidence notes

- Timestamps in evidence files are UTC; Seattle local time for these October dates is PDT (UTC−7). Narrative comments include local times where useful.
- Coordinates are WGS84 latitude/longitude for public landmarks. Use the included guide; external searches are unnecessary.
- GPX tracks contain dense simulated fixes during five public-venue windows. Each file has separate venue segments, so no road route is implied. The tracks describe no real attendee.
- Device IDs are case labels, not phone numbers, IMEIs, or other real identifiers.
- The staged records are the complete source set. No external social-media searches, account access, or contact with real people or organizations is in scope.

## Submission

Use [`submission-template.md`](submission-template.md). Facilitators may award partial credit for a correctly supported timeline even if the final location is wrong.

## Suggested timing

For a group of 20, work in four teams of five. Allow 55 minutes for investigation, 15 minutes for team submissions, and 20 minutes for a debrief.
