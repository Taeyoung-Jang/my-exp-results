---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md", "summaries/session-01_2025-06-15.md"]
description: "Chunked Export splits a large video render into smaller segments to ease processing and avoid crashes."
---

# Chunked Export

**Definition**: A workflow that divides a long‑duration video export into a series of shorter, self‑contained segments (chunks) that can be rendered independently and later re‑assembled, reducing memory and CPU strain on the editing workstation.

## Why Use Chunked Export?
- **Hardware limits**: High‑resolution projects (e.g., 8K) often exceed a single‑machine’s capacity, leading to crashes or excessive render times.
- **Reliability**: Rendering smaller sections minimizes the risk of a complete job failure; if a chunk crashes, only that segment needs to be re‑rendered.
- **Flexibility**: Chunks can be processed on different machines or off‑loaded to cloud resources.

## Recommended Parameters (from [[summaries/session-01_2025-06-15]])
| Parameter | Recommended Value |
|-----------|-------------------|
| **Chunk length** | 5–10 minutes – long enough to keep file count low, short enough to stay within hardware limits. |
| **Method** | Duplicate the master sequence and trim each copy to a clean back‑to‑back range (preferred) or set precise in/out points on a single sequence, ensuring frame‑accurate boundaries to avoid gaps/overlaps. |
| **Export codec** | Use the same [[concepts/mezzanine-codec]] for every chunk (e.g., DNxHR HQ on Windows, ProRes 422 HQ on macOS). |
| **Stitching** | Import the exported chunk files into a new 8K sequence in chronological order and export **once more** with the identical mezzanine preset – effectively a re‑wrap with no additional quality loss. |

## Integration with Other Workflows
- **Proxy workflow**: Edit with low‑resolution proxies to keep the timeline responsive, then switch back to full‑resolution media for chunked export. See [[concepts/proxy-workflow]].
- **Off‑loading**: Individual chunks can be sent to stronger machines via [[entities/adobe-team-projects]] or rendered on cloud workstations such as [[entities/aws-ec2-g-series]] or [[entities/paperspace]].
- **Mezzanine codec consistency**: Keeping a single [[concepts/mezzanine-codec]] across chunks and the final master avoids generation loss.

## Practical Steps in [[entities/adobe-premiere-pro]]
1. Duplicate the master sequence for each desired segment.
2. Trim each duplicate to cover a 5‑10 minute range.
3. Open the **Export Settings** dialog:
   - Container: QuickTime (MOV) – or MXF if required.
   - Codec: DNxHR HQ (or HQX for 10‑bit log footage).
   - Resolution: Full project resolution (8K).
   - Audio: PCM 48 kHz, 24‑bit.
   - Disable "Render at Maximum Depth" and "Use Maximum Render Quality" unless scaling is performed.
4. Export each chunk.
5. Create a fresh 8K sequence, place all chunk files in order, and export using the same settings.

## Benefits Summary
- **Reduced render crashes** by limiting per‑render workload.
- **Scalable** – allows distribution of work across multiple machines or cloud services.
- **Quality preservation** through consistent mezzanine codec usage.
- **Simplified post‑production** – re‑wrapping avoids extra encoding passes.

---
*Related concepts*: [[concepts/mezzanine-codec]], [[concepts/proxy-workflow]]
*Relevant entities*: [[entities/adobe-premiere-pro]], [[entities/adobe-team-projects]], [[entities/aws-ec2-g-series]], [[entities/paperspace]]

See also: [[summaries/session-33_2025-08-15]]