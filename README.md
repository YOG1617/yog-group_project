Student Stress Analyzer (C Project)
 *Overview

The Student Stress Analyzer is a console-based application developed in C that evaluates a student’s stress level based on daily habits, academic pressure, and career-related concerns. The program interacts with users through a structured questionnaire and provides personalized feedback along with a dynamically generated study timetable.

This project focuses on combining basic programming concepts with a real-world problem—student stress management—to create a simple decision-support tool.

* Objectives
To analyze student stress factors such as study hours, sleep, and external pressure
To provide personalized suggestions for improving productivity and mental balance
To generate a customized timetable based on user preferences
To demonstrate structured programming and logic building in C
 Features
1.  Interactive Questionnaire

The program asks users a set of questions related to:

Study hours
Sleep duration
Source of pressure (self, parents, peers, teachers)
2. Stream-Based Analysis

*Different streams have different stress factors, so the program includes separate modules for:

JEE/NEET Aspirants (Science) – Rank anxiety, exam pressure
UPSC Aspirants – Attempt limits, vast syllabus
Commerce/CAT Aspirants – Percentile and competition stress
Humanities Students – Career uncertainty and societal pressure
3. Personalized Analysis Report

Based on user responses, the program:

Identifies key stress indicators
Provides specific suggestions for improvement
Highlights issues like low sleep or high pressure
4.  Dynamic Timetable Generator

The timetable adapts based on:

Preferred study time (morning/night)
Focus area (strong vs weak subjects)
Selected academic stream

It also adjusts recommendations if poor sleep habits are detected.

* Technical Implementation
 Programming Language
C (Standard I/O library)
 Core Concepts Used
Functions (modular design)
Conditional statements (if-else, switch-case)
Global variables
User input handling (scanf)
Structured program flow
 Functional Decomposition

The program is divided into multiple functions:

common() → collects general data
science(), upsc(), commerce(), humanities() → stream-specific inputs
analysis() → generates stress report
timetable() → creates personalized schedule
 *Program Flow
User selects their academic stream
Common questions are asked
Stream-specific questions are presented
Stress analysis report is generated
Personalized timetable is displayed
*Advantages
Simple and easy-to-use interface
Modular and readable code structure
Real-world application of programming logic
Personalized output enhances user engagement
* Limitations
No input validation (invalid inputs may cause incorrect behavior)
Uses basic rule-based logic (no advanced analytics)
Relies on global variables (less scalable design)
Console-based UI (no graphical interface)
* Future Enhancements
Implement input validation for robustness
Introduce a scoring system to classify stress levels (Low/Medium/High)
Store user data and generate reports using file handling
Improve UI with colors or transition to a GUI-based application
Integrate data analytics or machine learning for smarter insights
* Conclusion

The Student Stress Analyzer demonstrates how fundamental programming concepts can be applied to solve real-life problems. While simple in implementation, it provides meaningful insights and serves as a strong foundation for building more advanced, user-friendly mental wellness tools in the future.                                                                                                                                                                                                                                                                                                                                                                                 * Test cases 5
Test Case 1 – High Stress (JEE Aspirant)

Input:

Stream: 1
Study: 4
Sleep: 1
Pressure: 2
Rank: 1
Future: 1
Preference: 1
Focus: 2

Expected Output:

Long study hours warning
Low sleep warning
Parental pressure detected
Rank anxiety present
One-exam mindset warning
Timetable with weak subject focus
 Test Case 2 – Balanced Student (UPSC)

Input:

Stream: 2
Study: 2
Sleep: 3
Pressure: 1
Attempt: 3
Syllabus: 3
Preference: 2
Focus: 1

Expected Output:

Study manageable
Sleep adequate
No major stress detected
Balanced timetable
No strong warnings
 Test Case 3 – Moderate Stress (Commerce/CAT)

Input:

Stream: 3
Study: 3
Sleep: 2
Pressure: 3
Percentile: 2
Competition: 2
Preference: 1
Focus: 2

Expected Output:

High study hours note
Low sleep warning
Peer pressure detected
Percentile stress
Competition pressure
Weak area focused timetable
Test Case 4 – Humanities Pressure Case

Input:

Stream: 4
Study: 2
Sleep: 3
Pressure: 4
CareerFear: 1
SocietyPressure: 1
Preference: 2
Focus: 1

Expected Output:

Normal study/sleep
Career uncertainty stress
Social validation pressure
Advice on skills and passion
Balanced timetable
 Test Case 5 – Invalid Input Case

Input:

Stream: 5

Expected Output:

"Invalid choice" message
