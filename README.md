# 💰 Expense Management System

A full-stack financial tracking application featuring a dynamic **Streamlit** user interface and a high-performance **FastAPI** backend service.

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **Backend:** FastAPI (Uvicorn)
* **Database:** MySQL
* **Testing:** pytest
* **IDE / Environment:** PyCharm

## ✨ Key Features

- **Bulk Expense Entry:** Add multiple new expenses simultaneously through a streamlined data entry grid.
- **Dynamic Categorical Visualization:** View filtered financial records automatically compiled into interactive categorical bar charts.
- **Monthly Expense Analytics:** Track, filter, and break down spending trends month-over-month to analyze historical financial behaviors.
- **Robust API Backend:** Fully decoupled FastAPI service managing relational data constraints, database persistence, and payload validation.

## 📁 Project Structure

- **`frontend/`**: Contains the Streamlit user interface and application view logic.
- **`backend/`**: Contains the FastAPI server architecture and API routing.
- **`tests/`**: Contains unit and integration test suites for checking system stability.
- **`requirements.txt`**: Declares required third-party Python dependencies.
- **`README.md`**: Project documentation and infrastructure setup overview.

## 🚀 Getting Started & Setup

Follow these instructions to configure and run the application locally on your machine.

### Prerequisites

1. Ensure **Python 3.8+** is installed on your local operating system.
2. Ensure you have a running instance of **MySQL Server**. Create an empty database schema dedicated to this project before executing the backend server.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd expense-management-system
   ```

2. **Open with PyCharm:**
   * Open PyCharm and select **Open** to import the cloned project directory.
   * PyCharm will automatically detect the `requirements.txt` file and prompt you to create a virtual environment (`.venv`).
   * Confirm the setup to allow PyCharm to build the environment and install the dependencies automatically.

3. **Manual Dependency Fallback (Optional):**
   * If you prefer setting up the dependencies manually via the command line, run:
     ```bash
     pip install -r requirements.txt
     ```

### Running the Application

To start the system, you must run both the backend server and the frontend client simultaneously. 

1. **Start the FastAPI Backend:**
   Open a terminal window inside the root directory and run:
   ```bash
   uvicorn server.server:app --reload
   ```
   *The backend documentation will be accessible natively at `http://127.0.0`.*

2. **Start the Streamlit Frontend:**
   Open a second terminal window or use PyCharm's built-in terminal and run:
   ```bash
   streamlit run frontend/app.py
   ```
   *The frontend dashboard will automatically launch in your default web browser.*

## 🧪 Testing

The codebase relies on `pytest` for managing the continuous integration suites inside the `tests/` folder.

To run the complete test suite, execute the following command from the project root:
```bash
pytest
```
