---
sources: ["summaries/session-33_2025-08-15.md", "summaries/session-01_2025-06-15.md"]
type: "Product"
description: "A professional video editing application for Windows and macOS."
---

## Adobe Premiere Pro

Adobe Premiere Pro is a flagship video‑editing product from Adobe, available on Windows and macOS. It provides a timeline‑based interface, robust color‑grading tools, and support for a wide range of codecs and export formats.

### Role in [[summaries/session-01_2025-06-15]]
In the June 15 2025 conversation, Premiere Pro is the editing platform used to create an 8K master. The discussion covered:
- Using a **proxy workflow** to edit low‑resolution proxies while keeping the full‑resolution media linked. [[concepts/proxy-workflow]]
- Exporting the project in **chunks** (5–10 minutes each) to avoid crashes, then stitching the chunks into a final master. [[concepts/chunked-export]]
- Selecting a **mezzanine codec** (DNxHR HQ or HQX) for both the chunk files and the final stitched export to preserve visual quality. [[concepts/mezzanine-codec]]
- Off‑loading the heavy render to remote resources such as **Adobe Team Projects**, **AWS EC2 G‑series**, or **Paperspace**.

### Related concepts
- [[concepts/proxy-workflow]] – low‑resolution editing proxies.
- [[concepts/chunked-export]] – dividing large projects into manageable segments.
- [[concepts/mezzanine-codec]] – intermediate lossless codecs for high‑resolution masters.

### Related entities
- [[entities/adobe-team-projects]] – collaborative cloud workspace for Premiere projects.
- [[entities/aws-ec2-g-series]] – cloud GPU instances for off‑loading renders.
- [[entities/paperspace]] – another cloud workstation option.
- [[entities/avid-dnxhr]] – the DNxHR codec referenced for Windows exports.
- [[entities/apple-prores]] – the ProRes codec mentioned as the macOS counterpart.


See also: [[summaries/session-33_2025-08-15]]