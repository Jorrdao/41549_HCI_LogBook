<!-- 
This markdown document will contain all information and decisions concerning the HCI project for
< The Title of the Project Here >
Work carried out by:

-->
# *HCI Project Logbook*

**Title of the project**: YRU Running
**Team:**
- Student 1: [José Jordão   103075] 
- Student 2; [Rodrigo Lopes 113811]


---
# [A. Stage 0 - Planning and Problem Identification](stage0_planning/a_stage_0_planning_problem_identification.md)
 Running is a fast-growing sport, with more people taking it up for fitness, competition, and social engagement. However, while there are several platforms dedicated to tracking runs and connecting runners, there is a significant gap when it comes to race registration and community engagement focused on official events.

One of the biggest frustrations for runners is the process of signing up for races. Currently, each race has its own website and registration system, forcing runners to search for events individually and go through separate sign-up processes for each one. This fragmentation makes it inconvenient to discover new races, compare options, and keep track of upcoming events.

With this in mind, the YRU Running project aims to bridge the gap by creating a social network for runners that not only allows users to track their runs and connect with other athletes but also simplifies race registration in a unified platform. This will benefit both runners and race organizers—runners will have a seamless experience when signing up for races and finding training partners, while organizers will have a better way to promote their events and reach a larger audience.

By combining race registration, training logs, and social interaction, YRU Running will provide a more complete and engaging experience for runners, making it easier to stay motivated, connected, and prepared for upcoming races.


# [B. Stage 1 - Context Definition](stage1_context/b_stage_1_context_definition.md)

## Competitor analysis
We identified three main competitors that serve different aspects of the running community:

1. **Strava** – The leading social network for runners, offering performance tracking, route sharing, and community engagement. However, it lacks direct race registration      features.
2. **Garmin Connect** – A platform focused on in-depth performance analytics, mainly used by runners with Garmin devices. While it provides comprehensive training insights, it is not designed for discovering or signing up for races.
3. **Portugal Running** – A local website dedicated to listing and managing race sign-ups in Portugal. While it provides centralized race registration, it lacks the social and tracking features present in other platforms.

## Heuristic Evaluation & Cognitive Walkthrough

To assess the usability and effectiveness of Strava’s user experience, we conducted two evaluations:

1. **Cognitive Walkthrough** – Testing how new users interact with the registration process.
2. **Heuristic Evaluation** – Analyzing Strava’s interface using  usability heuristics to identify key usability issues.

### Cognitive Walkthrough

To evaluate the ease of use and potential usability issues in Strava’s account registration process. Three participants (Rafael, Rodrigo, and Guilherme) performed the task and rated each step.

- **Step 1: Finding the Sign-Up Option** – Rated 4/5 by all participants, indicating that the sign-up button was easy to locate.
- **Step 2: Choosing a Sign-Up Method** – Rated between 4 and 5, meaning the process was intuitive.
- **Step 3: Filling Personal Information & Submitting** – Scores ranged from 3 to 5, with some users experiencing a lack of confirmation after account creation

### Heuristic Evaluation

To analyze specific UI problems based on Jakob Nielsen’s usability heuristics. Participants rated each issue’s severity from 0 (no issue) to 4 (major issue).

![alt text](<Screenshot from 2025-03-10 22-42-17.png>)

The Cognitive Walkthrough confirmed that Strava’s registration process is mostly intuitive but lacks a clear confirmation message after account creation. The Heuristic Evaluation highlighted usability problems related to unclear system feedback, race enrollment difficulties, and complex terminology.

## User Feedback & Insights

To ensure that YRU Running meets the needs of different types of runners, we conducted user interviews to gather insights about their expectations and pain points. The feedback collected validated the need for a platform that goes beyond simple run tracking, integrating personalization, race management, and community-driven features.

Based on the interviews, we identified distinct needs between inexperienced runners and experienced runners, as well as common expectations shared by both groups.

**Inexperienced Runners**
- Interested in detailed post-run data, including distance, time, and pace, to track progress.
- Would like to have a personalized training plan based on their performance to guide improvement.
- Appreciate a runner matchmaking system that suggests training partners with similar performance levels.
- Motivated by a gamification system with XP points and trophies to encourage consistency.

**Experienced Runners**
- Want an integrated race registration system to avoid searching and signing up on different websites.
- Would like to see a map of highlights showing the best moments from their training and races.

The user research phase confirmed that YRU Running should not be limited to activity tracking, but should also provide race discovery, training guidance, social engagement, and competition management. The feedback gathered will guide the next development stages, ensuring that the platform aligns with real user needs and offers a complete running experience for both casual and competitive runners.
 
# [C. Stage 2 - Requirement Analysis](stage2_requirements/c_stage_2_requirement_definition.md)
To build an effective and user-centered platform, it is essential to define the key requirements of YRU Running. 
This phase focuses on understanding user needs, defining system functionalities, and selecting appropriate tools for development. 
Through structured analysis, we aim to ensure that the platform meets the expectations of runners, race organizers, and the broader running community.
In this stage we covered:
1. **Personas**, creating representative user profiles based on real world insights to understand different types of users and their needs.
2. **Scenarios**, where we defined typical use cases to illustrate how users will interact with our platform.
3. **Requirements**, where we identified functional and non-functional requirements  to guide the platform's development.
4. **Developments Tools**, where we selected the technologies we saw fit for our project.

## Personas

### 1. Helena

**Profile**
- 42 years old
- Accountant
- Former Track and filed athlete
- Runs over 50km a week

**Motivation**

Ana is a dedicated and experienced runner who maintains a high weekly mileage. She actively participates in races but struggles to find the best options that fit her preferences. Currently, **she must browse multiple websites to compare races, often finding it difficult** to determine which events offer the best experience or value for money.

She wants a **centralized platform** that allows her to easily find and register for races based on her own criteria—such as location, distance, price, and race difficulty. Instead of spending time researching various races manually, she would prefer personalized recommendations that align with her training goals and budget.

### 2. Vitor

**Profile**
- 27 years old
- Human Resources specialist at Decathlon
- Former football player in his youth
- New to running

**Motivation**
Miguel has recently decided to take up running to improve his fitness after spending long hours at the office. However, as a beginner, **he feels overwhelmed by many existing running apps that focus heavily on advanced stats and complex performance metrics**. He wants a simple and intuitive platform that helps him ease into running without unnecessary complications.

He is looking for a **user-friendly experience** where he can track his progress without being bombarded with data. He also wants a way to find beginner-friendly races that match his current level, helping him stay motivated and gradually improve.


## Scenarios

### Helena signs up for a race
As soon as Helena opens the site, she is greeted with the login form, allowing her to quickly access her account. Once logged in, she is taken directly to the main feed, where she can explore posts from other runners. Without hesitation, she navigates to the Races page and clicks on New Race to begin the registration process. Browsing through the available options, she selects her desired competition and proceeds to fill out the sign-up form, ensuring all necessary details are entered. With just a few clicks, she successfully registers for her next race, ready to take on the challenge ahead.

### Vitor creates his account
Vítor opens the site and is immediately directed to the login page. Instead of logging in, he clicks on Register, which takes him to the registration page. There, he fills out the form with his name, age, height, weight, email, and password. He also selects his running level—Beginner, Intermediate, or Advanced. After successfully completing the form, he is redirected back to the login page, ready to access his new account.

### Vitor logs his first run
Vítor opens the platform and is immediately taken to the login page. After successfully logging in, he navigates to the Run section and clicks Start to begin his run. Once finished, he returns to the platform and clicks Stop to end the session. Upon doing so, the platform congratulates him on completing his first run and redirects him to a preview of his activity, where he has the option to post it.

## Requirements

### Functional
- [P1] Sign Up Page - User should be able to create and account
- [P1] Log in Page - User should be able to log in tho his account
- [P1] Profile Page - User should be able to see his profile page with his informations
- [P1] Race Page - User should be able to sign up for a race
- [P2] Log Run - User should be able to enter a run
- [P2] Map of official races - Interactive map that filter races
- [P2] Feed page - main page with posts
- [P3] In deepth Statistics - statistics such as how many runs, km one user had and his average times
- [P3] Search users - User should be able to search a user and see his profile
- [P4] Reward system - User should be able to level up and earn rewards with xp earned in runs 
- [P5] Interact with posts - user should be able to interact with other users
 
### Non-functional
- Simple and Intuitive UI 
- Minimalist Data Presentation
- Mobile-First Design
- Secure Authentication
- Data Protection & GDPR Compliance

## Developing Tools and Technology

To develop YRU Running, we chose a modern and scalable technology stack that ensures performance, usability, and efficient collaboration.
- **Front-End: React.js** – A component-based library that enables a responsive and mobile-friendly user interface with fast rendering.
- **Back-End: FastAPI** – A high-performance Python framework that provides asynchronous processing, built-in validation, and automatic API documentation for seamless integration of user authentication, race management, and tracking.
- **Version Control & Collaboration: GitHub** – Manages project tasks through pull requests, issue tracking, and CI/CD support, ensuring a structured and efficient development workflow.

This technology stack allows YRU Running to be fast, scalable, and user-friendly, providing an optimal experience for both beginner and experienced runners while maintaining an agile and maintainable development process.

---
# [P1 - First Assignment Presentation](presentation_1/p1_first_assignment_presentation.md)
>	Presentations will take place in weeks 5 and 6
---

# [D. Stage 3 - Low-Fidelity Prototype and Evaluation](stage3_low_fidelity/d_stage_3_low-fidelity_prototype_and_evaluation.md)
>	The low-fidelity prototype stage spans weeks 7 and 8. Based on the scenarios and requirements a low fidelity prototype is designed and evaluated adopting a formative evaluation approach




# [E. Stage 4 - Functional Prototype and Evaluation](stage4_functional_prototype/e_stage_4_functional_prototype_and_evaluation.md)
>	Weeks 9, 10, and 11. During this stage, and incorporating the feedback from the evaluation performed in stage D, a functional prototype is developed and evaluated.




# [F. Stage 5 - Discussion and Solution Refinement](stage5_discussion_and_refinement/f_stage_5_reporting_discussion_refinement.md)
>	Week 12. Stage 5 concerns gathering all the data from the evaluation, discuss the findings, perform some refinement to the functional prototype and, if needed, additional evaluation.



# [G. Stage 6 - Critical Analysis](stage6_critical_analysis/g_stage_6_critical_analysis.md)
>	This should be done before the presentation and entails a critical analysis over the whole work that was performed, what were the strong points and what could have been done better.




---
# [P2 - Second Assignment Presentation](presentation_2/p2__second_assignment_presentation.md)
>	Final Presentations of the project will take place in weeks 13 and 14


