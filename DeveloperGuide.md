3. docs/DeveloperGuide.md

# Developer Guide – Mitomba eSales

##  Tech Stack
- **Frontend**: HTML, CSS, JavaScript (React optional)
- **Backend**: Django + REST Framework
- **Database**: PostgreSQL
- **Payments**: M-Pesa or MTN MoMo APIs

##  Local Setup
```bash
git clone https://github.com/yourusername/mitomba-esales.git
cd mitomba-esales
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

 Folder Structure

/mitomba-esales
  ├── api/         # Backend APIs
  ├── frontend/    # Static files or React
  ├── media/       # Uploaded images
  ├── templates/   # HTML templates

 Environment Variables

API_KEY=<your-payment-api-key>
DEBUG=True
DATABASE_URL=...

Contributing

Fork repo

Create new branch

Submit PR

