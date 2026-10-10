---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md"]
description: "A structured set of steps to verify and fine‑tune a workstation after installing a new discrete GPU."
---

## GPU Upgrade Checklist

The **GPU Upgrade Checklist** is a practical workflow for confirming that a newly installed discrete graphics card is fully recognized, correctly configured, and delivering expected performance. It originates from the discussion in [[summaries/session-33_2025-08-15]] and covers hardware, OS, driver, and application layers.

### 1. Hardware Verification
- **Device Manager** – Ensure the new GPU appears under *Display adapters* with no warning icons. If the integrated graphics (iGPU) is still listed, consider disabling it in the BIOS.
- **BIOS Settings** – Set *Primary Display* to PCIe or explicitly disable the iGPU. This prevents the motherboard from defaulting to the integrated output.
- **Cable Connections** – Verify that all monitors are plugged into the discrete GPU’s ports (HDMI/DisplayPort). Use the method described in [[concepts/display-connection-verification]] to confirm which GPU drives each monitor.

### 2. Driver & Power Management
- **Driver Installation** – Install the latest driver from the GPU vendor (e.g., [[entities/nvidia]]). Keep the driver up‑to‑date to avoid stale‑driver issues.
- **Power Plan** – Switch Windows to *High performance* or *Maximum performance* for the GPU. Disable PCI Express Link State Power Management if possible.

### 3. Control Panels & OS Settings
- **GPU Vendor Control Panel** – In the NVIDIA Control Panel (or AMD Adrenalin), set the *Preferred graphics processor* to the high‑performance GPU globally and per‑application.
- **Windows Graphics Settings** – Navigate to *System → Display → Graphics* and assign demanding apps (Photoshop, Premiere, Blender) to *High performance*.
- **Entity Reference** – See [[entities/windows-graphics-settings]] for the Windows UI location.

### 4. Benchmark & Monitoring
- Run a lightweight monitor such as **GPU‑Z** or use the **Task Manager – Performance** tab. Switch to each GPU entry; the *Displays* list indicates which monitor is attached. Observe GPU load when launching a GPU‑intensive task.
- Optionally run a quick benchmark (e.g., Unigine Heaven, Blender benchmark) to verify expected frame rates.

### 5. iGPU vs dGPU Considerations
- Leaving the iGPU enabled is safe if all displays are routed to the discrete GPU. It can be beneficial for Intel Quick Sync video encoding. See [[concepts/quick-sync-utilization]] and [[entities/intel-quick-sync]] for details.
- Beware of apps that default to *GPU 0* (often the iGPU). Override with per‑app Windows graphics settings or the NVIDIA Control Panel.

### 6. Reducing "GPU 0" Stickiness
- **Windows** – Assign each media app to *High performance*.
- **NVIDIA Control Panel** – Set the global *Preferred graphics processor* to the high‑performance NVIDIA GPU.
- This combination minimizes the chance that applications fall back to the integrated graphics.

### 7. Common Gotchas After Upgrade
- Stale or generic Windows drivers.
- Power plan set to *Balanced*, throttling the dGPU.
- Monitors still connected to motherboard video ports.
- Applications left on *Auto* renderer, causing them to pick the iGPU.
- BIOS not disabling the iGPU, leading to resource conflicts after driver updates.

---
*The **GPU Upgrade Checklist** synthesizes these steps into a single reference that can be reused across workstation refresh projects.*