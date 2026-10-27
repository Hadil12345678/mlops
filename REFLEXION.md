
## Lab 3 — MLflow

### 1. Which model is the best? Can you prove it?

MLflow allows us to compare experiment runs using their F1 scores. Trial-1 and trial-3 have the same F1 score, while trial-2 performs worse. Trial-3 is preferable because it achieves the same performance without the salary feature.

### 2. Can you give back exactly the model of Trial 1?

Yes. MLflow saves each trained model with its run. We can reload a specific model using its run ID and `mlflow.sklearn.load_model()`.

### 3. Can a classmate reproduce your work on another machine?

Partly. Git preserves the code, and MLflow records parameters and metrics. However, differences in software versions and environments can prevent perfectly identical reproduction.
