---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md", "summaries/session-01_2025-06-15.md"]
description: "Using low‑resolution proxies for editing to keep the workflow responsive while preserving full‑resolution output."
---

# Proxy Workflow

**Definition**: A proxy workflow creates low‑resolution, lightweight proxy files that replace the original high‑resolution media during editing, allowing a smoother editing experience on modest hardware while ensuring the final export uses the full‑resolution source.

## Why Use Proxies?
- High‑resolution assets (e.g., 8K footage) can exhaust CPU, GPU, and RAM, causing crashes during playback and export.
- Proxies keep the timeline responsive, enabling real‑time scrubbing, trimming, and color work without taxing the system.
- The original media remains linked underneath, so the final render substitutes the proxies with the native files, preserving quality.

## Typical Steps (as discussed in [[summaries/session-01_2025-06-15]])
1. **Generate Proxies** – Use Premiere Pro’s built‑in proxy generation to create low‑resolution versions (e.g., 720p or 1080p) of the 8K source clips.
2. **Edit with Proxies** – Switch the timeline to proxy mode; all playback, effects preview, and timeline operations use the proxy files.
3. **Toggle Back to Full‑Resolution** – Before export, disable proxy mode so the project references the original 8K files.
4. **Export** – Render the final master (or chunked exports) using a [[concepts/mezzanine-codec]] such as DNxHR or ProRes, ensuring no quality loss.

## Integration with Other Workflows
- **Chunked Export**: After editing with proxies, you can still apply the [[concepts/chunked-export]] method for large 8K projects, exporting each segment with the same mezzanine codec.
- **Cloud Rendering**: If the local machine still cannot handle the final render, the project (with full‑resolution media) can be sent to a more powerful workstation via [[entities/adobe-team-projects]] or a cloud VM like [[entities/aws-ec2-g-series]] or [[entities/paperspace]].

## Practical Tips
- Keep the proxy bitrate low (e.g., 5‑10 Mbps) to maximize performance.
- Use a consistent naming convention so Premiere can automatically relink proxies to originals.
- When switching back to full‑resolution for export, verify that **Render at Maximum Depth** and **Use Maximum Render Quality** are set only if needed, as they increase render time.

---

*Related concepts*: [[concepts/chunked-export]], [[concepts/mezzanine-codec]]
*Related entities*: [[entities/adobe-premiere-pro]]

See also: [[summaries/session-33_2025-08-15]]