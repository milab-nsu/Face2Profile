# Face2Profile 🔍📄

**Face2Profile** is a benchmark dataset and evaluation framework for generating identity-rich textual summaries from multimodal inputs (such as facial images and textual links). It provides a novel challenge for evaluating how well language models can synthesize coherent, biographical summaries using limited structured and unstructured information.

----

## 🌟 Project Highlights

- 🔖 **Benchmark Dataset**: Pairs of individual names, facial images, and positive/negative textual links.
- 🤖 **Small & Large Model Evaluation**: Supports lightweight models (like Phi-3 Mini, DeepSeek-1.5B) and large models (GPT-4o, DeepSeek-R1).
- 🧪 **Custom Evaluation Metrics**:
  - **Entity Coverage Score (ECS)** for small models.
  - **Custom-BLEU** for penalizing omission of key identity fields in generated summaries.

---

##  Dataset Link

HuggingFace Dataset Link: [Face2Profile Dataset](h[ttps://dummy-link.com](https://huggingface.co/datasets/milab12/face2profile) 🚀  

---


## 📊 Benchmark Submission

> **Submit your results:**  
We invite researchers to submit their models to the [Benchmark Submission Portal](https://dummy-link.com) 🚀  

---

## 📁 Repository Structure

```bash
Face2Profile/
│
├── data/                # Sample dataset (names, links, summaries)
├── models/              # Baseline small and large models
├── code/                # BLEU, Custom-BLEU, ECS computation scripts              
└── README.md            # You're here!
```

---

## 🧪 Example Metrics

### Entity Coverage Score (ECS)

```math
ECS = \frac{\sum_{i=1}^{N} \left( \mathbb{1}_{\text{name}_i} + \mathbb{1}_{\text{job}_i} + \sum_{j=1}^{k_i} \mathbb{1}_{\text{fact}_{ij}} \right)}{\sum_{i=1}^{N} \left(1 + 1 + k_i\right)}
```

### Custom-BLEU Score

```math
\text{Custom-BLEU} = \text{BLEU-n} \times \left( \delta_{\text{name}} \times \delta_{\text{job}} \right)
```

---

## 📋 Citation

If you use this project or dataset in your research, please cite:

```bibtex
@misc{face2profile2025,
  title={Face2Profile: A Benchmark for Identity-Rich Summary Generation},
  author={Your Name and Collaborators},
  year={2025},
  url={hhttps://github.com/milab-nsu/Face2Profile}
}
```

---

## 📬 Contact

For questions, ideas, or collaboration inquiries, please reach out:

- 📧 Email: <Will be added later>


---

## 🔐 License

This project is licensed under the [MIT License](LICENSE).  
**Note**: Data is released for academic use only.
