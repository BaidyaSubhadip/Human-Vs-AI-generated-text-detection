# Statistical Analysis of Human vs AI Generated Text

## 📌 Overview
This Statistical Analysis contains analysis comparing **human-written** text with **AI-generated** text using entropy-based metrics.  
The core objective is to explore whether **Entropy distributions** can help distinguish between human authorship and outputs from modern large language models.

---

## 📂 Data Sources

### **1. Human-Generated Text**
We used the *Human vs AI Text* dataset from Kaggle:  
🔗 https://www.kaggle.com/datasets/shanegerami/ai-vs-human-text

This dataset provides verified human-written paragraphs used as the baseline for comparison.

### **2. Writing Prompts for AI Generation**
AI-generated texts were produced using prompts sampled from:  
🔗 https://huggingface.co/datasets/euclaise/writingprompts

These prompts served as inputs to various large language models.

---

## 🤖 AI Models Used
We generated AI-written paragraphs using the following models:

- **deepseek-r1:latest**
- **qwen2.5:7b**
- **llama3.2**

All models were evaluated using identical prompt sets to ensure fairness in comparison.

---

## 🧪 Methodology

1. Extract human-written text samples from the Kaggle dataset.  
2. Select writing prompts from the HuggingFace WritingPrompts dataset.  
3. Generate AI responses using the selected LLMs.  
4. Compute entropy-based metrics for each text sample, including:
   - Token-level entropy  
   - Normalized entropy  
   - Averaged entropy across sequences  
5. Perform statistical analysis and visualization:
   - Histograms  
   - KDE (Kernel Density Estimation) curves  
   - Comparative distribution plots  

All generated figures are stored in the **`figures/`** folder.

---

## 📊 Visualizations
Below are some of the plots included in the analysis (all available in `figures/`):

- `figures/humanText_plot.jpg`
- `figures/llama3.2_3b_plots.jpg`
- `figures/qwen2.5_7b_plots.jpg`


## 📁 Repository Structure

