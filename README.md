# Automatic Faculty Timetable Generator

This project is a web-based application for **automatic timetable generation** for faculty members. It allows you to upload faculty and subject details, add theory and lab subjects, and generates a weekly timetable with faculty mapping. The application also includes a login page for secure access.

## Features

- **Login Page** for secure access (`index.html`)
- **Add Theory and Lab Subjects** with weekly hours
- **Upload Faculty Details** via Excel file
- **Automatic Timetable Generation** for 6 days and 7 periods per day
- **Lab periods are always continuous** and start at 1st or 5th period
- **Theory periods are never consecutive** and are randomly distributed
- **Faculty have classes every day** (if hours permit), and not at the same period each day
- **Faculty Mapping Table** shows subject, faculty, type, and periods allocated
- **Download Timetable** as Excel or CSV
- **Responsive and clean UI** using Bootstrap and custom CSS

## How to Use

1. **Login**
   - Open `index.html` in your browser.
   - Use the demo credentials:  
     **Username:** `admin`  
     **Password:** `admin123`

2. **Add Faculty and Subjects**
   - Enter theory faculty, subject, and hours, then click "Add Faculty".
   - Enter lab faculty, subject, and lab hours, then click "Add Lab".
   - Or, upload an Excel file with columns: `Faculty Name`, `Subject`, `Hours/Week`.

3. **Generate Timetable**
   - Click "Generate Timetable" to create the timetable.
   - The timetable will display for 6 days and 7 periods per day, with breaks after 2nd and 4th periods.

4. **Download**
   - Download the timetable and faculty mapping as an Excel file or CSV.

## File Structure

- `index.html` — Login page
- `main.html` — Main timetable generator page
- `style.css` — Custom styles for both pages
- `README.md` — This file

## Requirements

- Modern web browser (Chrome, Edge, Firefox, etc.)
- No server required (runs locally)
- [Bootstrap 5](https://getbootstrap.com/) and [SheetJS (xlsx)](https://sheetjs.com/) are loaded via CDN

## Sample Excel Format

| Faculty Name   | Subject         | Hours/Week |
|----------------|-----------------|------------|
| Dr. A. Kumar   | Mathematics     | 5          |
| Ms. B. Singh   | Physics         | 4          |
| Mr. C. Rao     | Chemistry Lab   | 3          |

## Notes

- Lab hours are always scheduled as continuous periods, starting at the 1st or 5th period.
- Theory subjects are never scheduled in consecutive periods or at the same period each day.
- The faculty mapping table shows only those who are assigned periods in the timetable.

## Contact

For doubts (saranramesh709@gmail.com)
