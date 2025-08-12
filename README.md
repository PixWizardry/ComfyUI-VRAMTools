# ComfyUI VRAM Tools

A set of custom nodes for ComfyUI to help you monitor and manage your VRAM and system RAM usage. These tools are designed to provide clear insights into how your workflows are impacting your system's memory, allowing you to optimize for performance and prevent crashes.

## 🛠️ Installation

Follow these simple steps to get the VRAM Tools node up and running in your ComfyUI environment.

### Step 1. Clone the Repository

First, you need to clone this repository into your `ComfyUI/custom_nodes/` directory.

Open your terminal or command prompt and navigate to your ComfyUI installation folder.

**For a standard PC installation:**
```bash
cd ComfyUI/custom_nodes/
git clone https://github.com/PixWizardry/ComfyUI-VRAMTools
```

### Step 2: Restart ComfyUI

After the repository has been successfully cloned, make sure to restart ComfyUI. This will allow it to recognize and load the new custom node.


## ✨ Available Nodes

Here are the nodes included in this package:

### 1. Reset VRAM Peak Counter

This node resets the peak VRAM memory counter in PyTorch. It's a simple but powerful tool for measuring the VRAM consumption of specific parts of your workflow.

*   **What it does:** Resets the counter to zero.
*   **Key Inputs:**
    *   `passthrough_*`: Can accept and pass through any data type (images, models, latents, etc.) without modifying them. This allows you to place it anywhere in your workflow.
*   **Use Case:**
    *   Place this node right before a demanding operation (like a KSampler or a model loader) to measure exactly how much VRAM that specific operation requires.

### 2. Log VRAM Peak Usage

This node logs a detailed snapshot

## 🔎 How to Find the Node in ComfyUI

Once everything is installed, you can find the node under the following category:

*  Right-click on the canvas
*  Select "Add Node"
*  In the next menu, find and click on the **"VRAM Tools"** category.
*  You will see the list of available nodes:
    *   `Reset VRAM Peak Counter`
    *   `Log VRAM Peak Usage`
*  Click on the node you want to add, and it will appear on your canvas.
