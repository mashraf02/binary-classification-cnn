## Dataset

This project uses an image dataset containing photographs of **Asian Elephants** and **African Elephants** for binary image classification. The dataset is organized into training, validation, and test subsets and is used to evaluate the effectiveness of transfer learning and image preprocessing techniques on species recognition.

### Dataset Characteristics

| Feature                | Description                      |
| ---------------------- | -------------------------------- |
| Task                   | Binary Image Classification      |
| Classes                | Asian Elephant, African Elephant |
| Data Type              | RGB Images                       |
| Input Resolution       | 224 × 224 Pixels                 |
| Preprocessing Variants | Original, CLAHE, Sobel           |
| Dataset Split          | Train, Validation, Test          |
| Deep Learning Models   | ResNet-50, DenseNet-121          |
| Framework              | PyTorch                          |

### Classes

| Label | Class            |
| ----- | ---------------- |
| 0     | Asian Elephant   |
| 1     | African Elephant |

### Image Preprocessing Techniques

#### Original Images

Raw images without additional enhancement.

#### CLAHE (Contrast Limited Adaptive Histogram Equalization)

Enhances local image contrast and highlights visual details while preventing over-amplification of noise.

#### Sobel Edge Detection

Extracts edge and shape information by emphasizing object boundaries and structural features.

### Dataset Structure

```text
dataset/
│
├── train/
│   ├── asian_elephant/
│   └── african_elephant/
│
├── validation/
│   ├── asian_elephant/
│   └── african_elephant/
│
└── test/
    ├── asian_elephant/
    └── african_elephant/
```

### Source Dataset

The elephant image dataset can be obtained from Kaggle:

https://www.kaggle.com/datasets

Search Keywords:

* "Asian vs African Elephant Dataset"
* "Elephant Species Classification Dataset"

> Note: The dataset was further processed to create CLAHE-enhanced and Sobel-filtered versions for comparative analysis of preprocessing effects on deep learning performance.
