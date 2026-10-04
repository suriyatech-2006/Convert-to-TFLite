# Convert to TFLite – Light-Level Classifier

**Author:** suriyakumar P

## Task

Train a light-level classifier for **Dark, Normal, Bright**, convert it to a TensorFlow Lite `.tflite` model, and verify inference in Python.

## Categories

| Light Level | Category |
|---|---|
| Below 300 | Dark |
| 300–699 | Normal |
| 700 and above | Bright |

## Files

- `Light_Level_Classifier_TFLite.ipynb` - Google Colab notebook
- `requirements.txt` - Python dependencies

## Workflow

1. Create labeled light-level data.
2. Train a small TensorFlow neural network.
3. Convert the trained model using `tf.lite.TFLiteConverter`.
4. Save the model as `light_level_classifier.tflite`.
5. Load the TFLite model using `tf.lite.Interpreter`.
6. Verify inference in Python.

## Test Values

- 100 → Dark
- 500 → Normal
- 900 → Bright

Open the notebook in Google Colab and run all cells. The final conversion cell creates the `light_level_classifier.tflite` file.
