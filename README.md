# F1 Driver Match Quiz

This project is a Streamlit-based F1 driver matching quiz.
The app is implemented as a Python project with separated modules for authentication, data loading, quiz logic, and UI rendering.

## Run

```bash
pip install -r requirements.txt
streamlit run app.py
```

`app.py` is the main execution file for grading.

## Assignment Notes

- First screen shows the student ID and name.
- Login is required before solving the quiz.
- Quiz JSON data is loaded with Streamlit caching via `@st.cache_data`.
- The quiz is multiple-choice and produces a score-based personality match result.

## Structure

- `app.py`: main Streamlit execution entrypoint
- `src/config.py`: project constants and paths
- `src/state.py`: session state initialization and reset
- `src/data.py`: cached JSON loading and asset helpers
- `src/logic.py`: score calculation and top-3 result logic
- `src/ui.py`: login, quiz, and result screen rendering
- `assets/`: image assets used by the app
- `requirements.txt`: Python dependencies

## Reproducibility

- The required package version is pinned in `requirements.txt`.
- `.gitignore` excludes Python cache files, virtual environments, editor folders, and Streamlit secrets.
