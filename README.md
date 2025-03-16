# LinkedIn Easy Apply Bot

An automated bot to apply for jobs on LinkedIn using the "Easy Apply" feature. This bot is customized to support:

## Features
- Multiple job positions and locations
- Experience level filtering
- Resume and Cover Letter uploads
- Automatic form filling
- Job application tracking
- Blacklist support for companies and job titles

## Configuration
1. Create a `config.yaml` file with your LinkedIn credentials and job preferences:
```yaml
username: your_email@example.com
password: your_password
phone_number: your_phone_number

positions:
  - "Position 1"
  - "Position 2"

locations:
  - "Location 1"
  - "Location 2"

experience_level:
  - 1  # Entry level
  - 2  # Associate
  - 3  # Mid-Senior level

uploads:
  Resume: "/path/to/your/resume.pdf"
  Cover Letter: "/path/to/your/cover_letter.pdf"

output_filename:
  - "output.csv"
```

2. Place your resume and cover letter in the `Application` directory

## Installation
1. Clone the repository
2. Create a virtual environment:
```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
1. Activate the virtual environment:
```bash
source env/bin/activate  # On Windows: env\Scripts\activate
```

2. Run the bot:
```bash
python easyapplybot.py
```

## Notes
- The bot will automatically handle LinkedIn's Easy Apply process
- Job application results are saved in `output.csv`
- Questions and answers are stored in `qa.csv`
- The bot uses smart delays to avoid detection

## Contributing
Feel free to submit issues and enhancement requests!
