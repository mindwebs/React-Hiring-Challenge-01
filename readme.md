# React Hiring Challenge

## Table of Contents
- [Introduction](#introduction)
- [Technical Requirements](#technical-requirements)
  - [Dashboard Interface](#dashboard-interface)
  - [Control Panel](#control-panel)
  - [Data Point based Visualisation Algorithm](#data-point-based-visualisation-algorithm)
  - [Technical Pointers](#technical-pointers)
  - [Bonus](#bonus)
- [Submission](#submission)
- [Evaluation Criteria](#evaluation-criteria)
  - [Functionality](#functionality)
  - [Design](#design)
  - [Code Quality](#code-quality)
  - [Algorithms](#algorithms)
  - [Testing](#testing)

## Introduction

You are tasked with building an interactive dashboard for spatial visualization, focusing on locational or geometric data. This dashboard will display coordinates and perform various algorithmic operations to visualize results.

## Technical Requirements

### Dashboard Interface

- Design an intuitive dashboard layout with a main screen showcasing a map that visualizes data points based on geographical location.
- Implement a component-based design, utilizing separate React components for the map, data point tooltip, and control panel.
- Ensure the interface is responsive for both mobile and desktop views.

### Control Panel

- Place the control panel on the side or top of the dashboard.
- Include the following features:
  - Filter data points by "date range" and "value range."
  - An "Add" button to facilitate bulk addition of data points, opening a modal for inputting geo-coordinates, category, date, and value.
  - A dynamic table format for adding data points, including coordinate-x, coordinate-y, date, value, latitude, longitude, and date in dd-mm-yyyy format.
  - 
    | Coordinate-X | Coordinate-Y | Date        | Value          |
    |--------------|--------------|-------------|----------------|
    | Latitude     | Longitude    | DD-MM-YYYY  | Number (0->100)|

  - Optional: Provide an option to toggle between different visualization modes (e.g., heat-maps, clusters, individual points).

### Data Point based Visualisation Algorithm

- Visualize a route starting from any point with the lowest value as the origin, traversing through each point and returning to the origin.
- Display this path/route on the map using lines and provide the total perimeter (length) and area of the curve/polygon created by these points.
- Implement calculations using the distance formula of 2D coordinate geometry.
- Optionally, explore heuristic methods like the nearest neighbor algorithm or more advanced methods.
- Dynamically display and update the length and area of the curve.

### Technical Pointers

- Utilize TypeScript for type safety.
- Integrate state management (e.g., Redux or Zustand) to manage the application state.
- Ensure code modularity and comprehensive code comments for improved readability.

### Bonus

- Implement a "Time Travel" feature, allowing users to move back and forth in time to observe data point evolution.
- Include a time range slider for selecting points based on the provided range, with dynamic updates to calculations and the map's polygon.
- Use an external API to pull real-world data or enhance visualization (e.g., real-time weather).

## Submission

- Share the GitHub repository containing your code.
- Optionally, deploy the application to a hosting platform of your choice (e.g., Vercel, Netlify).
- Include a README in the codebase with:
  - Setup and installation instructions.
  - A brief summary of the algorithms used.
  - Challenges faced and how they were overcome.
  - Any improvements or features you'd like to add in the future.

## Evaluation Criteria

Candidates will be evaluated based on the following criteria:

### Functionality

Does the application work without errors?

### Design

How user-friendly, responsive, and creative is the interface?

### Code Quality

Is the code modular, readable, and well-documented?

### Algorithms

Are the algorithms correctly implemented and efficient?

### Testing

Are there meaningful tests, and do they cover key functionality?
