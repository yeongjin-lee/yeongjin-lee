## Hi, I'm Yeongjin Lee 👋

I am an undergraduate researcher at VCMI Lab, Seoul Women's University, working on medical imaging AI with a focus on the reliability of foundation models and MLLMs.

My research began with zero-shot bowel segmentation in MRE and has since moved toward verifying model predictions in Crohn's disease detection — using MLLMs to check whether detector candidates are spatially consistent with independently predicted lesion regions. I am currently interested in whether such verification can be grounded in the model's internal representations rather than its outputs alone.

📫 **Contact**:  [📧 yeongjinlee@swu.ac.kr](mailto:yeongjinlee@swu.ac.kr) |  [💼 LinkedIn](https://www.linkedin.com/in/yeongjin-lee)

---
## 🔬 Research Interests
- **Trustworthy Medical AI**: Verifying whether model predictions are grounded in actual image evidence
- **Interpretability of MLLMs**: Internal representations, visual grounding, and intervention-based analysis
- **Foundation Models under Clinical Constraints**: Zero-shot adaptation with limited pixel-level annotation
---
## 🛠️ Technical Skills
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

- **Medical Imaging**: nnU-Net, MRSegmentator, MONAI, NiBabel, SimpleITK, ITK-SNAP
- **Vision-Language Models**: prompt design and evaluation for zero-shot medical inference (GPT, Qwen-VL)
---
## 🧪 Research

### **False Positive Reduction via MLLM-based Verification** *(ongoing)*

*Verifying detector predictions against independently predicted lesion regions.*

- **Key Problem**: Detectors trained for high sensitivity produce many false positives in MRE bowel inflammation detection.
- **Approach**: A two-stage zero-shot verification pipeline — an MLLM judges inflammation presence and outputs candidate lesion locations, which are then compared against detector boxes for spatial consistency.
- **Open Question**: Model-predicted locations are themselves outputs. Whether the model actually relied on that region remains unverifiable at the output level — which motivates my interest in internal representations.

---

### **Zero-shot Bowel Segmentation on MRE**

*Investigating the robustness of foundation models in practical clinical settings.*

- **Key Problem**: Performance degradation due to anisotropic voxel spacing and protocol variability in Crohn's disease MRE.
- **Approach**: Applied **MRSegmentator** in a zero-shot setting with tailored preprocessing, including isotropic resampling and morphological post-processing.
- **Impact**: Improved segmentation performance (**Dice: 69.5 → 81.0**) and applied the pipeline to cohort-level clinical data analysis.
---
## 🏆 Honors & Awards

**KMMS 2025 Fall Conference – Excellence Award (First Author)** 🏆  
*Korea Multimedia Society (National Academic Conference)*  
- Presented research on *"Zero-Shot Bowel Segmentation in MRE using Foundation Models"*.
- Conducted qualitative and quantitative evaluation of **baseline zero-shot segmentation performance**.

**DACON 2025 Medical AI (MAI) Challenge – Top 8% (38 / 477)** 📈  
*Korea’s largest AI competition platform*  
- Developed a two-phase training framework for **genomic language models (gLMs)**.
- Improved sensitivity to **single-nucleotide variants (SNVs)** using cosine-distance metrics.

**Hult Prize OnCampus 2025 – Best Award / Advanced to Hult Prize Korea National** 🏆  
- Proposed an AI-assisted digital data cleanup platform linking carbon reduction with user behavior.  
- *(Note: Source code is private due to ongoing competition regulations)*  
  🔗 Repository: https://github.com/yeongjin-lee/hult-prize-2025-DEW

**SWU 2025 GURU2 Project Competition – Excellence Award** 🏆  
*University-level Project Competition*
- Developed **"Bin-Go"**, a facility-aware running route recommendation service using a **heuristic sector-based routing algorithm** to generate personalized round-trip courses from urban POI data.
- Designed backend routing logic with **adaptive fallback mechanisms** to ensure robustness against **sparse POI distributions**.

---
## 📂 Featured Repositories
*Please check the pinned repositories below for my main research prototypes and experiments.*
