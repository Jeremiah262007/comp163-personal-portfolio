# ==========================================================
# Personal Academic & Life Portfolio
# Author: Jeremiah Cooper
# Description: This program stores and organizes academic,
# personal, and financial data using strings, lists, tuples,
# sets, and dictionaries. It also performs calculations
# for GPA, budgets, and more using the specified values.
# ==========================================================

# ===== 1. PERSONAL INFORMATION =====
full_name = "Jeremiah Cooper"
student_email = "jdcooper4@ncat.edu"
hometown = "Charlotte, NC"
graduation_semester = "Spring 2029"
major = "Computer Science"

# ===== 2. ACADEMIC DATA =====
current_courses = ["COMP 163", "MATH 131", "GEEN 111", "HIS 206"]
completed_courses = ["Chemistry", "AP Literature", "AP Calculus BC", "Spanish IV", "AP Government"]
credit_hours = [3, 3, 3, 3]
gpa_history = [3.8, 3.9, 3.7, 4.0]

# ===== 3. CONTACT INFORMATION =====
emergency_contact = ("Mom", "Felicia Cooper", "704-321-9876")
home_address = ("456 Oak Street", "Charlotte", "NC", 28202)
instagram_info = ("Instagram", "@whos.jeremiah", 427)
twitter_info = ("Twitter", "@Envy_J", 43)
birthday = ("Birthday", 8, 5, 2007)

# ===== 4. INTEREST TRACKING =====
current_skills = {"Python basics", "JAVA", "Critical thinking", "OpenSim", "Public speaking"}
skills_to_learn = {"CSS+", "HTML", "Git", "Cybersecurity", "Organization"}
career_interests = {"Software development", "Software engineer", "Machine learning engineer", "Cybersecurity"}
hobbies = {"Gaming", "Golfing", "Bowling", "Thrifting", "Music"}
entertainment_backlog = {"One Piece", "Breaking Bad", "Boondocks", "Regular Show", "Attack on Titan"}

# ===== 5. ORGANIZATIONAL MAPPING =====
course_credits = {
    "COMP 163": 3,
    "MATH 131": 3,
    "GEEN 111": 3,
    "HIS 206": 3
}

course_professors = {
    "COMP 163": "Prof. Rhodes",
    "MATH 131": "Dr. V",
    "GEEN 111": "Dr. Parrish",
    "HIS 206": "Prof. Beale"
}

course_rooms = {
    "COMP 163": "M-Eric 300",
    "MATH 131": "Marteena 201",
    "GEEN 111": "Crosby 121",
    "HIS 206": "Crosby 210"
}

monthly_budget = {
    "Food": 325,
    "Entertainment": 75,
    "Books": 60,
    "Transportation": 85
}

study_hours_per_subject = {
    "Programming": 11,
    "Math": 9,
    "Engineering": 2,
    "History": 5
}

contact_directory = {
    "Mom": "704-321-9876",
    "Tristin": "704-555-7777",
    "Mason Jones": "336-333-5555"
}

# ===== 6. REQUIRED CALCULATIONS =====
total_credits = sum(credit_hours)
cumulative_gpa = round(sum(gpa_history) / len(gpa_history), 2)
completed_courses_count = len(completed_courses)
total_study_hours = sum(study_hours_per_subject.values())
academic_load = total_credits + total_study_hours
monthly_budget_total = sum(monthly_budget.values())
daily_food_budget = round(monthly_budget["Food"] / 30, 2)
annual_budget = monthly_budget_total * 12
study_cost_per_hour = round(monthly_budget["Books"] / total_study_hours, 2)

# ===== 7. ANALYTICS CALCULATIONS =====
total_followers = instagram_info[2] + twitter_info[2]
skills_have = len(current_skills)
skills_want = len(skills_to_learn)
contact_count = len(contact_directory)
backlog_count = len(entertainment_backlog)
academic_workload = academic_load

# ===== FORMATTED OUTPUT =====
print("=" * 58)
print("              PERSONAL ACADEMIC & LIFE PORTFOLIO")
print("=" * 58)
print(f"Student: {full_name} | Email: {student_email}")
print(f"From: {hometown} | Graduating: {graduation_semester}")
print(f"Major: {major}")
print("=== ACADEMIC PROFILE ===")
print(f"Current Semester: {total_credits} credits across {len(current_courses)} courses")
print(f"Cumulative GPA: {cumulative_gpa}")
print(f"Weekly Study Time: {total_study_hours} hours")
print(f"Academic Investment: ${study_cost_per_hour} per study hour")
print("\nCurrent Courses:")
print(f"{current_courses[0]} - {course_credits['COMP 163']} credits - {course_professors['COMP 163']} - {course_rooms['COMP 163']}")
print(f"{current_courses[1]} - {course_credits['MATH 131']} credits - {course_professors['MATH 131']} - {course_rooms['MATH 131']}")
print(f"{current_courses[2]} - {course_credits['GEEN 111']} credits - {course_professors['GEEN 111']} - {course_rooms['GEEN 111']}")
print(f"{current_courses[3]} - {course_credits['HIS 206']} credits - {course_professors['HIS 206']} - {course_rooms['HIS 206']}")

