# EIE Placement Cell Management System

A complete, production-quality single-folder web application that runs entirely in the browser without requiring Node.js, npm, servers, databases, or any external installations.

## Features

### 🎓 Student Portal
- **Profile Management**: Update personal details, CGPA, and academic marks
- **Job Search**: View eligible job postings based on academic criteria
- **Application Tracking**: Apply for jobs and track application status
- **Placement Status**: View current placement status

### 👨‍🏫 Faculty Portal
- **Student Management**: View all student details and mark students as placed
- **Job Posting**: Create new job postings with eligibility criteria
- **Application Review**: Review job applications and update status
- **Placement Tracking**: Monitor student placement progress

### 📊 Placement Cell
- **Alumni Showcase**: View placed alumni with their experiences
- **Placement Reports**: Department-wise placement statistics
- **Visual Analytics**: Interactive charts showing placement and salary data
- **Company Statistics**: Track company-wise placement numbers

## Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Database**: IndexedDB for persistent browser storage
- **Authentication**: Web Crypto API for password hashing
- **Charts**: Canvas API for data visualization
- **Architecture**: Simulated REST API using JavaScript modules

## Quick Start

### Running the Application

1. **Download/Clone** the project folder
2. **Open** `index.html` in any modern web browser
3. **That's it!** No installation required.

### Default Login Credentials

#### Students
- **Email**: `john@student.com` | **Password**: `password123`
- **Email**: `jane@student.com` | **Password**: `password123`
- **Email**: `alice@student.com` | **Password**: `password123`

#### Faculty
- **Email**: `prof1@faculty.com` | **Password**: `faculty123`
- **Email**: `prof2@faculty.com` | **Password**: `faculty123`

## File Structure

```
EIE Placement Cell Management System/
├── index.html              # Homepage
├── role.html              # Role selection page
├── login.html             # Login/Signup page
├── student.html           # Student dashboard
├── faculty.html           # Faculty dashboard
├── placement.html         # Placement cell section
├── css/
│   └── styles.css         # All application styles
├── js/
│   ├── db.js             # IndexedDB database setup
│   ├── api.js            # Simulated REST API
│   ├── auth.js           # Authentication logic
│   ├── student.js        # Student dashboard logic
│   ├── faculty.js        # Faculty dashboard logic
│   └── placement.js      # Placement section logic
└── README.md             # This file
```

## Database Schema

### Students
- ID, Name, Email, Password (hashed), Roll Number
- CGPA, 10th Mark, 12th Mark
- Placement Status, Placed Company

### Faculty
- ID, Name, Email, Password (hashed)

### Jobs
- ID, Company, Role, Salary, Last Date
- Eligibility Criteria (CGPA, 10th, 12th marks)
- Description, Posted By, Posted Date

### Applications
- ID, Student ID, Job ID, Status, Applied Date

### Alumni
- ID, Name, Roll Number, Company, Role
- Salary, Graduation Year, Experience

## Key Features

### 🔐 Security
- Password hashing using Web Crypto API
- Session management with localStorage
- Role-based access control

### 💾 Data Persistence
- All data stored in browser's IndexedDB
- Automatic data seeding with dummy records
- Offline functionality

### 📱 Responsive Design
- Mobile-friendly interface
- Modern CSS Grid and Flexbox layouts
- Cross-browser compatibility

### 🎯 Smart Features
- **Auto-filtering**: Students only see eligible jobs
- **Real-time updates**: Application status changes reflect immediately
- **Data validation**: Form validation and error handling
- **Visual feedback**: Status badges and progress indicators

## Usage Guide

### For Students
1. Select "Student" role and login/signup
2. Update your profile with academic details
3. Browse available jobs (auto-filtered based on eligibility)
4. Apply for jobs and track application status

### For Faculty
1. Select "Faculty" role and login
2. View all student details and academic performance
3. Post new job opportunities with eligibility criteria
4. Review applications and update status
5. Mark students as placed when they get jobs

### For Visitors
1. Visit the Placement Cell section
2. View alumni placement success stories
3. Check department placement statistics
4. Analyze placement trends with interactive charts

## Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 11+
- ✅ Edge 79+

## Development Notes

### Simulated Backend
The application uses a sophisticated client-side architecture that simulates a full backend:

- **API Layer**: `js/api.js` provides REST-like endpoints
- **Database**: IndexedDB with proper indexing and relationships
- **Authentication**: Secure password hashing and session management
- **Data Validation**: Client-side validation with error handling

### Performance Optimizations
- Lazy loading of data
- Efficient IndexedDB queries with indexes
- Minimal DOM manipulation
- Optimized CSS with modern layout techniques

## Troubleshooting

### Common Issues

1. **Data not persisting**: Ensure browser allows IndexedDB storage
2. **Login issues**: Check browser console for errors
3. **Charts not displaying**: Ensure Canvas API is supported

### Browser Storage
The application uses approximately 1-2MB of browser storage for:
- Student and faculty data
- Job postings and applications
- Alumni records and placement statistics

## Future Enhancements

- Export data to CSV/PDF
- Email notifications (simulated)
- Advanced search and filtering
- Bulk operations for faculty
- Mobile app version

## License

This project is created for educational purposes and demonstration of modern web technologies.

---

**Note**: This is a demonstration application. In a production environment, you would use a real backend server, database, and proper security measures.