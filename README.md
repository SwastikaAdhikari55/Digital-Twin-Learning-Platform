# TwinLearn - AI-Powered Digital Twin Learning Platform

TwinLearn is an AI-powered Digital Twin learning platform prototype developed for an ML hackathon. The platform represents a student's learning state through a Digital Twin and provides personalized learning analytics, performance predictions, adaptive learning support, and teacher-level monitoring.

The current prototype demonstrates the complete user-facing workflow through an interactive web interface.

## Project Overview

TwinLearn creates a digital representation of a student's learning profile using information such as concept mastery, cognitive indicators, study behaviour, learning progress, and risk metrics.

The prototype is designed around a student named Arjun Sharma and demonstrates how the Digital Twin can be used to:

- monitor overall learning mastery
- visualize relationships between learning concepts
- track cognitive indicators
- show memory retention and forgetting behaviour
- predict future performance
- identify at-risk concepts
- generate a personalized study schedule
- provide adaptive quiz questions
- provide a Twin-aware AI Tutor interface
- simulate the effect of changes in study behaviour
- explain prediction factors
- provide a teacher-level view of multiple students

## Main Modules

### Digital Twin Dashboard

The dashboard presents the student's current learning state, including overall mastery, study streak, focus score, learning hours, knowledge graph, cognitive profile, memory retention curve, and concept mastery.

### Predictions and Early Warning

This section presents predicted performance trajectories and risk indicators. The prototype includes exam failure risk, dropout risk, burnout risk, and frustration index.

It also provides an at-risk concept forecast containing the concept, subject, risk level, risk score, timeframe, root issue, and recommended action.

### Personalized Study Planner

The study planner provides a weekly schedule with study time, topic, activity type, priority, and subject. It also displays the daily goal, today's progress, study streak, and predicted exam score associated with the plan.

### Adaptive Quiz Engine

The quiz module selects questions around the learning concepts represented in the Digital Twin. The prototype includes questions from topics such as derivatives, limits, integration, trigonometry, matrices, and probability.

After an answer is processed, the interface updates the quiz state and represents a Digital Twin confidence or mastery update.

### AI Tutor

The AI Tutor interface is designed around the student's Digital Twin profile and provides personalized learning suggestions such as explaining concepts, understanding score changes, improving retention, and creating a study plan.

### Learning Simulation

The simulation provides a What-If interface where study variables can be adjusted and the projected exam score is updated.

The available controls in the prototype are:

- Daily Study Time
- Focus Level
- Spaced Repetition Adherence
- Calculus Priority Weight

The prototype displays a four-week score projection comparing the current trajectory with the simulated plan.

### Explainable AI

The Explainable AI section shows the factors represented as influencing the exam failure risk prediction. It also provides a feature-importance visualization, model information, other predictions, and knowledge-tracing trends.

### Teacher View

The teacher view provides a class-level overview for Grade 11A and displays student-level information including mastery, failure risk, burnout, trend, and alerts.

## Machine Learning and Analytics Concepts Represented

The prototype represents the following ML and learning-analytics concepts:

- Digital Twin based learning representation
- Knowledge Tracing
- Performance prediction
- Risk prediction
- Adaptive learning
- Personalized study planning
- Spaced repetition
- Cognitive profiling
- Explainable AI
- What-If simulation
- Concept dependency analysis
- Learning analytics dashboards

The prototype displays a model information section identifying the approach as a GradBoost + KT Ensemble and shows the model accuracy and training-data figures used in the interface.

## Technology Used

The provided prototype is a web-based frontend built with:

- HTML5
- CSS3
- JavaScript
- Chart.js

Chart.js is loaded through a CDN in the prototype.

## Project Structure

```text
TwinLearn/
|
├── index.html
├── css/
│   └── style.css
└── js/
    ├── app.js
    └── data.js
```

## How to Run the Prototype

No Python environment or package installation is required for the current prototype.

1. Download or clone this repository.
2. Open the `TwinLearn` folder.
3. Open `index.html` in a modern web browser.
4. Navigate through the available sections using the sidebar.

Because Chart.js and the Google Fonts used by the interface are loaded from external CDNs, an internet connection may be required for all visual elements to load correctly.

## Data in the Current Prototype

The current prototype uses the data defined in `js/data.js`. The student profiles, mastery values, predictions, risk metrics, quiz questions, study schedules, and other displayed values are part of the prototype data.

The repository does not contain a separate machine learning training dataset or a backend training pipeline in the supplied prototype.

## Hackathon Prototype Scope

This repository represents the working prototype submitted as part of an ML hackathon project. Its purpose is to demonstrate the proposed Digital Twin learning analytics experience and the interaction between learning-state representation, prediction, personalization, simulation, explainability, and teacher monitoring.

The README describes only functionality present in the supplied prototype and does not assume additional backend services, datasets, APIs, or model-training pipelines that are not included in this repository.

## Future Development

Future implementation details should be added only when they are actually developed and included in the project repository.

