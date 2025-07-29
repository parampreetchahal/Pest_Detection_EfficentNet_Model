```markdown
# 🐛 Insect Classification Using CNN (TensorFlow / Keras)

This project is a Convolutional Neural Network (CNN) model trained to classify 9 different types of crop pests. The model has been trained on a custom dataset and evaluated for real-world accuracy. It can be integrated into agriculture-based pest control solutions for early pest detection.

---

## 📁 Dataset

The dataset consists of insect images organized into 9 classes:

- aphids
- armyworm
- beetle
- bollworm
- grasshopper
- mites
- mosquito
- sawfly
- stem_borer

Each class contains several `.jpg` images of the respective insect. The dataset is structured in standard subfolders under `train`, `validation`, and `test`.

**Google Drive Dataset Link**: [📂 Click to Access Dataset](https://your-link-here)

---

## 🧠 Model Details

- **Architecture**: Custom CNN using Keras Sequential API.
- **Framework**: TensorFlow / Keras
- **Image Size**: 128 x 128
- **Batch Size**: 32
- **Epochs**: 30

---

## 🏁 Training and Evaluation Results

### ✅ **Test Performance**

Loss      : 0.1658
Accuracy  : 94.26%

````

### 📉 **Model Accuracy Curve**
![Accuracy Graph](path/to/accuracy_graph.png)

> The graph shows signs of **overfitting**, as validation accuracy drops after a few epochs. Regularization techniques may help generalize better.

---

## 🔍 Confusion Matrix

![Confusion Matrix](path/to/confusion_matrix.png)

| Class Name      | Precision/Observation |
|-----------------|-----------------------|
| aphids          | 100% (65/65)          |
| armyworm        | 100% (67/67)          |
| beetle          | 94.2% (66/70)         |
| bollworm        | ~61% (38/62)          |
| grasshopper     | 100% (54/54)          |
| mites           | 96.3% (63/65)         |
| mosquito        | ~91% (41/45)          |
| sawfly          | ~93% (53/57)          |
| stem_borer      | 100% (62/62)          |

---

## 🧪 Prediction Example

You can predict any insect image with:

```python
class_names = ['aphids', 'armyworm', 'beetle', 'bollworm', 'grasshopper', 'mites', 'mosquito', 'sawfly', 'stem_borer']
preds = model.predict(x)
predicted_class = class_names[np.argmax(preds)]
````

---

## 💾 Model Saving

```python
model.save('/desired/path/insect_model.h5')
```

---

## 🛠️ Future Improvements

* Add **dropout**, **batch normalization**, or **data augmentation** to reduce overfitting.
* Experiment with **transfer learning** (e.g., MobileNet, ResNet50).
* Improve dataset diversity to help generalization.
* Deploy using Flask or Streamlit.

---

## 🙋‍♂️ Author

**Parampreet Singh**
B.Tech CSE, Graphic Era Hill University
📧 Email: [param.cse@gehu.ac.in](mailto:param.cse@gehu.ac.in)

---

## 📄 License

MIT License

```

---

### ✅ To finalize:
Replace:
- `https://your-link-here` with your Google Drive link.
- `path/to/accuracy_graph.png` and `path/to/confusion_matrix.png` with relative GitHub paths to those images.

Would you like me to generate the GitHub folder structure or README preview with your images embedded?
```
