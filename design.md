# DYNLEARN – System Design Document

## 1. System Overview
DYNLEARN follows a modular architecture where each component operates independently while sharing user context. The system uses AI to analyze skill alignment and prioritize learning paths.

## 2. High-Level Architecture
- Frontend: Web-based interface for students.
- Backend: Handles application logic and processing.
- AI Layer: Performs skill analysis and prioritization.
- Database: Stores user profiles, skills, and analysis results.

## 3. Module Design

### Skill Input Module
- Accepts manual skill input.
- Supports resume upload for automatic skill extraction.
- Sends skill data to the AI layer.

### Role Analysis Module
- Maintains skill requirements for different job roles.
- Provides baseline data for comparison.

### Skill Gap Analyzer
- Compares student skills with role-specific requirements.
- Identifies missing or weak skills.

### Priority Engine
- Assigns priority levels to identified skill gaps.
- Determines recommended learning order.

### Output and Guidance Module
- Displays skill gap analysis results.
- Provides clear learning guidance.

## 4. AI Decision Flow
1. User provides skills manually or uploads a resume.
2. User selects a target job role.
3. AI extracts and normalizes skill data.
4. AI compares skills with role requirements.
5. Skill gaps are identified.
6. Priority levels are assigned.
7. Learning guidance is generated.

## 5. User Flow
Signup → Skill Input → Role Selection → AI Analysis → Skill Gap Report → Learning Guidance

## 6. Design Principles
- Learning-first approach
- Simplicity and clarity
- Productivity-focused guidance
- Ethical and responsible AI usage
