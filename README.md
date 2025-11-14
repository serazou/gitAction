# AWS IP Lookup Application

## How to Run

1. **Create virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application:**
   ```bash
   python src/use.py <IP_ADDRESS>
   ```
   
   Example:
   ```bash
   python src/use.py 52.95.110.1
   ```

## DevOps Tasks

* Clonez ce repo et créez un repo privé avec son code (changez le remote et push).
* Définir un workflow GitHub Actions pour
  * Build l'application (pip) avec Python 3.9
  * Lint avec Flake8
  * Tests avec nose (nosetests)
* Définir un workflow CodeBuild 
* Faire un buildspec équivalent et créer un build dans CodeBuild
* Enrichir ce workflow pour générer un rapport JUnit avec nosetests et le stocker dans CodeBuild
