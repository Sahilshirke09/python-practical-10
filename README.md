# MCA Semester I - Practical 10: Unit Testing, Logging & Code Quality
**Course:** Python & Relational Programming  
**Student:** Sahil Surendra Shirke  

## Files Included
- `order.py` — Order processing module with discount, GST, and total calculation plus input validation
- `test_order.py` — Pytest unit test suite covering valid calculations, zero discount, and `ValueError` exceptions
- `logging_demo.py` — Order logger demonstrating `DEBUG`, `INFO`, `WARNING`, and `ERROR` levels
- `application.log` — Generated log output from `logging_demo.py`
- `bad_code.py` — Code quality sample linted and formatted using Ruff

## Testing vs. Logging vs. Formatting
- **Unit Testing (`pytest`):** Verifies functional correctness by checking that functions return expected values and raise proper exceptions for invalid inputs.
- **Logging (`logging`):** Records runtime events, warnings, and errors to `application.log` to trace execution and troubleshoot issues after deployment.
- **Linting & Formatting (`ruff`):** Enforces consistent code style and catches static issues (such as unused imports or variables) without executing the program.

## macOS Setup & Execution
    python3 -m venv .venv
    source .venv/bin/activate
    python -m pip install pytest ruff
    python -m pytest -v
    python logging_demo.py
    cat application.log
    python -m ruff check bad_code.py
    python -m ruff format bad_code.py
