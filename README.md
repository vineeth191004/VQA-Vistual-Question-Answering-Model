## README: Question-Answering Image Captioning System

### Overview

This project implements a **Question-Answering (QA) Image Captioning System** that combines image processing with natural language understanding. The system takes an image and a question as input and predicts an appropriate answer using deep learning models. The architecture involves feature extraction using MobileNetV2, sequence modeling using LSTMs, and beam search for accurate answer generation.

---

### Requirements

#### Dependencies
To run this code, you need the following libraries:
- Python 3.10+
- TensorFlow
- NumPy
- Matplotlib
- scikit-learn
- Pillow (PIL)
- Spacy

You can install the dependencies using:
```bash
pip install tensorflow numpy matplotlib scikit-learn pillow spacy
```

---

### Dataset

The system requires the following datasets:
1. **Image Data**
   - Training images are stored in `/content/drive/MyDrive/train` and `/content/drive/MyDrive/train2`.
   - Validation images are stored in `/content/drive/MyDrive/valid`.
   - Test images are stored in `/content/drive/MyDrive/test`.

2. **Annotations**
   - Annotations are JSON files located at:
     - Training: `/content/train_combined.json`, `/content/train2_combined.json`
     - Validation: `/content/valid_combined.json`
     - Testing: `/content/test_combined.json`

Each annotation file should contain objects with `image_path`, `Q` (question), and `A` (answer) fields.

### Outputs

- Predicted answers for input questions on test images.
- Visualized test results (image, question, actual answer, predicted answer).

---

### Example Usage

**Input**:
- Image: *`sample_test_image.jpg`*
- Question: "What is shown in the picture?"

**Output**:
- Predicted Answer: *"A cat sitting on a chair."*
