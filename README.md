# End-to-End Machine Learning Project

## Setup Instructions

### Prerequisites
- Python 3.8+ (detected 3.13.0)

### 1. Create Virtual Environment (Windows PowerShell)
```
python -m venv venv
```

### 2. Allow PowerShell Scripts (one-time, if needed)
Run as Administrator PowerShell:
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### 3. Activate Environment
```
.\venv\Scripts\Activate.ps1
```
Prompt changes to `(venv)`.

### 4. Install Project & Dependencies
```
pip install -e .
```

### Run Pipelines
```
# Train
python src/pipeline/train_pipeline.py

# Predict (example)
python src/pipeline/predict_pipeline.py
```

### Deactivate
```
deactivate
```

## Project Structure
- `src/components/`: Data ingestion, transformation, model trainer.
- `src/pipeline/`: Train & predict pipelines.
- Logs via `src/logger.py`.

Venv created at `./venv` (Python 3.13). Conda not needed; pip/setup.py used. Deps (numpy, pandas, seaborn) installed globally, but use venv for isolation.
