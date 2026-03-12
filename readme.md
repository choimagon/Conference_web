<div style="column-count:2; column-gap:40px; text-align:justify;">

# Paper Title Example

**Author:** Jihoon Choi  
**Affiliation:** Sejong University  
**Email:** example@email.com  

---

## Abstract

This document demonstrates how Markdown can be displayed in a two-column layout similar to a research paper.

Standard Markdown does not support multi-column layouts, but HTML and CSS can be embedded inside Markdown to simulate a paper-style format.

This method is useful when writing drafts, notes, or technical documentation that visually resembles academic papers.

---

## 1. Introduction

This section begins in the left column.

Markdown syntax works normally inside the HTML block.

You can use:

- **bold text**
- *italic text*
- `inline code`
- links

Example:

[Example Link](https://example.com)

If the text becomes long enough, the content automatically flows into the second column.

This behavior is similar to the layout used in many academic papers.

---

## 2. Related Work

Feature matching has been widely studied in computer vision.

Some representative approaches include:

- SIFT
- ORB
- SuperPoint
- SuperGlue
- LightGlue

Recent work focuses on improving both **matching accuracy** and **computational efficiency**.

---

## 3. Method

Our pipeline consists of three main stages:

### 3.1 Feature Extraction

Keypoints are extracted from the input images.

Example pseudo-code:

```python
def extract_features(image):
    keypoints = detector.detect(image)
    descriptors = descriptor.compute(image, keypoints)
    return keypoints, descriptors
```

### 3.2 Feature Matching

Descriptors from two images are compared to find correspondences.

Typical approaches include:

- nearest neighbor search
- ratio test
- attention-based matching networks

### 3.3 Geometric Verification

Outlier matches are filtered using RANSAC.

Example:

```python
H, inliers = cv2.findHomography(pts1, pts2, cv2.RANSAC)
```

---

## 4. Experiment

Experimental setup:

| Item | Description |
|-----|-------------|
| GPU | RTX 3060 |
| Framework | PyTorch |
| Dataset | HPatches |
| Metric | MMA |

Evaluation thresholds:

- 1 px
- 3 px
- 5 px

Results typically show that stricter thresholds emphasize precise correspondences.

---

## 5. Result

At a **1 px threshold**, the difference between methods is relatively small.

At **3 px and 5 px**, performance differences become clearer.

This suggests that while both methods produce accurate matches, their robustness differs when the tolerance increases.

---

## 6. Conclusion

Using HTML inside Markdown allows a simple two-column layout.

Although this approach is not suitable for final academic submissions, it is convenient for:

- research notes
- draft papers
- technical documentation

For final publication, tools such as **LaTeX**, **Pandoc**, or **Quarto** are recommended.

---

## References

[1] D. Lowe, “Distinctive Image Features from Scale-Invariant Keypoints,” IJCV, 2004.  
[2] P.-E. Sarlin et al., “SuperGlue: Learning Feature Matching with Graph Neural Networks,” CVPR, 2020.  
[3] P. Lindenberger et al., “LightGlue: Local Feature Matching at Light Speed,” ICCV, 2023.

</div>