# Software Engineering Lab File
**Topic:** Pradhan Mantri Internship Scheme (PMIS) Recommendation System

### 1. Problem Statement

**Background**
The Pradhan Mantri Internship Scheme is a major initiative by the Government of India designed to connect youth aged 21 to 24 with internship opportunities across top Indian companies. It was launched in 2024 with a very ambitious goal of providing 1 crore internships over five years. The scheme offers financial support, including a monthly stipend of 5,000 rupees, a one time assistance of 6,000 rupees, and insurance coverage.

While the centralized portal allows companies to post openings and students to apply, there is a big challenge when it comes to matching the right candidate with the right role. Many students register but struggle to find internships that fit their specific academic background, skills, or location preferences. This leads to low selection rates and empty internship seats. At the same time, companies find it difficult to filter through thousands of applications to find suitable candidates. The main issue is a lack of intelligent, personalized matching.

**Descriptive Problem**
The current PMIS portal is missing a smart recommendation layer. Right now, it cannot analyze a candidate's full profile like their education, skills, and interests to suggest the most relevant opportunities. It relies on basic keyword searches instead of ranking internships based on how well they actually fit the student. This is especially hard for first time applicants from rural areas who might not know how to search effectively. It also lacks a way to predict a candidate's chances of selection or help companies automatically shortlist the best applicants. Because of this, deserving students miss out, and companies are overwhelmed with irrelevant applications.

**Expected Solution**
To solve this, we need an AI powered Recommendation System built into the PMIS portal. This system should be able to collect applicant data and intelligently match them to internships using advanced filtering techniques. It needs to create a personalized feed of recommended internships for every student, showing them exactly why a particular role is a good fit. It should also provide companies with a ranked list of the best candidates for their postings, while supporting multiple languages to be accessible to everyone across India.

### 2. Proposed Solution

The solution we are proposing is the Pradhan Mantri Internship Scheme Recommendation System. This is an intelligent web platform that adds a smart recommendation engine to the existing PMIS ecosystem.

**System Architecture**
The system is built on a standard three tier architecture. The Presentation Layer is a responsive web interface that works on both browsers and mobile devices. The Application Layer contains the core logic, including the recommendation engine, profile analyzer, and API connections. Finally, the Data Layer manages the databases for user profiles, internship listings, and the machine learning models.

**Recommendation Strategy**
The core of the system is a Hybrid Recommendation Engine. It uses Content Based Filtering to match what an internship requires with what an applicant has on their profile. It also uses Collaborative Filtering, which looks at what similar candidates have successfully applied for in the past to suggest new opportunities. To make things easier for students, the system includes a resume parser that automatically extracts their skills and education details when they upload a document, and it actively encourages them to complete their profiles to get better recommendations.

### 3. Key Components

The system relies on several important modules to function effectively:

1. User Profile Module: Manages student data, academic details, and handles resume parsing.
2. Internship Listings Module: Allows companies to post and manage their internship openings.
3. Recommendation Engine: The AI core that generates the personalized, ranked suggestions.
4. Fit Score Calculator: Calculates a percentage match between a student and a specific internship.
5. Explainability Module: Gives a simple reason why an internship was recommended, like "Matches your skills in Python and preferred location in Delhi."
6. Candidate Shortlisting Module: Provides companies with AI ranked lists of applicants.
7. Notification System: Alerts students about new matches and application deadlines.
8. Admin Dashboard: Gives government officials a high level view of scheme statistics.
9. Multilingual Interface: Ensures the portal can be used in Hindi and other regional languages.
10. Analytics Module: Tracks placement success rates and system performance.

### 4. Users

The platform is designed for four main types of users:

**Applicants (Students)**
These are the primary users, typically youth aged 21 to 24 who have completed their schooling or graduation. Their main goal is to find good internships, apply easily, and track their progress.

**Company Representatives**
These are HR professionals or recruiters from participating companies. They use the system to post new internships and find the best candidates from the ranked lists provided by the AI.

**Government Administrators**
Officials managing the scheme use the portal to monitor overall success, view analytics, and make sure everything is running smoothly.

**System Administrators**
The technical team that keeps the servers running, updates the machine learning models, and ensures all user data is secure.

### 5. Functionalities

The system has two types of functionalities: Functional Requirements and Non Functional Requirements. Both are organized by priority below.

**Functional Requirements**
These are the core features the system must have to work properly.

| Priority | Requirement | Description |
|---|---|---|
| High | User Registration | Students must be able to easily register, create profiles, and upload resumes for automatic skill extraction. |
| High | Smart Recommendations | The system has to generate personalized, ranked internship recommendations and explain the fit score for each one. |
| High | Search and Apply | Students need search filters for location and stipend, and the ability to apply directly. |
| High | Company Portal | Companies must be able to post internships and instantly receive ranked applicant lists. |
| High | Alerts and Dashboard | The system needs to send timely alerts to students and provide a comprehensive dashboard for administrators. |
| Low | Language Support | Support for multiple regional languages to improve accessibility. |
| Low | AI Chatbot | A chatbot to guide first time users through the application process. |
| Low | Status Tracking | Allow students to track their application status in real time. |
| Low | Social Login | Log in using DigiLocker or Aadhaar. |
| Low | Bookmark Candidates | Allow companies to bookmark interesting candidates for later review. |
| Low | Feedback System | A feedback and rating system for completed internships. |

**Non Functional Requirements**
These outline how well the system performs, its security, and overall user experience.

| Priority | Requirement | Description |
|---|---|---|
| High | Performance | The system must be fast, returning recommendations in under 3 seconds even with thousands of users online. |
| High | Scalability | It needs to be highly scalable to handle up to 1 crore users over five years and maintain 99.5 percent uptime. |
| High | Security and Privacy | Security is critical, requiring strong encryption and strict compliance with India's Digital Personal Data Protection Act. |
| High | AI Accuracy | The artificial intelligence recommendations need to be highly accurate and relevant to the user. |
| Low | Usability | The platform should be very user friendly, achieving high scores in usability testing. |
| Low | Accessibility | It must be accessible to users with disabilities following WCAG standards. |
| Low | Device Compatibility | It needs to work perfectly on all modern browsers and mobile phones. |
| Low | Maintainability | The code must be well documented so updates can be made quickly, and all administrative actions should be logged for security audits. |

### 6. Summary

The PMIS Recommendation System is designed to solve the matching problem between India's youth and participating companies. By using smart AI recommendations, automatic resume reading, and a clear, user friendly portal, the system makes it much easier for students to discover internships that truly fit their skills. This intelligent approach will significantly improve placement rates and help the Pradhan Mantri Internship Scheme reach its full potential.
