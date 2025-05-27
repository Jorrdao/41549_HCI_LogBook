[Back to main Logbook Page](../hci_logbook.md)

---

# E. Functional Prototype and Evaluation

# Prototype
This high-fidelity prototype simulates the core interface and functionality of the YRU Running platform. It was developed using **React**, prioritizing user experience and clean, modern UI elements.

## Feed Page

The Feed Page is designed to simulate a **social running dashboard** that encourages motivation through community engagement and personal goal tracking.

### Main Features:
- **Friend Activity Feed**: Displays recent activities by friends, including:
  - Distance
  - Average pace
  - Total time
  - Mini map preview
- **Weekly Leaderboard**:
  - Ranks users by: distance, moving time, elevation gain
- **Weekly Goals Tracker**:
  - Visual progress towards user-defined goals (e.g., 50 km/week)
- **Suggested Routes**:
  - Personalized recommendations for running paths
  - Information shown: name, surface, distance, elevation, difficulty

### Design Elements:
- Scrollable sections with horizontal and vertical layouts
- Cards with icons and data highlights
- Motivational color scheme and clear layout


## Race Page

The Race Page helps users explore and discover global running events in an engaging and interactive way.

### Main Features:
- **3D Interactive Globe**:
  - Clickable pins showing upcoming races worldwide
  - Basic race information popup
- **Race List View**:
  - Scrollable list with race name, date, location, type (e.g., Marathon, 10k)
- **Filter Options**:
  - By location, date, distance, difficulty, race type
- **Registration Management** *(planned)*:
  - Placeholder for future race registration system

### Design Elements:
- Interactive globe (Three.js or similar)
- Clean race cards
- Responsive UI with search and filter tools

# E.X. User Evaluation

To evaluate our prototype, we conducted usability testing with three different users. The goal was to gather both quantitative and qualitative feedback on the interface, overall usability, and clarity of user flows.

We used two main evaluation methods:

1. **System Usability Scale (SUS) Questionnaire**  
   After interacting with the prototype, each user was asked to complete a SUS questionnaire. This provided us with a standardized score reflecting the overall usability of the system. The SUS helped us quantify user satisfaction and identify broader usability issues.

2. **Standard Usability Testing Form**  
   During the testing sessions, we also observed users completing predefined tasks such as:
   - Visit and follow a profile
   - Edit profile (stats and description)
   - Register for an official race

   We recorded any visible hesitations or misunderstandings. Users were also encouraged to think aloud while interacting with the prototype, which gave us deeper insights into their expectations and pain points.

Overall, the feedback was very useful. Users found the interface intuitive, especially the "Race" and "Feed" pages. However, a few users pointed out that certain icons and buttons could be more prominent, which helped us refine the layout in the next iteration.

The combination of quantitative SUS scores and observational usability testing allowed us to make data-informed improvements and better align the final product with user needs.


---
[Back to main Logbook Page](../hci_logbook.md)

---
