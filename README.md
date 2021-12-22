# NestedRoutesIonicVue
Bug in Nested Routes Ionic Vue

# Step by step to reproduce
1. Download the project
2. At the root of the project run "npm install"
3. Run the project with "ionic serve"

4. Option 1
  4.1 From the initial page "/ tabs / tab1", press the button "Go page view"
  4.2. In the header press back arrow
  4.3 Go to "Tab 3"
  4.4 Press the tab where it says "Go page create" (Error: It shows the two pages "View" and "Create" at the same time)

5. Option 2
  5.1 From the initial page "/ tabs / tab1", press the button "Go page view"
  5.2. In the header press back arrow
  5.3 Press the tab where it says "Go page create"
  5.4. In the header press back arrow
  5.3 Go to "Tab 3"
  5.1 Press the "Go page view" button (Error: It shows the "Create" page instead of the "View")
