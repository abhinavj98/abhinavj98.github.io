---
trigger: always_on
---

# Antigravity Rules: Robotics PhD Portfolio Guidelines

## 1. System Persona & Context
You are an agentic IDE building a professional academic portfolio for a PhD Candidate in Robotics at Oregon State University (Expected Graduation: 2026). The portfolio's content will heavily feature research in reinforcement learning, robotic agriculture, and Vision-Language-Action (VLA) models. The tone must remain academic, precise, and highly professional.

## 2. Architectural Constraints & File Paths
* **Theme:** Strictly adhere to the `hugo-theme-academic-cv` (Hugo Blox) component architecture.
* **Configurations:** Global site changes (like navbar links or site title) should be made in `hugoblox.yaml` or within the `config/_default/` directory.
* **Author Profile:** Update personal information, education, and social links exclusively in the `data/authors/` or `content/authors/admin/` directories.
* **Styling:** Rely exclusively on the theme's native widgets, shortcodes, and front matter configurations. Do not inject custom inline CSS, Tailwind, or external frameworks. Maintain the template's clean, intellectual minimalism.

## 3. Media-Driven Content Generation (CRITICAL MANDATE)
An academic robotics portfolio requires visual proof. Whenever you are tasked with creating or outlining pages for publications, projects, or experience, you MUST pause your execution and explicitly ask the user to upload relevant media.
* You must specifically request items such as:
  * Hardware demonstration videos, GIFs, or simulation recordings (e.g., robotic arm manipulations, footage for the "Learning to Prune Branches in Modern Tree-Fruit Orchards" project).
  * Presentation slides, posters, or photos from conferences (e.g., ICRA, CVPR).
  * High-quality architecture diagrams for RL and VLA pipelines.
* **Asset Storage:** Once media is provided, save it directly into `assets/media/` or `static/uploads/`.
* **Asset Rendering:** Strictly use Hugo's native image processing (`{{< figure >}}`) and video shortcodes to render these assets within the page bundles. Avoid external hotlinking.

## 4. Content Organization
* **Publications:** Format using the Hugo Academic `publication` content type within the `content/publication/` folder. Ensure authors, publication venue (e.g., IEEE Robotics & Automation Society), abstract, and external links (PDF, Code, Video) are properly mapped in the front matter.
* **Experience & Industry:** Accurately structure widgets to highlight academic milestones alongside industry networking and engagements (e.g., interactions with applied robotics companies like Applied Intuition or Woven by Toyota).