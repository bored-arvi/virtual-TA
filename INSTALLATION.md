# Installation Guide for Virtual TA

This guide explains how to set up the **Virtual TA** project on your local machine or server.

## 1. Prerequisites
- **Python 3.8+** (Check with `python --version` or `py --version`)
- **pip** (Comes with Python 3.8+)
- **Git** (Optional, for cloning the repository)
- **Docker** (Optional, for containerized setup)

## 2. Clone the Repository
```bash
git clone https://github.com/your-username/virtual-TA.git
cd virtual-TA
```

## 3. Create a Virtual Environment
**Windows (CMD):**
```bash
python -m venv venv
venv\Scripts\activate
```
**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

## 4. Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## 5. Run the Application
```bash
python main.py
```

## 6. Docker Setup (Optional)
### Build the Docker Image
```bash
docker build -t virtual-ta .
```
### Run the Container
```bash
docker run -it --rm virtual-ta
```

## 7. Environment Variables & Secrets
- Store sensitive keys in a `.env` file:
```env
API_KEY=your_api_key_here
```
- Install python-dotenv:
```bash
pip install python-dotenv
```

## 8. Troubleshooting
- **venv activation error on Windows (PowerShell)**:
```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```
- **Permission errors**: Run terminal as Administrator (Windows) or use `sudo` (Linux/macOS).

## 9. Next Steps
- Check out the [README.md](README.md) for usage details.
- Explore the `course_md/` folder for example content.
- Contribute improvements via pull requests.
