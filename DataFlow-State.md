# Data flow using @State

With UIKit, it’s up to you to update your UI when data changes. For example, whenever you add a new movie to Fave Flicks, you want it to appear in the list of movies on the main screen. Ensuring this happens isn’t difficult, but it’s easy to forget something when your app grows with new features. In addition to keeping the UI data up to date, you might need to show a loading spinner while the view loads. If the movie list is empty, you can show a message to prompt the user to add something. If there’s an error, you can hide everything else and show an error message. You have to do this every time your data changes.

In place of the imperative approach, SwiftUI adopts a declarative programming style that makes updating your UI a breeze. Rather than focusing on how to update the UI, you focus on what to update. SwiftUI’s data flow handles the rest. Every time your data changes, SwiftUI rebuilds any views depending on that data from scratch according to the latest data. This means there’s no risk of displaying a loading spinner, a table of results and an error message all at once.

## Example
