<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Farm Registry - Authentication Web App</title>
</head>
<body>
    <h1>Farm Registry - Authentication Web App</h1>

    <h2>Overview</h2>
    <p>Farm Registry is an authentication-based web application built with <strong>Express.js</strong>, <strong>EJS</strong>, and a <strong>database</strong>. It allows users to <strong>register, log in, and navigate</strong> different sections of the platform, including <strong>Global Community, Learn and Grow, and Innovation</strong>.</p>

    <h2>Features</h2>
    <ul>
        <li>User Registration & Login</li>
        <li>Authentication with a database</li>
        <li>Dynamic Routing for Home Sections</li>
        <li>EJS Templating</li>
        <li>Static File Serving</li>
    </ul>

    <h2>Tech Stack</h2>
    <ul>
        <li><strong>Frontend</strong>: HTML, CSS, JavaScript, EJS</li>
        <li><strong>Backend</strong>: Node.js, Express.js</li>
        <li><strong>Database</strong>: MySQL / MongoDB</li>
    </ul>

    <h2>Installation</h2>
    <h3>1. Clone the Repository</h3>
    <pre><code>git clone https://github.com/your-username/farm-registry.git
cd farm-registry</code></pre>

    <h3>2. Install Dependencies</h3>
    <pre><code>npm install</code></pre>

    <h3>3. Configure Database</h3>
    <p>Create a database (MySQL or MongoDB) and add database credentials to <code>.env</code></p>

    <p>Example <code>.env</code>:</p>
    <pre><code>DB_HOST=localhost
DB_USER=root
DB_PASS=yourpassword
DB_NAME=yourdatabase
PORT=3000</code></pre>

    <h3>4. Start the Server</h3>
    <pre><code>npm start</code></pre>

    <h2>Project Structure</h2>
    <pre><code>📂 farm-registry
├── 📂 node_modules       # Dependencies
├── 📂 views             # EJS Templates
│   ├── 📂 extra
│   │   ├── globalCommunity.ejs
│   │   ├── home.ejs
│   │   ├── innovation.ejs
│   │   ├── learnGrow.ejs
│   ├── login.ejs
│   ├── loginForm.ejs
│   ├── register.ejs
│   ├── registerForm.ejs
│   ├── styling.ejs
├── index.js             # Main entry point
├── Register.js          # User Registration Logic
├── package.json         # Dependencies & Scripts
├── package-lock.json    # Lockfile</code></pre>

    <h2>API Endpoints</h2>
    <table border="">
        <thead>
            <tr>
                <th>Method</th>
                <th>Endpoint</th>
                <th>Description</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>GET</td>
                <td>/</td>
                <td>Home page</td>
            </tr>
            <tr>
                <td>GET</td>
                <td>/home/innovation</td>
                <td>Innovation section</td>
            </tr>
            <tr>
                <td>GET</td>
                <td>/home/community</td>
                <td>Global Community section</td>
            </tr>
            <tr>
                <td>GET</td>
                <td>/home/learnGrow</td>
                <td>Learn and Grow section</td>
            </tr>
            <tr>
                <td>POST</td>
                <td>/register</td>
                <td>Register user</td>
            </tr>
            <tr>
                <td>POST</td>
                <td>/login</td>
                <td>Login user</td>
            </tr>
        </tbody>
    </table>

    <h2>How It Works</h2>
    <ol>
        <li><strong>User Registers</strong> → Data is stored in the database.</li>
        <li><strong>User Logs In</strong> → Credentials are verified.</li>
        <li><strong>Access Home & Sections</strong> → Users navigate through different sections.</li>
    </ol>

    <h2>Future Improvements</h2>
    <ul>
        <li>Password encryption (e.g., bcrypt)</li>
        <li>JWT-based authentication</li>
        <li>Profile management</li>
        <li>Social login integration</li>
    </ul>

    <h2>License</h2>
    <p>This project is licensed under the <strong>MIT License</strong>.</p>
</body>
</html>
