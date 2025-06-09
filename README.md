# WeSplit - SwiftUI Bill Splitter App

WeSplit is a simple yet interactive SwiftUI application that helps users split a bill among multiple people, calculate the tip, and determine how much each person owes. It also lets users choose their favorite dish and rate the service quality, making it a practical and fun dining companion app.

 ## Features

**Bill Input**: Enter the total check amount with a native currency formatter.
**People Picker**: Choose the number of people (from 2 to 99) to split the bill.
**Dish Selector**: Select your favorite dish from a predefined list.
**Service Rating**: Rate the service from 1 to 5 stars.
**Tip Selection**: Choose a tip percentage (0%, 10%, 15%, 20%, 25%) using a segmented picker.
**Live Calculations**:
  - Total with Tip
  - Amount per Person
**User Experience**
  - Keyboard dismiss button for better input handling
  - Red warning color if no tip is selected

 How It Works

The app calculates the total tip and then divides the full amount among the selected number of people. The total and per-person amounts are dynamically updated as the user changes inputs.
 Formulas Used

- **Total with Tip**:
Note: `numberOfPeople` is stored as an offset, so it starts from 2.

## 🧩 Components

### `ContentView.swift`

The main interface, structured using SwiftUI `Form` and `Section` components. It uses:

- `@State` for managing user inputs
- `@FocusState` for managing keyboard focus
- `NavigationStack` for structured navigation

### `RatingView.swift`

A reusable component to visually rate the service using tappable stars.

- Uses `@Binding` to sync with parent view
- Customizable star images and colors
- Accessible and styled with `.plain` button style

## 🔧 Requirements

- Xcode 15+
- iOS 17+
- SwiftUI

## 🧪 Preview

Includes `#Preview` and `RatingView_Previews` for SwiftUI canvas rendering during development.

## 📝 Author

Created as a first SwiftUI application project to learn state management, layout, and user interaction in Swift.



