# Software Stack Overview

Welcome to the **Stinger** software stack documentation. This guide covers setup, node architecture, and deployment procedures for the software stack.

---

## 🚀 Quick Navigation

<div class="grid cards" markdown>

-   🛠️ **[Environment Setup](setup.md)**

    ---

    Prerequisites, container setup, dependency installation, and workspace configuration.

-   🧠 **[Core Architecture](architecture.md)**

    ---

    ROS 2 node hierarchy, messaging protocols, data pipelines, and behavior tree execution.

-   📡 **[Interfaces & Drivers](interfaces.md)**

    ---

    Sensor driver configurations, actuator protocols, and communication bridge specifications.

-   🧪 **[Testing & Simulation](testing.md)**

    ---

    Gazebo simulation execution, unit testing, integration tests, and hardware-in-the-loop (HIL).

</div>

---

## 📊 System Requirements & Status

| Component | Target / Version | Status |
| :--- | :--- | :--- |
| **OS** | Ubuntu 24.04 LTS (Noble Numbat) | <span style="color:green;">✔ Supported</span> |
| **Middleware** | ROS 2 Jazzy Jalisco | <span style="color:green;">✔ Supported</span> |
| **Container Engine** | Docker Engine / Apptainer | <span style="color:green;">✔ Recommended</span> |
| **Python** | 3.12+ | <span style="color:green;">✔ Supported</span> |

---

## ⚡ Quick Start

Execute the following commands to clone the workspace, install dependencies, and build the stack:

```bash
# 1. Clone repository
git clone [https://github.com/your-org/stinger-software.git](https://github.com/your-org/stinger-software.git)
cd stinger-software

# 2. Build environment using container runner
docker compose up -d

# 3. Build workspace
colcon build --symlink-install
source install/setup.bash
```

---

## 🛠️ Software Stack Architecture

```text
       +-----------------------------------------------+
       |             Behavior & Mission Control        |
       +-----------------------------------------------+
                                |
                                v
       +-----------------------------------------------+
       |       Navigation / State Estimation / Vision  |
       +-----------------------------------------------+
                                |
                                v
       +-----------------------------------------------+
       |       Hardware Interfaces & Low-Level Drivers |
       +-----------------------------------------------+
```

---

### Key Operational Guidelines

1. **Safety First:** Always test mission nodes in simulation prior to deployment on hardware.
2. **Deterministic Builds:** Run `colcon build` with clean workspaces before field tests.
3. **Logging:** Standard node output must route through ROS logging levels (`INFO`, `WARN`, `ERROR`).
