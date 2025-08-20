<!DOCTYPE html>
<html lang="en">
<head>
<title>Student form</title>
</head>
<body>
    <header>
        <h1>Campus Student Registration</h1>
        <nav aria-label="Main Navigation">
            <ul>
                <li><a href="#form">Form</a></li>
                <li><a href="#info">Info</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="form">
            <h2>Fill Out the Form</h2>
            <form action="/submit" method="post" novalidate>
                <fieldset>
                    <legend>Personal Details</legend>
                    <ul>
                        <li>
                            <label for="name">Full Name*:</label>
                            <input type="text" id="name" name="name" placeholder="Enter your full name" required>
                        </li>
                        <li>
                            <label for="email">Email*:</label>
                            <input type="email" id="email" name="email" placeholder="e.g., student@campus.edu" required>
                        </li>
                        <li>
                            <label for="age">Age:</label>
                            <input type="number" id="age" name="age" min="16" max="100" placeholder="Enter your age" required>
                        </li>
                        <li>
                            <label for="dob">Date of Birth:</label>
                            <input type="date" id="dob" name="dob" required>
                        </li>
                        <li>
                            <label for="password">Password*:</label>
                            <input type="password" id="password" name="password" placeholder="Create a password" required pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" title="Must contain at least one number, one uppercase, one lowercase letter, and at least 8 characters">
                        </li>
                        <li>
                            <label for="phone">Phone (readonly):</label>
                            <input type="tel" id="phone" name="phone" value="+1234567890" readonly>
                        </li>
                        <li>
                            <label for="course">Course (autocomplete):</label>
                            <input type="text" id="course" name="course" list="courses" autocomplete="on" placeholder="Select a course">
                            <datalist id="courses">
                                <option value="Computer Science">
                                <option value="Engineering">
                                <option value="Business">
                            </datalist>
                        </li>
                        <li>
                            <button type="submit">Submit</button>
                            <button type="reset">Reset</button>
                        </li>
                    </ul>
                </fieldset>
            </form>
        </section>

        <section id="info">
            <h2>Campus Info</h2>
            <table>
                <thead>
                    <tr>
                        <th>Course</th>
                        <th>Students</th>
                        <th>Duration</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Computer Science</td>
                        <td>150</td>
                        <td>4 years</td>
                    </tr>
                    <tr>
                        <td>Engineering</td>
                        <td>120</td>
                        <td>4 years</td>
                    </tr>
                </tbody>
            </table>
            <p>Check out our <a href="https://campus.edu/media" aria-label="Campus media gallery">media gallery</a>!</p>
            <img src="https://via.placeholder.com/300x200" alt="Campus Image" aria-describedby="img-desc">
            <p id="img-desc">A beautiful view of the campus.</p>
        </section>
    </main>

    <footer>
        <h3>Contact Us</h3>
        <p>&copy; 2025 Mike Nelius Muthomi. All rights reserved.</p>
    </footer>
</body>
</html>
