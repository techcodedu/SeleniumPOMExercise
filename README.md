
# Selenium WebDriver Exercise: Agricultural Resources Website

## Introduction
This exercise will guide you through automated web testing using Selenium WebDriver with Java and the Page Object Model (POM) design pattern. Your target application is a locally hosted website detailing agricultural resources.

## Exercise Setup
- Set up a Maven project in your IDE and configure it with the necessary dependencies for Selenium WebDriver and WebDriverManager.
- Download Liver Server extension via VSCode

## Local Website
The following HTML files represent your local website about agricultural resources. These should be served using the Live Server extension in VSCode.

```markdown
### `index.html` (Homepage)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agricultural Resources</title>
</head>
<body>
    <h1>Agricultural Resources</h1>
    <ul id="resource-list">
        <li><a href="resource1.html">Resource 1: Soil Improvement</a></li>
        <li><a href="resource2.html">Resource 2: Water Conservation</a></li>
        <!-- More resources can be added here -->
    </ul>
</body>
</html>
```

### `resource1.html` (Resource Detail Page)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Soil Improvement</title>
</head>
<body>
    <h1>Soil Improvement Techniques</h1>
    <p>Details about soil improvement...</p>
    <a href="index.html">Back to Resources</a>
</body>
</html>
```

### `resource2.html` (Another Resource Detail Page)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Conservation</title>
</head>
<body>
    <h1>Water Conservation Strategies</h1>
    <p>Details about water conservation...</p>
    <a href="index.html">Back to Resources</a>
</body>
</html>
```

### Serving the Website Locally
Right-click on your `index.html` file, and select `Open with Live Server` to serve your website locally.

## Exercise Instructions

### Task 1: Page Object Creation
Create page objects in Java for the homepage (`HomePage`) and the individual resource detail pages (`Resource1Page`, `Resource2Page`, etc.). These classes should encapsulate the structure and the functionalities of the respective web pages.

### Task 2: Writing Test Cases
Develop test cases using JUnit in Java that will:
- Verify that the homepage correctly lists all available resources.
- Check that each resource link on the homepage navigates to the correct resource detail page.
- Confirm that each resource detail page displays the expected information.

### Task 3: Test Execution
Run your tests against the local website served by the Live Server and ensure they all pass successfully.

## Additional Guidelines
- Utilize WebDriverManager to automate the management of the browser driver.
- Implement the POM pattern to keep your test code clean and maintainable.
- Document your code with comments where necessary to maintain readability and ease of maintenance.
```
