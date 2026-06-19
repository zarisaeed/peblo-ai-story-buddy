# Peblo AI Story Buddy

## Framework Chosen

I used HTML, Tailwind CSS, and JavaScript to build a lightweight interactive prototype. This approach allowed rapid development, smooth animations, and simple deployment.

## Audio to Quiz Transition

The application waits for story/audio completion before revealing the quiz state. This creates a clear learning flow and prevents users from answering before finishing the story.

## Data Driven Quiz

Quiz content is designed to be generated from question data objects rather than hardcoded UI. This allows different question counts and option counts without changing the rendering logic.

## Caching Approach

For local assets, browser caching is used automatically. If remote audio were used in production, it would be cached using browser cache/storage to avoid repeated downloads.

## Audio Loading and Failure States

Loading states should be shown while audio is being prepared. If loading fails, the user receives feedback and can retry instead of the application becoming unusable.

## Performance Profiling

The application uses lightweight HTML, Tailwind CSS, and minimal JavaScript. Performance was verified through browser rendering and interaction testing to ensure smooth transitions.

## Android Optimization

The interface uses lightweight assets, minimal dependencies, efficient rendering, and responsive layouts suitable for mid-range Android devices.

## AI Usage and Judgment

AI assistance was used for rapid prototyping, UI ideation, and code generation. Some generated suggestions were simplified to keep the application lightweight and easier to maintain.

## Files

- code.html
- DESIGN.md
- screen.png
