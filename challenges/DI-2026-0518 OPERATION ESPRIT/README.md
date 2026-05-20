# OPERATION ESPRIT — Case Briefing

```
    /\_/\
   ( ◣_◢ )       OPERATION BLACKCAT
    > ^ <        Digital Investigation Division
   /_____\       Classified — Investigator Use Only
```

## THE INCIDENT: BUILDING 34

On **March 25, 2026, at 23:51 UTC**, a silent environmental alarm triggered in Archive Vault A, Building 34 (Redmond Campus). 

Initial physical inspection confirmed the theft of **"The Greenberg Memo"**. This 1978 internal memorandum is the primary historical record for the original Microsoft group photo. Due to its provenance, it is a high-value target for private collectors, with an estimated street value of **$750,000**.

CCTV in the archive wing failed due to a "corrupted" storage pointer at roughly 23:45. No biometric alarms were logged, indicating the use of valid—likely social-engineered or cloned—credentials.

---

## THE INITIAL SWEEP

Following the alarm, Global Security Operations (GSOC) performed a geofenced sweep of public social media platforms for the Redmond campus area. 

A deleted Flickr upload, geotagged less than 300m from the archive, was flagged during the incident window. While the post was removed within minutes, GSOC managed to archive the image and its header metadata. Preliminary analysis of the file reveals an "Artist" string that matches a former employee terminated six months ago. Due to the sensitivity of the internal HR file, this individual is currently designated as **Subject Alpha**.

---

## THE RECOVERY

On **March 27**, a mobile device (IMEI `490154203237518`) was recovered by local staff at a hospitality venue in the Bellevue area. 

Encrypted location logs on this device show a brief convergence with a second device (IMEI `356789045623781`) at a facility in the Redmond area late on the night of the theft. Access to the secondary device's owner is restricted; we believe this "Subject Bravo" is the buyer.

---

## MISSION OBJECTIVES

You are tasked with reconstructing the timeline and securing the memo.

1.  **Identify Subject Alpha**: Use the evidence from the Flickr upload to confirm the suspect's identity and online footprint.
2.  **Verify the Hand-off**: Document the movement of both devices to confirm if and where a physical exchange occurred.
3.  **Locate the Asset**: Identify the final destination of the stolen collection.

### Investigation Assets:
*   [PARTICIPANT.md](PARTICIPANT.md) — Case log and evidence checklist.
*   `campus_photo.jpg` — Preserved Flickr evidence.
*   `cell_tower_log.csv` — Network telemetry for the suspect device.
*   `suspect_gps.gpx` & `buyer_gps.gpx` — Location forensics.

---

*“History is just another vault. Someone always has the keys.”*
