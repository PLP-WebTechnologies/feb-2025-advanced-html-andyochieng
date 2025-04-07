# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced HTML5 Elements and Forms</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 10px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            width: 100%;
            margin: 20px 0;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .radio-group, .checkbox-group {
            margin: 10px 0;
        }
        .radio-group label, .checkbox-group label {
            display: inline;
            font-weight: normal;
            margin-left: 5px;
        }
        button {
            padding: 10px 15px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        img {
            max-width: 100%;
            height: auto;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <!-- Main heading -->
    <h1>Advanced HTML5 Elements and Forms</h1>
    
    <!-- Ordered list with Roman numerals -->
    <section>
        <h2>Course Outline</h2>
        <ol type="I">
            <li>Introduction to HTML5</li>
            <li>HTML5 Semantic Elements</li>
            <li>Lists and Tables</li>
            <li>Forms and Input Types</li>
            <li>HTML5 Multimedia</li>
        </ol>
    </section>
    
    <!-- External image from Pexels -->
    <section>
        <h2>Featured Image</h2>
        <img src="https://images.pexels.com/photos/270348/pexels-photo-270348.jpeg" 
             alt="Coding on a computer screen" 
             title="HTML5 Programming">
        <p>Image source: Pexels.com</p>
    </section>
    
    <!-- Table of contacts -->
    <section>
        <h2>Contact Directory</h2>
        <table>
            <caption>Contact Information</caption>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John Smith</td>
                    <td>123 Main St, Boston, MA</td>
                    <td>(555) 123-4567</td>
                    <td>john.smith@example.com</td>
                </tr>
                <tr>
                    <td>Sarah Johnson</td>
                    <td>456 Oak Ave, Chicago, IL</td>
                    <td>(555) 234-5678</td>
                    <td>sarah.j@example.com</td>
                </tr>
                <tr>
                    <td>Michael Wong</td>
                    <td>789 Pine Rd, San Francisco, CA</td>
                    <td>(555) 345-6789</td>
                    <td>michael.w@example.com</td>
                </tr>
                <tr>
                    <td>Jessica Lee</td>
                    <td>101 Maple Dr, Austin, TX</td>
                    <td>(555) 456-7890</td>
                    <td>jessica.lee@example.com</td>
                </tr>
                <tr>
                    <td>David Miller</td>
                    <td>202 Cedar Ln, Seattle, WA</td>
                    <td>(555) 567-8901</td>
                    <td>david.m@example.com</td>
                </tr>
            </tbody>
        </table>
    </section>
    
    <!-- Registration form -->
    <section>
        <h2>Registration Form</h2>
        <form id="registration" action="#" method="post">
            <!-- Name field -->
            <div class="form-group">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            </div>
            
            <!-- Email field -->
            <div class="form-group">
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
            </div>
            
            <!-- Password field -->
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" 
                       placeholder="Create a password" 
                       pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" 
                       title="Must contain at least one number, one uppercase and lowercase letter, and at least 8 characters"
                       required>
                <small>Password must contain at least 8 characters, including uppercase, lowercase, and numbers</small>
            </div>
            
            <!-- Date field -->
            <div class="form-group">
                <label for="birthdate">Date of Birth:</label>
                <input type="date" id="birthdate" name="birthdate" required>
            </div>
            
            <!-- Dropdown -->
            <div class="form-group">
                <label for="country">Country:</label>
                <select id="country" name="country" required>
                    <option value="">Select your country</option>
                    <option value="usa">United States</option>
                    <option value="canada">Canada</option>
                    <option value="uk">United Kingdom</option>
                    <option value="australia">Australia</option>
                    <option value="other">Other</option>
                </select>
            </div>
            
            <!-- Radio buttons -->
            <div class="form-group">
                <label>Gender:</label>
                <div class="radio-group">
                    <input type="radio" id="male" name="gender" value="male" required>
                    <label for="male">Male</label>
                </div>
                <div class="radio-group">
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Female</label>
                </div>
                <div class="radio-group">
                    <input type="radio" id="non-binary" name="gender" value="non-binary">
                    <label for="non-binary">Non-binary</label>
                </div>
                <div class="radio-group">
                    <input type="radio" id="prefer-not-to-say" name="gender" value="prefer-not-to-say">
                    <label for="prefer-not-to-say">Prefer not to say</label>
                </div>
            </div>
            
            <!-- Checkboxes -->
            <div class="form-group">
                <label>Interests (select all that apply):</label>
                <div class="checkbox-group">
                    <input type="checkbox" id="web-dev" name="interests" value="web-dev">
                    <label for="web-dev">Web Development</label>
                </div>
                <div class="checkbox-group">
                    <input type="checkbox" id="mobile-dev" name="interests" value="mobile-dev">
                    <label for="mobile-dev">Mobile Development</label>
                </div>
                <div class="checkbox-group">
                    <input type="checkbox" id="ui-ux" name="interests" value="ui-ux">
                    <label for="ui-ux">UI/UX Design</label>
                </div>
                <div class="checkbox-group">
                    <input type="checkbox" id="data-science" name="interests" value="data-science">
                    <label for="data-science">Data Science</label>
                </div>
            </div>
            
            <!-- Submit button -->
            <div class="form-group">
                <button type="submit">Register</button>
                <button type="reset">Reset Form</button>
            </div>
        </form>
    </section>
    
    <!-- HTML5 Multimedia section -->
    <section>
        <h2>HTML5 Multimedia</h2>
        
        <!-- Audio element -->
        <h3>Audio Sample</h3>
        <audio controls>
            <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        
        <!-- Video element -->
        <h3>Video Sample</h3>
        <video width="400" controls>
            <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </section>
    
    <footer>
        <p>&copy; 2025 Advanced HTML5 Course. All rights reserved.</p>
    </footer>
</body>
</html>
