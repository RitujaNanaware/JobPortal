# JobBhartee.com - Smart Job Search and Recruitment System

## Overview
JobBhartee.com is a comprehensive job search and recruitment platform that connects job seekers with employers. The platform utilizes advanced features including resume parsing and intelligent job matching to streamline the recruitment process.

## Features

### For Job Providers (Companies)
- **User Registration**: Companies can register with details including company name, establishment year, HR information, headquarters, and company type.
- **Profile Management**: Update company details and HR information.
- **Job Posting**: Create and post job openings with details such as:
  - Job designation
  - Salary
  - Bond years
  - Eligible branches (IT, Mechanical, Civil, EEE, ECE, Chemical, CSE)
- **Candidate Management**: 
  - View applications for posted jobs
  - Filter candidates based on criteria
  - Send emails to selected candidates
- **Job Management**:
  - View all posted positions
  - Delete job vacancies

### For Job Seekers (Students)
- **User Registration**: Students can register with personal and academic details.
- **Profile Management**: Update personal information, academic records, and skills.
- **Job Search**: Browse available job openings.
- **Job Application**: Apply for jobs with a single click.
- **Application Tracking**: View status of applied jobs.
- **Profile Details**:
  - Personal information (name, contact, gender, etc.)
  - Academic records (CGPA, 10th/12th scores)
  - Skills and certifications
  - Statement of Purpose (SOP)
  - Internship experience

### For Administrators
- **User Management**: Manage both job providers and job seekers.
- **System Monitoring**: Oversee the platform's operations.
- **Content Moderation**: Ensure appropriate content on the platform.

## Technology Stack

### Frontend
- HTML5
- CSS3
- JavaScript
- Modern UI/UX design principles

### Backend
- Django (Python web framework)
- Natural Language Processing (NLP) for resume parsing
- RESTful API architecture

### Database
- SQLite (Development)
- Scalable database design

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd final_year_project
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run migrations:
```bash
cd trial/campus
python manage.py migrate
```

5. Create a superuser:
```bash
python manage.py createsuperuser
```

6. Start the development server:
```bash
python manage.py runserver
```

## Project Structure
```
final_year_project/
├── trial/
│   └── campus/
│       ├── crs/          # Course management app
│       ├── campus/       # Main project settings
│       │   ├── models.py # Database models
│       │   ├── views.py  # View functions
│       │   ├── forms.py  # Form definitions
│       │   └── urls.py   # URL routing
│       ├── manage.py     # Django management script
│       └── db.sqlite3    # Database file
├── README.md
└── requirements.txt
```

## Data Models

### Student Details (stu_details)
- Username
- Name
- Phone number
- Parents' names
- Gender
- Place
- Branch (IT, Mechanical, Civil, EEE, ECE, Chemical, CSE)
- Academic records (BTech CGPA, 10th CGPA, 12th percentage)
- Certifications count
- Internship status
- Languages
- Statement of Purpose (SOP)
- Date of birth
- Email

### Company Details (comp_details)
- Username
- Company name
- Establishment year
- HR name and contact
- Headquarters
- About company
- Company type (product/service)
- Email

### Job Positions (job_pos)
- Job ID
- Username
- Company name
- Designation
- Salary
- Bond years
- Branch eligibility (IT, Mechanical, Civil, EEE, ECE, Chemical, CSE)

### Applied Jobs (applied_jobs)
- Company ID
- Job ID
- Student ID

## Key Functionality

### Student Features
1. **Registration**: Create account with personal and academic details
2. **Login**: Secure authentication
3. **Profile Update**: Modify personal and academic information
4. **Job Search**: Browse available positions
5. **Job Application**: Apply for jobs with one click
6. **Application Tracking**: Monitor application status

### Company Features
1. **Registration**: Create company account with business details
2. **Login**: Secure authentication
3. **Profile Update**: Modify company information
4. **Job Posting**: Create and publish job openings
5. **Candidate Management**: View and filter applications
6. **Communication**: Send emails to selected candidates

## Contributing
1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License
[Add your license information here]

## Contact
[Add contact information here]

## Acknowledgments
- Django Framework
- [Add other acknowledgments]
