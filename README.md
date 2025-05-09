# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Design with Flexbox and Grid</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Content -->
    <main>
        <section class="left">
            <h2>Welcome to Our Website!</h2>
            <p>This is a simple webpage layout using Flexbox and Grid.</p>
        </section>
        <section class="right">
            <h3>Featured Articles</h3>
            <p>Here are some featured articles related to our services.</p>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Responsive Design Example</p>
    </footer>
</body>
</html>
/* Base styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

nav {
    background-color: #333;
    color: white;
    padding: 1em;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 1em;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 20px;
    padding: 20px;
}

main .left {
    background-color: #f4f4f4;
    padding: 20px;
}

main .right {
    background-color: #e4e4e4;
    padding: 20px;
}

footer {
    text-align: center;
    padding: 1em;
    background-color: #333;
    color: white;
}

/* Mobile first */
@media (max-width: 600px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    main {
        grid-template-columns: 1fr;
    }
}

/* Tablet */
@media (min-width: 601px) and (max-width: 1024px) {
    main {
        grid-template-columns: 1fr 2fr;
    }
}

/* Desktop */
@media (min-width: 1025px) {
    main {
        grid-template-columns: 1fr 3fr;
    }
}


Happy Coding! 💻✨
