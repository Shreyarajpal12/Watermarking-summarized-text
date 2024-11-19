# Watermarking AI-Generated Summaries

This repository implements a **watermarking algorithm** for identifying AI-generated summaries by embedding detectable patterns into text. The algorithm demonstrates robust detection capabilities while maintaining text quality, as shown through comparisons of **Z-scores** and **green fractions** in watermarked and non-watermarked text. 

The experiments were conducted using **sequence-to-sequence models** pre-trained on summarization tasks, such as **T5** and **FLAN**, using the **CNN/Daily Mail dataset** as a benchmark. Additionally, comparisons were made between **causal models** and sequence-to-sequence models to evaluate their suitability for summarization and watermarking tasks.

---

## Key Features

1. **Watermarking Algorithm**:
   - Embeds algorithmically detectable, human-invisible patterns into generated text.
   - Assesses text through metrics like Z-scores and green fractions to identify AI-generated content.
   - Ensures minimal impact on text quality while enabling robust detection.

2. **Comparison**:
   - Practical comparisons between **watermarked** and **non-watermarked** text, showcasing the algorithm's effectiveness.
   - Analysis across 60 samples of summaries from the **CNN/Daily Mail dataset**, using **T5 Small** and **FLAN-T5 Large** models.
   - Includes a study of **causal models** and sequence-to-sequence models for this task, highlighting the strengths of the latter.

3. **Results**:
   - Comprehensive metrics for each sample, including:
     - **Number of tokens scored**
     - **Green fraction**
     - **Z-scores**
     - **T-values**
     - **Prediction accuracy**

---

## Experimental Details

- **Dataset**: CNN/Daily Mail summarization dataset
- **Models**: 
  - Sequence-to-sequence models: **T5 Small**, **FLAN-T5 Large**
  - Causal models: Explored but not optimal for summarization tasks
- **Comparisons**:
  - Watermarked vs. Non-watermarked summaries
  - Sequence-to-sequence vs. Causal models

---

## Results and Insights

- **Watermarked Summaries**: Consistently higher Z-scores and green fractions, making detection straightforward.
- **Non-Watermarked Summaries**: Lower Z-scores and green fractions, showing reduced detectability.
- **Sequence-to-Sequence Models**: Outperform causal models for summarization and watermarking effectiveness.
- Results demonstrate the potential of watermarking algorithms for practical use cases, such as ensuring content authenticity in academic or professional settings.

---

## Repository Contents

- **`collab notebook`**: Code for watermarking algorithm implementation.
- **`results/`**: Case study analysis conducted in this exp.
- **`results_{x}.txt files`**: Metrics and comparisons for ~60 samples, summarized using T5 and FLAN models.

---

## References

1. **Paper**: [A Watermark for Large Language Models](https://arxiv.org/abs/2301.10226)  
2. **Code**: [lm-watermarking GitHub Repository](https://github.com/jwkirchenbauer/lm-watermarking.git)  

---

## Getting Started

1. Clone this repository:
   ```bash
   git clone [This Repo](https://github.com/Shreyarajpal12/Watermarking-summarized-text)
   cd Watermarking-summarized-text
   ```

2. Run experiments in the jupyter notebook using Google collab

3. Access results:
   - Metrics and summaries are available in the **`results_{x}.txt`** files.
4. Access analysis:
   - Tabular and graphical analysis on a small segment is conducted and uploaded in the results folder
---

## License

This project is open-source and freely available for academic and research purposes. Please cite the referenced paper and repository if you use this work in your research.
