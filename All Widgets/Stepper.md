```dart
// Stepper Widget
// Use the Stepper widget to create a stepper with a list of steps.

Stepper(
  // List<Step> steps: The list of steps for the stepper.
  steps: [
    Step(
      // Widget title: The title of the step, displayed at the top of the step.
      title: Text('Step 1'),
      // Widget? subtitle: The subtitle of the step, displayed below the title.
      subtitle: Text('Step 1 subtitle'),
      // Widget content: The content of the step, displayed below the subtitle.
      content: Text('Step 1 content'),
      // bool isActive: Whether the step is active or not.
      isActive: true,
    ),
    Step(
      title: Text('Step 2'),
      subtitle: Text('Step 2 subtitle'),
      content: Text('Step 2 content'),
      isActive: true,
    ),
    Step(
      title: Text('Step 3'),
      subtitle: Text('Step 3 subtitle'),
      content: Text('Step 3 content'),
      isActive: true,
    ),
  ],
  // StepperType type: The type of stepper, either vertical or horizontal.
  type: StepperType.vertical,
  // int currentStep: The index of the current active step.
  currentStep: 0,
  // void Function(int)? onStepTapped: Callback when a step is tapped.
  onStepTapped: (step) {
    // Handle step tap
  },
  // void Function()? onStepContinue: Callback when the continue button is tapped.
  onStepContinue: () {
    // Handle continue tap
  },
  // void Function()? onStepCancel: Callback when the cancel button is tapped.
  onStepCancel: () {
    // Handle cancel tap
  },
)

```

### Properties
- `steps`: The list of steps for the stepper.
- `type`: The type of stepper, either vertical or horizontal.
- `currentStep`: The index of the current active step.
- `onStepTapped`: Callback when a step is tapped.
- `onStepContinue`: Callback when the continue button is tapped.
- `onStepCancel`: Callback when the cancel button is tapped.

### Explanation
- The `Stepper` widget creates a stepper with a list of steps.
- Each step consists of a title, subtitle, content, and an optional state icon.
- The stepper can be either vertical or horizontal, specified by the `type` property.
- The `currentStep` property determines the active step.
- Callbacks like `onStepTapped`, `onStepContinue`, and `onStepCancel` handle user interactions.
  
### Tips
- Use the `Stepper` widget to guide users through a series of steps in a process.
- Customize the appearance of each step using the `Step` widget's properties.
- Handle user interactions like tapping a step or continuing/canceling the process with appropriate callbacks.
