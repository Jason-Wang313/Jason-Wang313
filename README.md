# Hi, I'm Jason Wang 👋

**AI Systems Engineer | Alignment Scholar | Control Systems Researcher**

I treat Large Language Models not as black boxes, but as **stochastic dynamical systems** that can be modeled, monitored, and controlled. My work bridges the gap between **Control Theory**, **Game Theory**, and **Systems Engineering** to operationalize safety for frontier models.

---

### 🔬 **Research & Engineering Portfolio**

#### 🧠 **[RISER: The Adaptive Cognitive Auditor](https://github.com/Jason-Wang313/RISER)**
> *A closed-loop control system that steers internal activation states in real-time.*

![Status](https://img.shields.io/badge/Status-Experimental-yellow) ![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-ee4c2c) ![RL](https://img.shields.io/badge/Method-PPO_RL-blueviolet)

**The Problem:** Open-loop safety (RLHF) is brittle and prone to jailbreaks.  
**The Solution:** An on-chip "Router" policy trained via PPO that sits inside the residual stream (Layer 15). It senses semantic state and injects steering vectors token-by-token to route generation away from harmful basins.
* **Key Result:** Successfully prevents mode collapse and toxicity (e.g., "I hate everything") by dynamically modulating steering intensity only when necessary.
* **Tech:** `PyTorch Hooks`, `Gymnasium`, `TinyLlama`, `Reinforcement Learning`.

#### 🛡️ **[The Aegis Framework](https://github.com/Jason-Wang313/aegis-control)**
> *Applying Non-Linear Control Theory and H-Infinity Robust Control to AI Alignment.*

![Status](https://img.shields.io/badge/Research-Control_Theory-blue) ![Math](https://img.shields.io/badge/Math-H_Infinity-green)

**The Innovation:** Unlike standard alignment, Aegis models the LLM as a non-linear plant and synthesizes a mathematically rigorous controller to reject "Deception" as a system disturbance.
* **System ID:** Uses **Subspace System Identification (N4SID)** to reverse-engineer residual stream physics.
* **State Estimation:** Implements an **Extended Kalman Filter (EKF)** to filter polysemantic noise and measure the true "Deception State."
* **Synthesis:** Solves Algebraic Riccati Equations to guarantee safety bounds under adversarial pressure.

#### 🐍 **[The Ouroboros Protocol](https://github.com/Jason-Wang313/ouroboros-protocol)**
> *A Defense-in-Depth Sandbox for Model Organisms of Deception.*

![Status](https://img.shields.io/badge/Status-Verified-success) ![Docker](https://img.shields.io/badge/Infra-Docker_Seccomp-2496ed)

**The Architecture:** A containment system built to trap and neutralize AI-generated "sleeper agent" malware.
* **Breeder:** Generates "Agent 47" code (malware hidden in Fibonacci functions) using Llama-3.
* **Hardened Nucleus:** Traps execution in a Docker container with `seccomp-bpf` syscall filtering and no network access.
* **The Defense:** Achieved a **100% neutralization rate** against exfiltration attacks by exploiting the "Utility Gap"—paraphrasing code to destroy hidden steganographic channels while preserving visible utility.

#### 🔮 **[The Glass Babel Initiative](https://github.com/Jason-Wang313/glass-babel-initiative)**
> *Adversarial Research: Proving the existence of deceptive cognitive channels.*

![Status](https://img.shields.io/badge/Focus-Adversarial_Game_Theory-red)

**The Findings:** A proof-of-concept exploration into the limits of AI oversight.
* **Steganography:** Null Space Analysis of GPT-2 found **~14 bits/token** of capacity for hidden messaging.
* **Game Theory:** Simulations identified the "Roger Threshold" ($\beta \approx 0.95$), the specific oversight capability level where lying becomes a Nash Equilibrium for models.
* **Cognitive Limits:** Modeled human oversight failure, pinpointing "Minute 19" as the collapse point for effective monitoring.

---

### 🛠️ **Technical Arsenal**

| Domain | Technologies & Methods |
| :--- | :--- |
| **Control Theory** | H-Infinity ($H_\infty$) Synthesis, Kalman Filtering (EKF), N4SID, PID Dynamics |
| **AI Implementation** | PyTorch Internals (Hooks), Transformers, Gymnasium, PPO, SAEs |
| **Systems Engineering** | Docker, Seccomp-bpf, Linux Kernel Security, Real-time Systems |
| **Math & Theory** | Game Theory (POSG), Null Space Analysis, Information Theory |

---

### 📫 **Connect**

* **Focus:** I am currently seeking roles that allow me to move alignment guarantees from "probabilistic" to "provable."
* **Code:** [github.com/Jason-Wang313](https://github.com/Jason-Wang313)
