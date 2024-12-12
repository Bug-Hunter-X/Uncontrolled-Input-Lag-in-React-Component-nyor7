# React Uncontrolled Input Bug

This repository demonstrates a subtle bug in React related to uncontrolled inputs and state updates.  The `inputValue` state is updated, but this doesn't directly re-render the input element, resulting in a lag between what the user types and what is displayed.

## Bug Description
An uncontrolled input's value is directly bound to the component's state. When the state is updated, the display value might not reflect this immediately. This leads to a temporary discrepancy between the actual input value and its visual representation.

## Solution
The solution involves using a controlled input where the input's value is managed entirely by the component's state.  The state update now directly controls the input element's value, ensuring immediate visual feedback.