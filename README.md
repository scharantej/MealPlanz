## Flask Application Design

### HTML Files

* **index.html**: The main page of the application, where users can input their dietary restrictions and calorie needs. It should include:
    - A form with fields for **dietary restrictions**, **calorie needs**, and a **submit button**.
* **results.html**: The page that displays the meal plan based on the user's input. It should contain:
    - A table with columns for **Breakfast**, **Lunch**, **Dinner**, and **Snacks**.
    - Each row should represent a day of the week.
    - The cells should be populated with suggested meals that meet the user's dietary restrictions and calorie needs.

### Routes

* **index**: The route for the main page (`/`). Maps to the `index.html` file. Supports GET requests only.
* **results**: The route for the results page (`/results`). Maps to the `results.html` file. Supports POST requests to handle the form submission.
    - Processes the user's dietary restrictions and calorie needs.
    - Generates a meal plan using an external API or a custom algorithm.
    - Renders the `results.html` template with the meal plan.