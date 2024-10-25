# Flutter Bottom Navigation Bar Example

This is a simple Flutter app demonstrating the use of a bottom navigation bar with the `google_nav_bar` package. The app has a customizable bottom navigation bar with four tabs: Home, Likes, Search, and Settings.

## Features

- **Four navigation tabs**: Home, Likes, Search, and Settings.
- **Active and inactive states** for tabs, with customizable colors.
- **Customizable tab background colors** using `Container`.
- **On tab change event** to handle tab selection changes.

## Preview
<img src="https://github.com/user-attachments/assets/5fbb95cb-fb26-42de-9c7b-ee18a76f2b3d" alt="First Screenshot" style="width: 200px; height: auto;">

## Code Snippet

Below is the code snippet for the bottom navigation bar implementation:

```dart
bottomNavigationBar: Container(
  color: Colors.black,
  child: Padding(
    padding: const EdgeInsets.symmetric(
        horizontal: 15.0,
        vertical: 20
    ),
    child: GNav(
      onTabChange: (index) {
        print(index);
      },
      color: Colors.white,
      activeColor: Colors.white,
      tabBackgroundColor: Colors.grey.shade800,
      padding: const EdgeInsets.all(12.0),
      gap: 8, // Gap between icon and text
      tabs: const [
        GButton(icon: Icons.home, text: 'Home'),
        GButton(icon: Icons.favorite_border, text: 'Likes'),
        GButton(icon: Icons.search, text: 'Search'),
        GButton(icon: Icons.settings, text: 'Settings'),
      ]
    ),
  ),
),
```

## Dependencies

- `google_nav_bar`: [Google Nav Bar package on pub.dev](https://pub.dev/packages/google_nav_bar)

## Contact

For questions or feedback, please contact [@Bhavyansh03-tech](https://github.com/Bhavyansh03-tech) on GitHub or connect with me on [LinkedIn](https://www.linkedin.com/in/bhavyansh03/).

---
