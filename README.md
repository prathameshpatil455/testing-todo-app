# Test Plan for Footer Component

## Overview

The Footer component is responsible for rendering information about active todos, navigation links, and providing functionality to clear completed todos. The test plan includes various test cases to ensure the correct rendering and behavior of the Footer component.

## Test Cases

### Test Case 1: Rendering Footer Component

- **Type of Test:** Integration Test
- **Objective:** Ensure that the Footer component is rendered correctly with the necessary elements.
- **Steps:**
  1. Render the Footer component with a set of sample todos.
  2. Check if the component is present in the DOM.
  3. Verify the presence of the count of active todos and navigation links.

### Test Case 2: Disabled "Clear Completed" Button

- **Type of Test:** Unit Test
- **Objective:** Confirm that the "Clear completed" button is disabled when all todos are active (not completed).
- **Steps:**
  1. Render the Footer component with a set of active todos.
  2. Check if the "Clear completed" button is disabled.

### Test Case 3: Enabled "Clear Completed" Button

- **Type of Test:** Unit Test
- **Objective:** Verify that the "Clear completed" button is enabled when there are completed todos.
- **Steps:**
  1. Render the Footer component with a set of todos containing completed items.
  2. Check if the "Clear completed" button is enabled.


# Test Plan for Header Component

## Overview

The Header component is responsible for rendering the title and input field for adding new todos. The test plan includes various test cases to ensure the correct rendering and behavior of the Header component.

## Test Cases

### Test Case 1: Rendering Header Component

- **Type of Test:** Integration Test
- **Objective:** Ensure that the Header component is rendered correctly with the title and input field.
- **Steps:**
  1. Render the Header component.
  2. Check if the component includes the title "todos" and a text input field.

### Test Case 2: Dispatching Action on Adding New Item

- **Type of Test:** Unit Test
- **Objective:** Confirm that the dispatch function is called with the correct action when adding a new item.
- **Steps:**
  1. Render the Header component.
  2. Simulate adding a new item by changing the input value and pressing Enter.
  3. Verify if the dispatch function is called with the expected action and payload.


# Test Plan for Input Component

## Overview

The Input component is responsible for rendering an input field for adding new todos. The test plan includes various test cases to ensure the correct rendering and behavior of the Input component.

## Test Cases

### Test Case 1: Input Attributes and Values

- **Type of Test:** Unit Test
- **Objective:** Confirm that the input field has the correct attributes and values.
- **Steps:**
  1. Render the Input component with specified placeholder and label.
  2. Verify if the input field has the expected placeholder attribute value.
  3. Check if the label is associated with the input field.

### Test Case 2: Sanitizing and Submitting Input Value

- **Type of Test:** Unit Test
- **Objective:** Verify that the onSubmit function is called with the minValidLength and sanitized value when Enter key is pressed.
- **Steps:**
  1. Render the Input component with an onSubmit function.
  2. Simulate typing a value containing special characters.
  3. Press the Enter key and ensure that the onSubmit function is called with the minValidLength and sanitized value.


# Test Plan for Todo Item Component

## Overview

The Todo Item component is responsible for rendering individual todo items and handling interactions such as toggling completion. The test plan includes various test cases to ensure the correct rendering and behavior of the Todo Item component.

## Test Cases

### Test Case 1: Rendering Todo Item

- **Type of Test:** Integration Test
- **Objective:** Ensure that the Todo Item component is rendered correctly with the provided title.
- **Steps:**
  1. Render the Todo Item component with a sample todo.
  2. Check if the component is present in the DOM.
  3. Verify the presence of the todo item label, toggle checkbox, and action button.

### Test Case 2: Toggling Todo Completion

- **Type of Test:** Unit Test
- **Objective:** Confirm that the toggle function works correctly by dispatching the 'TOGGLE_ITEM' action.
- **Steps:**
  1. Render the Todo Item component with a sample todo.
  2. Simulate clicking the todo item's toggle checkbox.
  3. Verify if the dispatch function is called with the expected action and payload.

### Test Case 3: Rendering Different Todo Example

- **Type of Test:** Integration Test
- **Objective:** Ensure that the Todo Item component renders correctly for different todo examples.
- **Steps:**
  1. Render the Todo Item component with a different sample todo.
  2. Check if the component is present in the DOM.
  3. Verify the presence of the todo item label and toggle checkbox.



# Test Plan for Main Component

## Overview

The Main component is responsible for rendering the main content of the todo application, including the list of todos. The test plan includes a test case to ensure the correct rendering and structure of the Main component.

## Test Cases

### Test Case 1: Rendering Main Component

- **Type of Test:** Integration Test
- **Objective:** Ensure that the Main component is rendered with the correct structure.
- **Steps:**
  1. Render the Main component with a set of sample todos.
  2. Check if the component is present in the DOM.
  3. Verify the presence of specific elements such as 'main', 'toggle-all', and 'todo-list'.





