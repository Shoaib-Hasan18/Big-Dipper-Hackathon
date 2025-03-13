# Big-Dipper-Hackathon
# 🚀 One-Day Hackathon Tasks

## Overview
These tasks are designed to be completed in a single day and will introduce our new engineers to our monorepo structure, API services, and key technologies. Each task is scoped appropriately for the hackathon timeframe while providing valuable learning experiences.

---

## 👨‍💻 Frontend Engineer Tasks

### 1️⃣ Property Image Gallery Viewer
**Description:** Create a responsive image gallery component that fetches and displays property images from our Finn.no integration API.

**Implementation Details:**
- Use the `/finn/{property_id_nma}/listings/images` endpoint
- Create a carousel/gallery component to display the images
- Implement error states and loading indicators
- Add hover effects to show image descriptions

**Benefits:**
- Introduces the new frontend engineer to our API integration patterns
- Provides experience with UI component development
- Limited scope, achievable in one day

### 2️⃣ Property Valuation Dashboard Widget
**Description:** Develop a dashboard widget that displays property valuation data from multiple sources in a visually appealing way.

**Implementation Details:**
- Use the `/units/{unit_id}/index-valuation` and `/units/{unit_id}/propcloud-estimate` endpoints
- Create a widget showing valuation data with:
    - Price comparison between different valuation methods
    - Confidence ranges visualization
    - Price per square meter metrics
- Style according to our design system

**Benefits:**
- Works with multiple API endpoints
- Introduces data visualization concepts
- Provides experience with our styling approach

### 3️⃣ Property Search Map Layer
**Description:** Add a new layer to our ArcGIS map showing property boundary data.

**Implementation Details:**
- Use the `/properties/boundaries` endpoint to fetch GeoJSON data
- Create a new map layer using ArcGIS JavaScript API
- Add interactivity to display property details on hover/click
- Implement a toggle to show/hide the layer

**Benefits:**
- Experience with our map integration
- Introduction to ArcGIS SDK
- Practical GeoJSON implementation

---

## 👨‍💻 Backend Engineer Tasks

### 1️⃣ Batch Processing Performance Enhancement
**Description:** Optimize one of our batch processing endpoints to improve response time and reduce server load.

**Implementation Details:**
- Focus on optimizing the `/units/comparables/batch` endpoint
- Implement request validation to catch errors early
- Add caching for frequently requested comparable properties
- Implement parallel processing of batch requests
- Add performance metrics logging

**Benefits:**
- Hands-on experience with our API architecture
- Exposure to performance optimization techniques
- Meaningful impact with a contained scope

### 2️⃣ New GraphQL Resolver for Property Timeline
**Description:** Create a new GraphQL resolver that combines transaction timeline data with listing images.

**Implementation Details:**
- Use the existing `/finn/transactions/timeline` REST endpoint
- Create a new GraphQL resolver that:
    - Fetches transaction history
    - For each transaction with a `FINN_CODE`, fetches the corresponding images
    - Returns a combined response with transaction data and images
- Add appropriate error handling and caching

**Benefits:**
- Introduction to our GraphQL implementation
- Experience with multiple API integrations
- Practical resolver pattern implementation

### 3️⃣ Property Score Analytics Module
**Description:** Develop a simple analytics module that combines municipality and area scores.

**Implementation Details:**
- Use the `/score/municipality/{property_id_nma}` and `/score/area/{property_id_nma}` endpoints
- Create a new endpoint that:
    - Fetches both scores
    - Calculates a combined score with weighted values
    - Returns a comprehensive evaluation with recommendations
- Add basic unit tests

**Benefits:**
- Exposure to our scoring systems
- Experience with creating new business logic
- Practical testing implementation

---

## 🛠️ Additional Resources

### Frontend Resources
- ArcGIS JavaScript API Documentation
- React Component Library
- Design System Guidelines
- API Endpoint Documentation (see attached Swagger)

### Backend Resources
- API Architecture Documentation
- GraphQL Schema
- Data Models Reference
- Testing Framework Documentation

---

## 🏁 Expected Deliverables

### For Each Task
- Working code implementation
- Basic documentation of approach
- Brief demo presentation (2-3 minutes)
- List of challenges encountered

### Notes
- Focus on functionality over perfect implementation
- It's okay to use placeholder data if API integration proves difficult
- Ask for help early if you get stuck
- Remember this is a learning experience - have fun with it!