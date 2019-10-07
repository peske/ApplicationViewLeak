# Purpose

The purpose of the project is to demonstrate a memory leak which happens while opening / closing `ApplicationView` instances.


# Usage

 1. Start the app and remember it's initial memory consumption (in Task Manager);
 2. Click the giant button "New Window" (you cannot miss it - the window contains only this button) to open another window;
 3. Close the new window;
 4. Repeat steps 2 and 3 and notice how memory consumption rises about 1M per every opened / closed window.
You can also first open multiple windows, and then close them one-by-one, except the last one (if you close the last window, the app will exit, of course).
