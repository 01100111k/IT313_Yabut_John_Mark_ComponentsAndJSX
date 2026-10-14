# IT313 Laboratory 4 - React Components & JSX

## Student Roster Card Renderer

This project is a simple Expo React Native application for the IT313 Laboratory 4 activity. It demonstrates component-based architecture and JSX by displaying a list of enrolled students as reusable student cards.

## Problem

The IT313 registrar provided a list of currently enrolled students. The application displays each student using a reusable `StudentCard` component.

Each student card shows:

- Student name
- Course
- Units enrolled
- Full Load label when applicable

The application also displays the total number of students using a value computed from the students array.

## Component Structure

### StudentCard

`StudentCard` is a functional component that receives the following props:

- `name`
- `course`
- `units`
- `isFullLoad`

The props are destructured in the function signature and displayed using JSX.

The `Full Load` label is conditionally displayed using:

```jsx
{isFullLoad && <Text>Full Load</Text>}