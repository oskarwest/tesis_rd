# CORRECTIONS AND IMPROVEMENTS TO THE ABSTRACT

## CORRECTIONS

### 1. Inaccurate results reporting
**Problem:** The original abstract states "the best multiclass classification model reaches 76.8%" without specifying which metric, and this value is incorrect.

**Correction:** According to experimental results (Table in resultados.tex), the best multiclass model (MobileNetV2 with green channel) achieved 65% sensitivity, 55% accuracy, and 54% F1-score. Corrected to reflect 55% accuracy and 65% sensitivity.

**Justification:** Accuracy in reporting results is fundamental in a scientific abstract. Readers must be able to verify the exact reported figures.

---

### 2. Incomplete dataset description
**Problem:** Only mentions "a public dataset" and "a private dataset provided by the Santander Ophthalmological Foundation" without specifying sizes or other validation sources.

**Correction:** Specified "35,121 images from the Kaggle public dataset" and added external validation datasets (MESSIDOR-2, IDRiD, and FOSCAL).

**Justification:** Dataset size is critical information for evaluating study robustness. External validation is a quality element that should be highlighted.

---

### 3. Missing architecture specification
**Problem:** Says "pretrained networks" without specifying which ones.

**Correction:** Explicitly added: "MobileNetV2, ResNet50V2, InceptionV3, and VGG19"

**Justification:** Specific architectures are relevant information that enables reproducibility and comparison with other works.

---

### 4. Incomplete preprocessing description
**Problem:** Only mentions "preprocessing and image augmentation techniques" without specifying which ones.

**Correction:** Added: "color normalization, peripheral masking, class balancing through subsampling and data augmentation"

**Justification:** Preprocessing techniques are important methodological contributions of the work.

---

### 5. Vague problem statement
**Problem:** "manual diagnosis is challenging because it is costly and time-consuming" lacks specific context.

**Correction:** Contextualized with specific data about Colombia.

**Justification:** Scientific abstracts in medicine should contextualize the problem with specific epidemiological data.

---

## IMPROVEMENTS ADDED

### 1. Clinical motivation with Colombia-specific data
**Added content:** "In Colombia, with a ratio of 1.56 ophthalmologists per 100,000 inhabitants and approximately 1.2 million people with diabetic retinopathy, automated detection represents a critical solution to expand screening coverage."

**Justification:** Medical abstracts should contextualize the problem with specific epidemiological data. This data is in the introduction and is relevant to justify the work.

---

### 2. Global disease prevalence
**Added content:** "affecting 145 million people worldwide"

**Justification:** Dimensioning the problem globally is standard practice in medical research abstracts. The data is available in the introduction.

---

### 3. Specification of architectures and methods
**Added content:** Explicit mention of the four evaluated architectures and the use of transfer learning.

**Justification:** In applied deep learning work, specifying exact architectures is standard in scientific abstracts.

---

### 4. Regularization techniques
**Added content:** "incorporating Multi-Head Attention blocks, GaussianNoise layers, and regularization techniques (Dropout, L2, early stopping)"

**Justification:** Regularization techniques are specific methodological contributions that differentiate this work from basic implementations.

---

### 5. Green channel finding
**Added content:** "identifying the green channel as most effective for multiclass classification due to its better contrast for hemorrhagic lesions"

**Justification:** This is an original and relevant finding that should be highlighted in the abstract. It's a specific contribution to the field's knowledge.

---

### 6. External validation with results
**Added content:** "External validation on MESSIDOR-2, IDRiD, and FOSCAL datasets confirmed the model's generalization capability"

**Justification:** External validation is a fundamental methodological quality indicator in medical machine learning studies. It must be explicitly mentioned.

---

### 7. Complete evaluation metrics
**Added content:** Specification that "sensitivity, precision, F1-score, and AUC-ROC" were used as metrics.

**Justification:** Enumerating specific metrics is standard in medical classification work abstracts.

---

### 8. Specific best model
**Added content:** "MobileNetV2 with preprocessing through filtering and optimized threshold (0.4826) being the best-performing model"

**Justification:** Identifying the specific winning model and its configuration is critical information for reproducibility and comparison.

---

### 9. Confidence intervals
**Added content:** "with bootstrap confidence intervals (95% CI: AUC-ROC 0.9636–0.9936)"

**Justification:** Confidence intervals demonstrate statistical rigor and are increasingly required in medical scientific publications.

---

### 10. Improved structure and flow
**General improvement:** Text reorganized following typical scientific abstract structure:
1. Context and problem (DR as cause of blindness + epidemiological data)
2. Current limitations (shortage of specialists)
3. Work objective
4. Methodology (datasets, architectures, techniques)
5. Main results (binary and multiclass)
6. External validation
7. Conclusion/Contribution

**Justification:** This structure facilitates quick reading and allows finding specific information efficiently, following publication standards in the field.

---

## SUMMARY OF CHANGES

**Total corrections:** 5 errors/inaccuracies corrected
**Total improvements:** 10 elements added to meet scientific standards
**Length:** From ~150 words to ~220 words (increase of ~47%, staying within typical 200-250 word range for thesis abstracts)

**Keywords:** Not modified (they are adequate and complete)
