# OPERATION BLACKCAT — CASE FILE
## "OPERATION ESPRIT"

```
    /\_/\
   ( ◣_◢ )       OPERATION BLACKCAT
    > ^ <        Digital Investigation Division
   /_____\       Classified — Investigator Use Only
```

---

| Field | Detail |
|---|---|
| **Case Reference** | DI-2026-0326 |
| **Date Filed** | 26 March 2026 |
| **Status** | ACTIVE — EVIDENCE COLLECTION |
| **Classification** | RESTRICTED |
| **Assigned To** | [Investigator Name] |
| **Supervising Officer** | DI Moreno, Cybercrime & Cultural Property Unit |

---

## SITUATION REPORT

The investigation into the theft at **Building 34** began at **23:51 UTC on March 25**, when a silent environmental alarm was triggered in Archive Vault A. 

During the immediate Incident Response, a GSOC (Global Security Operations Center) Analyst performed a spatial digital sweep of the area. They identified a high-resolution photograph (attached as `campus_photo.jpg`) posted to a public photo-sharing platform. 

The photo was geotagged in the immediate vicinity of Building 34 and was uploaded mere minutes before the alarm. While the post was deleted shortly after, the file and its metadata were preserved by the analyst. Preliminary analysis of the unscrubbed EXIF headers suggests the photographer is a former employee with deep technical knowledge of the vault's infrastructure. 

Further intelligence indicates the suspect has been coordinating with an external buyer. Their physical movements were tracked via cell tower triangulation (IMEI `356789045623781`).

On **March 27**, a second mobile device (IMEI `490154203237518`) was found abandoned at **Paddy Coyne's Irish Pub** in Bellevue. This device contains persistent location logs showing a significant convergence with our primary suspect at a facility in Redmond late on the night of the theft. Most recently, the device recorded a stationary metadata event at **Pike Place Market** on March 27 at 11:42, near a specific stall known for its distinctive slogan.

**The "Greenberg Memo" has not been recovered.**

---

## YOUR ASSIGNMENT

You are the lead digital investigator on Case DI-2026-0326.

You have been provided with:

1. A high-resolution photo and metadata headers preserved from a deleted Flickr upload — **`campus_photo.jpg`**
2. Raw cell tower connection logs for IMEI **356789045623781** (Suspect) and IMEI **490154203237518** (Accomplice) — **`cell_tower_log.csv`**
3. GPS track data extracted from the suspect's cloud account and the abandoned device found in Bellevue — **`suspect_gps.gpx`** and **`buyer_gps.gpx`**
4. This case file

Your task is to **identify the suspect**, **reconstruct their movements** in the days before and after the theft, and **locate the stolen collection**.

Work through each phase in order. Document every source, URL, and timestamp. The BlackCat division relies on open-source intelligence — no warrants, no covert tools. Everything you need is publicly accessible.

---

## PHASE 1 — Digital Forensics: The Campus Photo

A photograph (`campus_photo.jpg`) was recovered from iCloud backup logs tied to a device registered to an unknown party. The photo appears to have been taken on the Microsoft campus.

> **Investigator Note:** All answers you need are in the metadata embedded in the photo file. Use any EXIF extraction tool (ExifTool, Jeffrey's Exif Viewer, or similar).

---

**Q1.1** — What camera make and model was used to take this photograph?

**Q1.2** — What GPS coordinates are embedded in the EXIF data? Provide in decimal degree format.

**Q1.3** — Using the GPS coordinates, identify the campus location where this photo was taken. What named structure or landmark is depicted in the photograph?

**Q1.4** — The EXIF metadata contains an "Artist" field with a partial username. What value is recorded?

**Q1.5** — What date and time was the photo taken, according to the EXIF timestamp?

---

## PHASE 2 — Digital Footprint: Tracing the Suspect

Using the username fragment from Phase 1, locate the suspect's online presence across multiple platforms.

> **Investigator Note:** The suspect maintained a consistent alias across platforms. Start with Flickr — the Artist field maps directly to a username.

---

**Q2.1** — Search Flickr for the username identified in Q1.4. What is the full Flickr username of this account?

**Q2.2** — One of the suspect's Flickr photos is captioned with a phrase about a building where "history sleeps." What Microsoft campus building number does the caption reference?

**Q2.3** — The suspect's Flickr account contains a geotagged photo at a famous Seattle public market. What iconic animal sculpture within that market is visible in the photo?

**Q2.4** — On March 27 at 11:42, the recovered accomplice device (IMEI 490154203237518) was tracked to a specific business at Pike Place Market. Use their official website to identify their unique five-word slogan.

**Q2.5** — What is the name of this Pike Place business where the March 27 exchange likely occurred?

**Q2.6** — Find the suspect's Instagram account, which follows the same naming convention as the Flickr username. What is the Instagram handle?

**Q2.7** — The suspect's Instagram posts show visits to two Seattle locations between March 22–24. Name both locations.

**Q2.8** — What is the full URL of the suspect's personal blog?

---

## PHASE 3 — Open Source Review Intelligence: TripAdvisor

The suspect maintained a TripAdvisor reviewer profile under a username consistent with their other accounts. Three reviews posted in the week of 22–27 March 2026 are of investigative significance.

> **Investigator Note:** Search TripAdvisor for reviewers matching the suspect's username pattern. Check their full reviewer profile for all recent activity.

---

**Q3.1** — What Seattle music venue did the suspect review on 25 March 2026?

**Q3.2** — According to the TripAdvisor review text, at what time did the suspect leave that venue on the evening of 24 March 2026?

**Q3.3** — The suspect reviewed a restaurant in Redmond on 26 March 2026 (covering a visit the previous evening). What is the name of that restaurant?

**Q3.4** — What does the suspect describe as making the restaurant's location "convenient" in their review?

**Q3.5** — The suspect posted a third review, for an Irish pub in Bellevue, dated 27 March 2026. What is the name of that pub?

**Q3.6** — Visit the pub's official website. According to their "About" or "News" section, what are they now open for?

---

## PHASE 4 — Blog Intelligence: The Written Record

The suspect maintained a personal travel and technology blog. A post published in the week of the theft contains both a description of the stolen collection and a comment that places the artifact at a specific location.

> **Investigator Note:** Read the full blog post and all reader comments — not just the article body. Comments are posted by secondary accounts and are not indexed by search engines.

---

**Q4.1** — What is the title of the blog post published on or around 22 March 2026?

**Q4.2** — In the blog post body, what specific collection does the suspect describe seeing "up close" during their campus visit?

**Q4.3** — A comment on the post was left by user `altair_88`. What street name does this comment reference?

**Q4.4** — What unit number does the `altair_88` comment reference?

**Q4.5** — A second comment, posted later, provides instructions for the March 27 hand-off. What punny four-word phrase does the commenter use to describe the meeting spot at the market?

---

## PHASE 5 — Cell Tower Analysis: Mapping the Route

The attached file `cell_tower_log.csv` contains connection logs between 24 March and 26 March 2026 for IMEI 356789045623781 and one additional device of interest. Each row contains an IMEI, timestamp, tower ID, descriptive location, and GPS coordinates, sorted chronologically.

> **Investigator Note:** Filter by IMEI 356789045623781 to isolate the primary suspect's movements. Note any other devices that appear at the same towers and times — they may indicate contact with an associate.

---

**Q5.1** — Which East Link light rail station is associated with the cell tower ping at approximately 08:52 on 25 March 2026? What street is this station located on?

**Q5.2** — At what time does the device connect to the cell tower closest to Building 34 on the Microsoft campus?

**Q5.3** — The device appears in the Bellevue area in the early hours of 26 March 2026. What street do the two Bellevue tower pings (BEL-156-3391) correspond to?

**Q5.4** — The final ping before the log ends shows movement toward SeaTac Airport. At what time does this ping occur, and what does it suggest about the suspect's next move?

---

### GPS Track Analysis

Two GPS track files have been recovered from devices involved in this case:
- **`suspect_gps.gpx`** — extracted from the primary suspect's iCloud backup
- **`buyer_gps.gpx`** — extracted from a device found abandoned at Paddy Coyne's Irish Pub by staff on 27 March 2026

> **Investigator Note:** Load both files into a GPS analysis tool (GPX.Studio, Google Earth, QGIS, or similar). All timestamps are UTC — Seattle PDT = UTC−7. Overlay the two tracks and look for temporal and spatial proximity.

---

**Q5.5** — Overlay both GPS tracks on a map. At what two locations do the two devices appear within 100 metres of each other on the night of 25–26 March 2026? Provide the street name or business name for each.

**Q5.6** — Based on the buyer's GPS track, from which city or neighbourhood did their device begin recording on the morning of 26 March?

---

## PHASE 6 — Location Intelligence & Final Report

Combine all gathered intelligence to locate the stolen collection.

---

**Q6.1** — At 00:44 on 26 March, the device pinged tower RDM-WIL-5512 (47.6809°N, 122.1423°W) in Redmond — the first new location after the theft at Building 34. Cross-reference these coordinates with local business listings. What self-storage facility is within 200 metres of this tower?

**Q6.2** — The blog comment from `altair_88` and the Redmond tower ping (RDM-WIL-5512) both point to the same street. What unit number at that storage facility is the stolen collection believed to be held in?

**Q6.3** — Construct a full timeline of the suspect's movements from 24 March to 26 March 2026. Use the table below as your submission:

| Date/Time | Location | Source | Activity |
|---|---|---|---|
| 24 March — evening | | | |
| 25 March — 08:11 | | | |
| 25 March — 08:52 | | | |
| 25 March — daytime | | | |
| 25 March — 23:51 | | | |
| 26 March — 00:44 | | | |
| 26 March — 02:08–03:44 | | | |
| 26 March — 07:19 | | | |

**Q6.4** — Based on all gathered intelligence, who is the suspect? Provide: full name, suspected alias, Flickr handle, Instagram handle, blog URL, and TripAdvisor username.

---

## FINAL FLAG SUBMISSION

The final flag encodes the storage location of the stolen artifact.

**Format:** `BC{streetname_unit##}`

- Street name: the primary street of the storage facility (use underscores, lowercase, abbreviated as in an address — e.g. `ne_40th_st`, `park_ave`)
- Unit: the specific unit number

**Example (not the answer):** `BC{main_st_unit07}`

Submit your flag:

```
BC{___________________}
```

---

## INVESTIGATOR RESOURCES

### Recommended Tools

| Tool | Use |
|---|---|
| ExifTool / Jeffrey's Exif Viewer | EXIF metadata extraction |
| Google Maps / what3words | GPS coordinate lookup |
| Flickr map search | Geotagged photo search by location |
| Instagram location/hashtag search | Social media trail |
| TripAdvisor profile search | Reviewer activity lookup |
| OpenCelliD / Mozilla Location Service | Cell tower GPS cross-reference |
| GPX.Studio / Google Earth / QGIS | GPS track overlay and proximity analysis |
| BNSF Transit / Sound Transit maps | East Link route and station lookup |
| Google Maps Street View | Physical location verification |
| Wayback Machine | Archived web content |

### Hints (Request from Facilitator Only)

Three hints are available. Each costs 50 points. Raise your hand to request — do not discuss hints between teams.

---

*"The cat always leaves a trace. Find it."*

```
 /\_/\
( ◣_◢ )
 > ^ <
```

**— Operation BlackCat Digital Investigation Division —**
**Case Reference: DI-2026-0326 | OPERATION ESPRIT**
