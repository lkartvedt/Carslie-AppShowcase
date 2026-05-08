# Carslie-AppShowcase
This is the public showcase for my iOS app Carslie

**[Download on the App Store](https://apps.apple.com/app/carslie/id123456789)** | **[Visit Website](https://yourwebsite.com)**

![App Preview](Screenshots/app-preview.png)

Carslie is a native iOS application for vehicle asset management designed for individuals and families who own one or more vehicles to track maintenance, documents, and reminders in one place. Your glovebox just got an upgrade!

**Key Capabilities:**
- Multi-vehicle management with photo support
- VIN and license plate decoding via auto.dev API
- AI-powered Q&A for vehicle-specific information
- Reorderable garage with SwiftData persistence
- Full light/dark mode and accessibility support

---

## Technical Stack

### Language & Platform
- Swift 5.9+
- iOS 17.0+ target
- 100% SwiftUI interface

### Apple Frameworks
- **SwiftUI** - Declarative UI with modern lifecycle
- **SwiftData** - Local persistence layer for vehicle models
- **PhotosUI** - Photo library integration
- **Foundation** - URLSession networking, JSON parsing

### Architecture
- MVVM pattern with service layer abstraction
- Async/await concurrency model
- Protocol-based API service design
- Type-safe JSON decoding with Codable

### API Integration
- RESTful integration with auto.dev vehicle database
- VIN decoding endpoint
- License plate lookup with state-based routing
- Error handling with localized user feedback

### Data Layer
- SwiftData models with relationship support
- Binary image storage within model objects
- JSON specification storage for flexible schema
- Ordered collection management

---

## Features

**Vehicle Management**
- Add vehicles via VIN or license plate with automatic data population
- Store comprehensive specs (engine, transmission, MPG, tire size, oil type)
- Custom naming with intelligent defaults (Color + Make + Model)
- Photo library integration for vehicle images
- Drag-to-reorder and swipe-to-delete gestures

**AI Chat Interface**
- Vehicle-specific conversational assistant
- Keyword-based intelligent response system
- Persistent chat history per vehicle
- Suggested questions with tap-to-send
- Contextual awareness of vehicle specifications

**Design & UX**
- Glass morphism visual effects with material backgrounds
- Blue-to-purple gradient accent system
- Adaptive layouts for different screen sizes
- Empty states with clear CTAs
- Loading indicators and error states

**Accessibility**
- VoiceOver support with semantic labels
- Dynamic Type scaling
- High contrast visual elements
- Keyboard navigation compatibility

---

## Technical Highlights

**SwiftData Implementation**
- Model-driven persistence with `@Model` macro
- Embedded binary data for images
- JSON string storage for flexible specification data
- Ordered relationships via custom sorting

**API Service Pattern**
- Protocol-based service design for testability
- Centralized error handling with custom error types
- Async/await networking with structured concurrency
- Response validation and transformation

**State Management**
- SwiftUI environment objects for data flow
- @Query macro for reactive data binding
- Local state management with @State and @Binding
- Navigation via NavigationStack and value-based routing

**UI/UX Engineering**
- Custom view modifiers for reusable styling
- Compositional layouts with adaptive sizing
- Gesture recognizers for interactive elements
- Animation timing functions for polish

---

## Data Flow

**Vehicle Creation:**
1. User inputs VIN or license plate + state
2. Service layer makes API request to auto.dev
3. Response parsed and mapped to Vehicle model
4. User customizes name and adds photo
5. SwiftData persists to local database

**AI Chat:**
1. User submits question about their vehicle
2. Service analyzes question for keywords (oil, tire, MPG, etc.)
3. Matches keywords against vehicle specs JSON
4. Generates contextual response
5. Appends to conversation history

---

## Technical Requirements

- iOS 17.0 or later
- Xcode 15.0 or later
- Active internet connection for vehicle lookup
- Photo library permissions for image selection

---

## Notes

This is a closed-source production application. The repository serves as a technical showcase and is not available for cloning or contributions. All code is proprietary.

For inquiries about the technical implementation or to discuss my work, please reach out via:
- **LinkedIn**: [Lindsey Kartvedt]([https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/lindsey-kartvedt-24ba46102/))
- **Email**: lindseykartvedt[AT]gmail[DOT]com

Love my work? [Buy me a coffee](https://buymeacoffee.com/lkartvedt)

---

**[Download Carslie on the App Store](https://apps.apple.com/app/carslie/id123456789)**


