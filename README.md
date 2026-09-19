# AI-Powered Digital Twin Platform for Personalized and Predictive Learning Analytics

## Overview

The AI-Powered Digital Twin Platform is a web-based learning analytics prototype that represents a student's learning state through a digital twin. It combines learning mastery, cognitive indicators, learning history, concept dependencies, risk metrics, study activity, and performance projections into a single interactive interface.

The platform is designed to show how a digital representation of a learner can be used to understand current learning performance, identify concept-level weaknesses, provide personalized study guidance, explore what-if learning scenarios, and present model explanations.

The current prototype uses the learner profile and learning data defined in the project files. The data is synthetic and is stored locally in JavaScript for demonstration of the platform interface and its analytics behaviour.

## What the Platform Contains

### Digital Twin Dashboard

The dashboard provides an overall view of the learner's current learning state. It includes overall mastery, learning streak, focus score, learning hours, twin version and twin accuracy.

It also contains a knowledge graph showing concept relationships and mastery levels, a cognitive profile, a forgetting curve, and a subject-concept mastery view.

The knowledge graph currently contains concepts including Algebra, Functions, Trigonometry, Limits, Derivatives, Integration, Statistics, Probability, Matrices, Vectors, Complex Numbers and Differential Equations.

### Predictions and Early Warning

The prediction view presents current performance together with projected performance under two situations: without intervention and with AI intervention.

It also displays learning-risk indicators for exam failure, dropout, cognitive burnout and frustration.

Concept-level warnings identify concepts that require attention and show their associated risk level, timeframe, identified issue and suggested action.

### Personalized Study Planner

The study planner displays a weekly schedule from Monday to Sunday.

The current schedule contains learning sessions for topics such as Limits, Derivatives, Waves, Probability, Integration, Matrices, Python Arrays, Trigonometry, Complex Numbers, Vectors, a Calculus mock test, mistake review, weak-concept revision and CS projects.

Each session contains a time, duration, topic, subject, session type and priority.

### Adaptive Quiz Engine

The quiz engine presents five questions during a quiz session.

Questions are selected with priority given to the currently weak areas of Derivatives, Limits and Integration, while other questions are also included.

The prototype supports answer selection, answer checking, skipping, explanations, scoring, quiz progress and starting a new quiz session.

### AI Tutor

The platform includes an AI Tutor interface named Ava.

The tutor is connected to the learner information represented in the digital twin and provides predefined responses based on the user's message. It also provides suggested questions related to integration, derivatives, calculus performance, study planning and retention.

The current implementation is a frontend prototype. Tutor responses are defined in the local project data rather than being generated through a live external AI API.

### Learning Simulation

The simulation view provides a what-if analysis interface.

The learner can adjust:

- Study time
- Focus
- Spacing
- Priority

The platform uses these inputs in the simulation formula and updates the projected score and learning trajectory.

It also provides predefined scenarios:

- Minimal Effort
- Current Pace
- Optimal Plan
- Intensive Mode

The simulation displays a projected four-week trajectory and compares it with the without-change trajectory.

### Explainable AI

The explainability view shows the factors used to explain the displayed learning-risk result.

The current prototype includes:

- Derivatives mastery
- Integration mastery
- Limits mastery
- Study streak
- Average session duration

It also displays a knowledge-tracing style chart showing the progression of selected concepts across eight weeks.

The interface includes model information displayed by the prototype, including the model name, reported accuracy and data description.

### Teacher and Parent Dashboard

The teacher view displays information for eight students in Grade 11A.

Each student card contains overall mastery, fail risk, burnout level, learning trend and alert information.

## Technology Used

The prototype is implemented as a client-side web application using:

- HTML5 for the application structure
- CSS3 for styling and responsive interface design
- JavaScript for application logic and interactive behaviour
- Chart.js for data visualizations
- Canvas API for the knowledge graph
- Local JavaScript data objects for the prototype learning data

Chart.js is loaded through its CDN in the current implementation.

## Project Structure

```text
Stu/
|
|-- index.html
|
|-- css/
|   |-- style.css
|
|-- js/
    |-- app.js
    |-- data.js
```

### File Responsibilities

`index.html`

Contains the complete interface structure and the different platform views.

`css/style.css`

Contains the visual styling, layout, cards, navigation, charts, tables and responsive interface rules.

`js/data.js`

Contains the learner profile, knowledge graph data, cognitive profile, forgetting curve, predictions, risk metrics, concept warnings, study plan, quiz questions, tutor suggestions and responses, explainability data and teacher dashboard data.

`js/app.js`

Contains the application logic, navigation, chart initialization, knowledge graph rendering, quiz behaviour, tutor interaction, simulation calculations, explainability visualizations, teacher dashboard rendering and digital-twin update behaviour.

## How the Prototype Works

The application starts from the Digital Twin Dashboard and loads the locally defined learner data.

The JavaScript application uses this data to render the different analytics views. When a user changes views, the corresponding charts and interactive components are initialized.

The knowledge graph represents relationships between learning concepts. Mastery values are visualized for individual concepts, while the cognitive profile and forgetting curve provide additional views of the learner's state.

The prediction section uses the predefined prediction data to visualize performance trajectories and learning risks.

The study planner renders the predefined weekly learning schedule.

The quiz engine selects questions from the local question bank, giving priority to weak topics.

The learning simulation calculates a projected final score from study time, focus, spacing and priority inputs and updates the displayed trajectory.

The prototype also contains a small live-update behaviour that slightly changes knowledge-node mastery values at regular intervals to simulate an updating digital twin.

## Running the Project

No backend server is required for the current prototype.

Clone or download the repository and open:

```text
Stu/index.html
```

in a modern web browser.

Because Chart.js is loaded from a CDN, an internet connection is required when the page loads the chart library.

## Data and Prototype Scope

The current implementation uses synthetic, locally defined learning data for the prototype.

The repository does not contain a backend database, model-training pipeline, authentication system, external AI API integration or real student data.

The AI, prediction, risk, explainability and simulation components shown in the interface are implemented through the data and JavaScript logic included in the current prototype.

## Project Objective

The objective of the platform is to demonstrate a digital-twin approach to personalized and predictive learning analytics, where a learner's knowledge state and learning indicators can be represented, monitored, analyzed and used to support personalized learning decisions.

## Current Prototype

The prototype brings the following components together in one interface:

Digital Twin Dashboard, Predictions and Early Warning, Personalized Study Planner, Adaptive Quiz Engine, AI Tutor, Learning Simulation, Explainable AI, and Teacher and Parent Dashboard.

This repository contains the current working frontend implementation of the platform.
