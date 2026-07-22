# 🔥 VR Fire Extinguisher Trainer — Demo Build

**A fully functional VR training simulator for fire extinguisher operation**, built with a custom rapid-development framework for industrial VR trainers.

[![Watch the Demo](https://img.shields.io/badge/▶%20Watch%20Demo-YouTube-red?style=for-the-badge&logo=youtube)](https://youtube.com/shorts/ZgqOn2Nq9HI?feature=share)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/Hire%20Me-LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/egor-fetisov-97a409304/)

---

## 📹 See It in Action

**[▶ Full scenario walkthrough on YouTube](https://youtube.com/shorts/ZgqOn2Nq9HI?feature=share)**

8 steps, from walking into a burning office to complete extinguishment — no cuts, real-time VR.

---

## 🏢 About the Scenario

The trainee spawns inside a loft office with an active fire. The simulation guides them through the full, physically accurate fire extinguisher operation procedure:

| Step | Action |
|------|--------|
| 1 | Spawn in office — fire detected |
| 2 | Locate the extinguisher |
| 3 | Approach and assess |
| 4 | Pull the safety pin |
| 5 | Aim the nozzle at the base of the fire |
| 6 | Squeeze the handle |
| 7 | Sweep — extinguish completely |
| 8 | Confirm: fire out, scenario complete |

**Environment:** baked-lighting loft office, high-detail fire extinguisher model, physically accurate hose with correct deformation behavior.

**Target platform:** Meta Quest (standalone build)

---

## 🛠 Tech Stack

| Category | Technology |
|---|---|
| Engine | Unity 6 |
| Render Pipeline | URP |
| XR Standard | OpenXR |
| Asset Management | Addressables |
| Dependency Injection | Zenject |
| Async | UniTask |
| Animation / Tweening | DOTween |
| Scenario Logic | Custom ScenarioSystem (xNode-based graph editor) |
| VR Interactions | Custom abstract layer over XR interaction frameworks |

---

## ⚙️ Built on a Custom VR Trainer Framework

This project was assembled using two proprietary tools built from the ground up for industrial training simulations.

### ScenarioSystem

A visual, node-graph scenario editor distributed as a **UPM package** for Unity:

- **xNode-powered** graph editor — scenarios are built visually, not in code
- **Event-driven architecture** — fully decoupled, reactive logic
- **MVC pattern** — clean separation between data, logic, and presentation
- **Barrier synchronization** — multi-condition transitions between steps (wait for N events before advancing)
- **DI-agnostic** — plug in Zenject, VContainer, or no DI at all

### VR Trainer Framework

Built on top of ScenarioSystem, purpose-built for rapid assembly of industrial VR trainers:

- **Steps → Interactions → Hints** pipeline — consistent structure across any training topic
- **Abstract VR interaction layer** — swap the underlying XR framework (XRI, Autohand, etc.) without rewriting scenario logic
- Reusable components across different training scenarios

> **Bottom line:** once the framework is in place, a new VR training scenario can be assembled and delivered in days, not months. The fire extinguisher demo is proof.

---

## 💼 Available for Custom VR Training Projects

I build VR training simulators for companies that need:

- 🔥 Fire safety & emergency response training
- 🏭 Equipment operation and industrial procedures
- 👷 Workplace hazard and OHS compliance training
- 🎓 Any step-based instructional scenario

**Who I work with:** occupational health & safety providers, HR and training departments at industrial enterprises, corporate training centers.

📩 **Let's talk about your project:**

- [LinkedIn](https://www.linkedin.com/in/egor-fetisov-97a409304/)
- [Upwork](https://www.upwork.com/freelancers/~011e3a108b65f34052?mp_source=share)
- Email: `skrininshot.trk@gmail.com`
- Telegram: `@skrininshot`

---

## 📦 Test Build

### 🥽 Installation Guide (Meta Quest)

#### Method 1: SideQuest (Recommended)
1. Download and install [SideQuest](https://sidequestvr.com/) on your PC/Mac.
2. Enable **Developer Mode** on your Meta Quest headset (via Meta mobile app).
3. Connect the headset to your PC via USB and authorize the connection in VR.
4. In SideQuest, click the **Install APKs from file** icon (folder) in the top right.
5. Select the downloaded `.apk` file and confirm installation.

#### Method 2: Meta Quest Developer Hub (Official)
1. Download [Meta Quest Developer Hub (MQDH)](https://developer.oculus.com/downloads/package/meta-quest-developer-hub/).
2. Enable **Developer Mode** and connect the headset via USB.
3. Open MQDH, select your device, and navigate to the **Device** tab.
4. Drag and drop the `.apk` file into the MQDH window or use the **Install APK** button.

#### Method 3: ADB (Command Line)
1. Ensure ADB is installed and **Developer Mode** is enabled.
2. Connect the headset via USB and authorize the computer in VR.
3. Open a terminal in the folder containing the `.apk` and run:
   ```bash
   adb install "BaseVR - Fire Extinguisher Demo.apk"

---

<sub>Built with Unity 6 · URP · OpenXR · Addressables · Zenject · UniTask · DOTween · Custom ScenarioSystem</sub>
