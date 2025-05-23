
Module 1-Bootstrap 5
1. Setting Up Bootstrap 5
Exercise 1.1:
Create a basic HTML page and link Bootstrap 5 via CDN.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap 5 CDN Example</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-primary">Hello, Bootstrap 5!</h1>
    <p>This is a simple example using Bootstrap 5 via CDN.</p>
  </div>

  <!-- Bootstrap 5 JS Bundle (includes Popper) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 1.2:
Set up a project using npm or downloaded Bootstrap files. Use the downloaded files in a sample
HTML page.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap 5 Local Example</title>
  <!-- Bootstrap 5 CSS -->
  <link rel="stylesheet" href="css/bootstrap.min.css">
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-success">Hello, Bootstrap 5!</h1>
    <p>This is a simple example using Bootstrap 5 locally.</p>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="js/bootstrap.bundle.min.js"></script>
</body>
</html>
2. Bootstrap Structure and Files
Exercise 2.1:
Explore the structure of the downloaded Bootstrap directory. Identify and explain the purpose of
the CSS, JS, and icons folders.
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   └── ...
├── js/
│   ├── bootstrap.bundle.js
│   ├── bootstrap.bundle.min.js
│   └── ...
└── icons/
    ├── bootstrap-icons.css
    └── ...

Exercise 2.2:
Modify your HTML to include Bootstrap's JavaScript plugins via bootstrap.bundle.min.js.
<head>
  <!-- Bootstrap CSS -->
  <link rel="stylesheet" href="css/bootstrap.min.css">
</head>
<body>
  <!-- Your content here -->

  <!-- Bootstrap JS Bundle -->
  <script src="js/bootstrap.bundle.min.js"></script>
</body>
3. Fundamentals of Responsive Grid Layout
Exercise 3.1:
Create a container with three columns that stack vertically on mobile, two-per-row on tablets,
and three-per-row on desktops.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Grid Example</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 1</div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 2</div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 3</div>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 3.2:
Use .container, .row, and .col-* classes appropriately for responsive design.
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 1 -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 2 -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 3 -->
    </div>
  </div>
</div>
4. Column Layouts and Grid Classes
Exercise 4.1:
Design a two-column layout with a sidebar (col-md-3) and content area (col-md-9).
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Two-Column Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <!-- Sidebar -->
      <div class="col-md-3 bg-light border p-3">
        <h4>Sidebar</h4>
        <p>Sidebar content goes here.</p>
      </div>
      <!-- Main Content -->
      <div class="col-md-9 bg-white border p-3">
        <h4>Main Content</h4>
        <p>Main content goes here.</p>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 4.2:
Create a four-column layout (col-sm-3) with equal width.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Four-Column Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <div class="col-sm-3 bg-light border p-3 text-center">Column 1</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 2</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 3</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 4</div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
5. Alignment and Reordering in Grid
Exercise 5.1:
Use justify-content-center and align-items-center to center content inside a row.
<div class="container" style="height: 300px;">
  <div class="row d-flex justify-content-center align-items-center h-100">
    <div class="col-6 text-center">
      <div class="p-4 bg-light border">
        <p>This content is centered both horizontally and vertically.</p>
      </div>
    </div>
  </div>
</div>

Exercise 5.2:
Reorder columns on different screen sizes using order-md-2, order-md-1.
<div class="container">
  <div class="row">
    <div class="col-md-6 order-md-2 bg-light p-3">
      <h5>Second Column (appears first on small screens)</h5>
      <p>Content for the second column.</p>
    </div>
    <div class="col-md-6 order-md-1 bg-white p-3">
      <h5>First Column (appears second on small screens)</h5>
      <p>Content for the first column.</p>
    </div>
  </div>
</div>
6. Responsive Flexbox Utilities
Exercise 7.1:
Create a navbar using d-flex, flex-column, and flex-md-row for responsive behavior.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Navbar</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <nav class="navbar bg-light">
    <div class="container d-flex flex-column flex-md-row align-items-center justify-content-between">
      <a class="navbar-brand mb-2 mb-md-0" href="#">Brand</a>
      <ul class="nav">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
      </ul>
    </div>
  </nav:contentReference[oaicite:5]{index=5}

Exercise 7.2:
Use justify-content-between and align-items-center in a card layout.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Card Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="card p-3">
      <div class="d-flex justify-content-between align-items-center">
        <div>
          <h5 class="card-title mb-0">Card Title</h5>
          <small class="text-muted">Subtitle</small>
        </div>
        <button class="btn btn-primary">Action</button>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
7. Typography
Exercise 7.1:
Create a sample page with different Bootstrap typography utilities: display-1, lead, text-muted,
fw-bold, etc.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Typography Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h1 class="display-1">Display 1 Heading</h1>
  <p class="lead">This is a lead paragraph. It stands out from regular paragraphs.</p>
  <p class="text-muted">This text is muted, making it less prominent.</p>
  <p class="fw-bold">This text is bold using the <code>.fw-bold</code> class.</p>
  <p class="fst-italic">This text is italicized using the <code>.fst-italic</code> class.</p>
  <p class="text-decoration-underline">This text is underlined using the <code>.text-decoration-underline</code> class.<

Exercise 7.2:
Use text-uppercase, text-lowercase, text-capitalize.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Text Transform Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <p class="text-uppercase">this text is transformed to uppercase.</p>
  <p class="text-lowercase">THIS TEXT IS TRANSFORMED TO LOWERCASE.</p>
  <p class="text-capitalize">this text is transformed to capitalized form.</p>

</body>
</html>
8. Forms
Exercise 8.1:
Create a registration form using Bootstrap form components like form-control, form-check, and
input-group.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Registration Form</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="container">
    <h2 class="mb-4">Register</h2>
    <form>
      <div class="mb-3">
        <label for="fullName" class="form-label">Full Name</label>
        <input type="text" class="form-control" id="fullName" placeholder="Enter your full name">
      </div>

      <div class="mb-3">
        <label for="email" class="form-label">Email address</label>
        <div class="input-group">
          <span class="input-group-text">@</span>
          <input type="email" class="form-control" id="email" placeholder="Enter your email">
        </div>
      </div>

      <div class="mb-3">
        <label for="password" class="form-label">Password</label>
        <input type="password" class="form-control" id="password" placeholder="Enter your password">
      </div>

      <div class="mb-3 form-check">
        <input t

Exercise 8.2:
Style a login form using form-floating
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Login Form</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="container">
    <h2 class="mb-4">Login</h2>
    <form>
      <div class="form-floating mb-3">
        <input type="email" class="form-control" id="loginEmail" placeholder="name@example.com">
        <label for="loginEmail">Email address</label>
      </div>

      <div class="form-floating mb-3">
        <input type="password" class="form-control" id="loginPassword" placeholder="Password">
        <label for="loginPassword">Password</label>
      </div>

      <button type="submit" class="btn btn-primary">Login</button>
    </form>
  </div>

</body>
</html>
9. Buttons
Exercise 9.1:
Create buttons using all contextual classes: btn-primary, btn-secondary, btn-outline-*, etc.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Buttons Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h2>Solid Buttons</h2>
  <button type="button" class="btn btn-primary">Primary</button>
  <button type="button" class="btn btn-secondary">Secondary</button>
  <button type="button" class="btn btn-success">Success</button>
  <button type="button" class="btn btn-danger">Danger</button>
  <button type="button" class="btn btn-warning">Warning</button>
  <button type="button" class="btn btn-info">Info</button>
  <button type="button" class="btn btn-light">Light</button>
  <button type="button" class="btn btn-dark">Dark</button>
  <button type="button" class="btn btn-link">Link</button>

  <h2 class="mt-4">Outline Buttons</h2>
  <button type="button" class="btn btn-outline-primary">Primary</button>
  <button type="button" class="btn btn-outline-secondary">Secondary</button>
  <button type="button" class="btn btn-outline-success">Success</button>
  <button type="button" class="btn btn-outline-danger">Danger

Exercise 9.2:
Add button groups using btn-group, and create toggle buttons with checkboxes
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Button Groups</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h2>Button Group</h2>
  <div class="btn-group" role="group" aria-label="Basic example">
    <button type="button" class="btn btn-primary">Left</button>
    <button type="button" class="btn btn-primary">Middle</button>
    <button type="button" class="btn btn-primary">Right</button>
  </div>

  <h2 class="mt-4">Checkbox Toggle Buttons</h2>
  <div class="btn-group" role="group" aria-label="Checkbox toggle button group">
    <input type="checkbox" class="btn-check" id="btncheck1" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck1">Checkbox 1</label>

    <input type="checkbox" class="btn-check" id="btncheck2" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck2">Checkbox 2</label>

    <input type="checkbox" class="btn-check" id="btncheck3" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck3">Checkbox 3</label>
  </div>

</body>
</html>
10. Navbars and Navigation
Exercise 10.1:
Create a responsive navbar with logo, navigation links, and a search form.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Navbar</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Logo</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pricing</a>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button

Exercise 10.2:
Use nav, nav-tabs, nav-pills for creating tabbed navigation.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Tabbed Navigation</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- Nav Tabs -->
  <ul class="nav nav-tabs" id="myTab" role="tablist">
    <li class="nav-item" role="presentation">
      <a class="nav-link active" id="home-tab" data-bs-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true">Home</a>
    </li>
    <li class="nav-item" role="presentation">
      <a class="nav-link" id="profile-tab" data-bs-toggle="tab" href="#profile" role="tab" aria-controls="profile" aria-selected="false">Profile</a>
    </li>
    <li class="nav-item" role="presentation">
      <a class="nav-link" id="contact-tab" data-bs-toggle="tab" href="#contact" role="tab" aria-controls="contact" aria-selected="false">Contact</a>
    </li>
  </ul>
  <div class="tab-content" id="myTabContent">
    <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">Home content...</div>
    <div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab">Profile content...</div>
    <div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab">Contact content...</div>
  </div>

  <!-- Nav Pills -->
  <ul class="nav nav-pills">
    <li class="nav-item">
      <a class="nav-link active" id="pills-home-tab" data-bs-toggle="pill" href="#pills-home" role="tab" aria-controls="pills-home" aria-selected="true">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" id="pills-profile-tab" data-bs-toggle="pill" href="#pills-profile" role="tab" aria-controls="pills-profile" aria-selected="false">Profile</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" id="pills-contact-tab" data-bs-toggle="pill" href="#pills-contact" role="tab" aria-controls="pills-contact" aria-selected="false">Contact</a>
    </li>
  </ul>
  <div class="tab-content">
    <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">Home content...</div>
    <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">Profile content...</div>
    <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">Contact content...</div>
  </div>

  <!-- Bootstrap JS and Popper.js -->
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.min.js"></script>

</body>
</html>
11. Cards and Media Objects
Exercise 11.1:
Create a profile card using card, card-body, card-title, and card-img-top.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Profile Card</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="card" style="width: 18rem;">
    <img src="https://randomuser.me/api/portraits/men/14.jpg" class="card-img-top" alt="John Doe">
    <div class="card-body">
      <h5 class="card-title">John Doe</h5>
      <p class="card-text">Creative Designer passionate about crafting user-centric digital experiences.</p>
      <a href="#" class="btn btn-primary">Connect</a>
    </div>
  </div>

</body>
</html>

Exercise 11.2:
Design a media object layout using media and align an image to the left of the content.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Media Object</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="d-flex">
    <img src="https://randomuser.me/api/portraits/men/14.jpg" class="me-3 rounded-circle" alt="John Doe" style="width: 60px; height: 60px;">
    <div>
      <h5 class="fw-bold">John Doe</h5>
      <p class="mb-1">Creative Designer passionate about crafting user-centric digital experiences.</p>
      <small class="text-muted">Posted on February 19, 2021</small>
    </div>
  </div>

</body>
</html>
12. Spacing Utilities
Exercise 12.1:
Apply margin (m-3, mt-4) and padding (p-2, py-5) utilities on layout sections.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Spacing Utilities Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <section class="bg-light p-3 mb-4">
      <h2 class="mb-3">Section 1</h2>
      <p>This section has padding and margin applied using Bootstrap's spacing utilities.</p>
    </section>

    <section class="bg-secondary text-white p-2 py-5">
      <h2 class="mb-3">Section 2</h2>
      <p>Notice the larger vertical padding applied here.</p>
    </section>
  </div>

</body>
</html>

Exercise 12.2:
Build a pricing section where spacing improves the layout.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Pricing Section</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container py-5">
    <div class="row row-cols-1 row-cols-md-3 g-4">
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Free</h5>
            <p class="card-text">$0/month</p>
            <ul class="list-unstyled">
              <li>10 users included</li>
              <li>2 GB of storage</li>
              <li>Email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Sign up</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Pro</h5>
            <p class="card-text">$15/month</p>
            <ul class="list-unstyled">
              <li>20 users included</li>
              <li>10 GB of storage</li>
              <li>Priority email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Get started</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Enterprise</h5>
            <p class="card-text">$29/month</p>
            <ul class="list-unstyled">
              <li>30 users included</li>
              <li>15 GB of storage</li>
              <li>Phone and email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Contact us</a>
          </div>
        </div>
      </div>
    </div>
  </div>

</body>
</html>
13. Colors and Backgrounds
Exercise 13.1:
Create a dashboard page using contextual background classes (bg-primary, bg-warning, etc.) and
text colors.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Dashboard</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="row">
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-primary text-white rounded">
          <h5>Sales</h5>
          <p>Monthly sales data and trends.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-warning text-dark rounded">
          <h5>Alerts</h5>
          <p>Recent system alerts and notifications.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-info text-white rounded">
          <h5>Updates</h5>
          <p>Latest updates and news.</p>
        </div>
      </div>
    </div>
  </div>

</body>
</html>

Exercise 13.2:
Use bg-gradient with bg-dark and white text.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Gradient Background</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="p-5 bg-dark bg-gradient text-white rounded">
      <h2>Welcome to the Dashboard</h2>
      <p>Your personalized overview of the system's performance.</p>
    </div>
  </div>

</body>
</html>
14. Display and Visibility
Exercise 14.1:
Use d-none, d-md-block, d-lg-flex to hide/show sections based on screen size.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Display</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="row">
      <div class="col-12">
        <div class="d-none d-md-block p-3 mb-3 bg-primary text-white">
          Visible on medium screens and larger
        </div>
        <div class="d-none d-lg-flex p-3 mb-3 bg-success text-white">
          Visible on large screens and larger
        </div>
        <div class="d-block d-md-none p-3 mb-3 bg-danger text-white">
          Visible on small screens only
        </div>
      </div>
    </div>
  </div>

</body>
</html>

Exercise 14.2:
Create a responsive sidebar that only shows on tablets and above.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Sidebar</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container-fluid">
    <div class="row">
      <!-- Sidebar -->
      <nav class="col-md-3 col-lg-2 d-none d-md-block bg-light sidebar">
        <div class="position-sticky">
          <ul class="nav flex-column">
            <li class="nav-item">
              <a class="nav-link active" href="#">
                Dashboard
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                Orders
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                Products
              </a>
            </li>
          </ul>
        </div>
      </nav>

      <!-- Main content -->
      <main class="col-md-9 ms-sm-auto col-lg-10 px-4">
        <h2>Main Content</h2>
        <p>This is the main content area.</p>
      </main>
    </div>
  </div>

</body>
</html>
15. Borders, Shadows, and Rounded Corners
Exercise 15.1:
Add border utilities like border, border-primary, border-3, and rounded-circle to an image.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Styled Image</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light text-center p-4">

  <img src="https://via.placeholder.com/150" class="border border-primary border-3 rounded-circle" alt="Styled Image">

</body>
</html>

Exercise 15.2:
Use shadow, shadow-lg and rounded-pill in a card.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Card with Shadow</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light p-4">

  <div class="card shadow-lg rounded-pill" style="width: 18rem;">
    <img src="https://via.placeholder.com/150" class="card-img-top rounded-top" alt="Card image">
    <div class="card-body">
      <h5 class="card-title">Card Title</h5>
      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
      <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>

</body>
</html>
16. Positioning Utilities
Exercise 16.1:
Create a fixed footer using position-fixed bottom-0.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Fixed Footer</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="min-vh-100 d-flex flex-column">

  <div class="container my-auto">
    <h1 class="text-center">Main Content</h1>
    <p class="text-center">Add your content here.</p>
  </div>

  <footer class="position-fixed bottom-0 start-0 end-0 bg-dark text-white text-center py-2">
    <p class="mb-0">© 2025 Your Company</p>:contentReference[oaicite:13]{index=13}:contentReference[oaicite:16]{index=16}

Exercise 16.2:
Use position-relative and position-absolute to overlay a badge over an image
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Image with Badge</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="position-relative d-inline-block">
    <img src="https://via.placeholder.com/300" class="img-fluid" alt="Sample Image">
    <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
      New
    </span>
  </div>

</body>
</html>
17. Icons with Bootstrap Icons
Exercise 17.1:
Install and use Bootstrap Icons in a webpage: add social media icons in the footer.
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
<footer class="text-center text-white" style="background-color: #f1f1f1;">
  <div class="container pt-4">
    <section class="mb-4">
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-facebook"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-twitter"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-instagram"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-linkedin"></i>
      </a>
    </section>
  </div>
</footer>

Exercise 17.2:
Replace text buttons with icon-only buttons using Bootstrap Icons.
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
<button type="button" class="btn btn-primary">
  <i class="bi bi-house-door"></i>
</button>
<button type="button" class="btn btn-secondary">
  <i class="bi bi-search"></i>
</button>
<button type="button" class="btn btn-danger">
  <i class="bi bi-trash"></i>
</button>
18. Bootstrap 5 JavaScript Plugins
Exercise 18.1:
Add a modal popup triggered by a button.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Modal Example</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- Button to trigger modal -->
  <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
    Open Modal
  </button>

  <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Modal Title</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          This is a simple modal example.
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          <button type="button" class="btn btn-primary">Save changes</button>
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle:contentReference[oaicite:5]{index=5}

Exercise 18.2:
Create a collapsible accordion using accordion and Bootstrap JavaScript behavior.
         <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Accordion Example</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="accordion" id="accordionExample">
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingOne">
        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          Accordion Item #1
        </button>
      </h2>
      <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the first item's accordion body. It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingTwo">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Accordion Item #2
        </button>
      </h2>
      <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Accordion Item #3
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the third item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
19. Customization with Sass
Exercise 19.1:
Set up a Bootstrap 5 project with Sass using npm.
mkdir my-bootstrap-project
cd my-bootstrap-project
npm init -y
npm install bootstrap sass --save-dev
my-bootstrap-project/
├── scss/
│   └── custom.scss
└── node_modules/
    └── bootstrap/
        ├── scss/
        └── js/
npx sass scss/custom.scss dist/styles.css
npm run build-css
npx sass --watch scss/custom.scss:dist/styles.css

Exercise 19.2:
Customize primary colors and border radius via _variables.scss and recompile Bootstrap.
// _variables.scss
$primary: #ff5733; // Custom primary color
$border-radius: 0.375rem; // Custom border radius
// custom.scss
@import "../node_modules/bootstrap/scss/functions";
@import "../node_modules/bootstrap/scss/variables";
@import "../node_modules/bootstrap/scss/mixins";
@import "../node_modules/bootstrap/scss/bootstrap";

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Module 1-CSS3 Exercises

Theme: Styling the "Local Community Event Portal"
1. Why CSS? Inline vs. Internal vs. External
Scenario: The designer wants you to experiment with different ways to apply styles.
Objective: Understand various CSS inclusion methods and their impact.
Task:
• Apply an inline style to make one heading red.
• Use an embedded <style> tag in the <head> to define body background.
• Link an external stylesheet styles.css and move all reusable styles there.
• Add comments in your CSS to label each section (/* Header styles */)
1. Inline CSS
Usage: Applied directly within an HTML element using the style attribute.

Scope: Affects only the specific element it's applied to.

When to Use: Ideal for quick, one-off styling changes.


2. Internal CSS
Usage: Defined within a <style> tag in the <head> section of an HTML document.

Scope: Affects all elements within the same HTML document.

When to Use: Suitable for single-page documents or when styles are unique to that page.

3. External CSS
Usage: Stored in a separate .css file and linked to the HTML document using the <link> tag.

Scope: Affects multiple HTML documents that link to the same CSS file.

When to Use: Best for multi-page websites to maintain consistent styling across all pages.
Practical Example
HTML File (index.html)
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Styling Methods</title>
    <!-- Internal CSS -->
    <style>
        body {
            background-color: #f0f0f0;
        }
    </style>
    <!-- External CSS -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Inline CSS -->
    <h1 style="color: red;">Welcome to CSS Styling</h1>
    <p>This is a demonstration of different CSS methods.</p>
</body>
</html>
External CSS File (styles.css)
css
Copy
Edit
h1 {
    font-family: 'Arial', sans-serif;
    font-size: 2em;
    text-align: center;
}

p {
    font-family: 'Verdana', sans-serif;
    font-size: 1.2em;
    color: #333;
}
2. CSS Syntax and Comments
Scenario: You’ve joined a team and need to understand and maintain a large stylesheet.
Objective: Write clean, readable CSS with proper structure and comments.
Task:
• Create a section in styles.css with formatted rules and consistent indentation.
• Add descriptive comments above selectors.
• Example:
.cta-button {
 background-color: #007BFF;
 color: white;
}

#navbar {
  background-color: #333; 
  padding: 10px 20px;      
  text-align: center;      
}

#navbar a {
  color: white;            
  padding: 14px 20px;      
  text-decoration: none;   
  display: inline-block;   
}

#navbar a:hover {
  background-color: #ddd;  
  color: black;            
}
.main-content {
  margin: 20px auto;       
  max-width: 1200px;       
  padding: 20px;           
}
.main-content article {
  margin-bottom: 30px;     
  border-bottom: 1px solid #ccc; 
  padding-bottom: 20px;    
}
footer {
  background-color: #333; 
  color: white;          
  text-align: center;     
  padding: 10px 0;       
  position: fixed;        
  bottom: 0;              
  width: 100%;           
}

3. Selectors Playground
Scenario: You need to style various elements based on IDs, classes, and element types.
Objective: Master different selector types.
Task:
• Use:
o Universal selector * to reset margin/padding
o Element selector to style all <h2>
o ID selector #mainHeader for the banner
o Class selector .eventCard for event containers
o Grouping selector for h3, p to style together

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; /* Ensures padding and borders are included in element's total width and height */
}
h2 {
  font-size: 2rem;
  color: #333;
  margin-bottom: 1rem;
}
#mainHeader {
  background-color: #007BFF;
  color: white;
  padding: 20px;
  text-align: center;
}
.eventCard {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 15px;
  margin-bottom: 20px;
  background-color: #f9f9f9;
}
h3, p {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: #555;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#mainHeader {
  background-color: #007BFF;
  color: white;
  padding: 20px;
  text-align: center;
}
.eventCard {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 15px;
  margin-bottom: 20px;
  background-color: #f9f9f9;
}
h2 {
  font-size: 2rem;
  color: #333;
  margin-bottom: 1rem;
}

h3, p {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: #555;
}

4. Color & Background Styling
Scenario: You’re theming the portal based on a city council’s branding.
Objective: Apply consistent colors and background visuals.
Task:
• Use HEX and RGBA for setting text and background colors
• Add a background image to the body with fallback color
• Apply gradients to section headers using background: linear-gradient(...)
h1 {
  color: #2c3e50;
}
section {
  background-color: rgba(46, 204, 113, 0.7); 
}
body {
  background-color: #ecf0f1; 
  background-image: url('cityscape.jpg');
  background-size: cover;
  background-position: center;
}
section header {
  background: linear-gradient(to right, #3498db, #8e44ad); /* Blue to purple */
  color: white;
  padding: 20px;
  text-align: center;
}

5. Typography: Fonts and Text
Scenario: The marketing team wants more appealing fonts and better readability.
Objective: Enhance textual appearance using CSS properties.
Task:
• Use @import or <link> to include a Google Font
• Set font-family, font-size, font-style, font-weight in different sections
• Use text-align, text-transform, letter-spacing, line-height on descriptions
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

body {
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  font-weight: 400;
  font-style: normal;
}
h1 {
  font-family: 'Roboto', sans-serif;
  font-size: 2.5rem;
  font-weight: 700;
  font-style: normal;
}
h2 {
  font-family: 'Roboto', sans-serif;
  font-size: 2rem;
  font-weight: 700;
  font-style: italic;
}
p {
  font-family: 'Roboto', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  font-style: normal;
}
p {
  text-align: justify;
  text-transform: capitalize;
  letter-spacing: 0.5px;
  line-height: 1.6;
}
<html>
<head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap">
  <style>
    body {
      font-family: 'Roboto', sans-serif;
      font-size: 16px;
      font-weight: 400;
      font-style: normal;
    }
    h1 {
      font-family: 'Roboto', sans-serif;
      font-size: 2.5rem;
      font-weight: 700;
      font-style: normal;
    }
    h2 {
      font-family: 'Roboto', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      font-style: italic;
    }
    p {
      font-family: 'Roboto', sans-serif;
      font-size: 1rem;
      font-weight: 400;
      font-style: normal;
      text-align: justify;
      text-transform: capitalize;
      letter-spacing: 0.5px;
      line-height: 1.6;
    }
  </style>
</head>
<body>
  <h1>Welcome to the City Council Portal</h1>
  <h2>Upcoming Events</h2>
  <p>Join us for the annual city cleanup event this Saturday. Volunteers are welcome to participate and make a difference in our community.</p>
</body>
</html>

6. Link and List Styling
Scenario: The default blue links and bullet lists don’t match the design.
Objective: Customize links and lists.
Task:
• Style links with :link, :hover, :active, and :visited pseudo-classes
• Use list-style-type, list-style-position, and remove bullets from nav menus
• Add padding and margin to list items for spacing
a:link {
  color: #0056b3; 
  text-decoration: none;
  font-weight: normal;
}
a:visited {
  color: #800080; 
}
a:hover {
  color: #ff6347; 
  text-decoration: underline;
}

{
  color: #ff4500; 
}
ul {
  list-style-type: none;
  list-style-position: outside;
  margin: 0;
  padding: 0;
}
ul li {
  margin-bottom: 10px;
  padding-left: 20px; 
  position: relative;
}
ul li::before {
  content: '•';
  color: #007bff; 
  position: absolute;
  left: 0;
  top: 0;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-around;
}
nav ul li {
  margin: 0 15px;
  padding: 10px 20px;
}
nav ul li a {
  color: #ffffff;
  text-decoration: none;
  font-weight: bold;
  text-transform: uppercase;
}
nav ul li a:hover {
  color: #ffd700; 
}

7. Table Styling
Scenario: The events admin table needs a cleaner look.
Objective: Format tables using CSS.
Task:
• Style table, th, and td with borders, padding, and background color
• Add zebra striping to rows using nth-child(even)
• Use border-collapse: collapse and text-align: center
table, th, td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: center;
  border-collapse: collapse;
}
tr:nth-child(even) {
  background-color: #f2f2f2;
}
th {
  background-color: #4CAF50;
  color: white;
  font-weight: bold;
}
td:first-child, th:first-child {
  background-color: #e7f7e7;
}

td:last-child, th:last-child {
  background-color: #e7f7e7;
}

8. Box Model & Layout Control
Scenario: Sections are cramped and need spacing.
Objective: Control element spacing with margin, padding, border, and outline.
Task:
• Use developer tools to inspect and tweak box model properties
• Add border, padding, and margin to .eventCard
• Add outline to highlight selected fields in a form
• Compare visibility: hidden vs. display: none
/* Global Box Model Reset */
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  background-color: #f4f4f4;
  color: #333;
  padding: 20px;
}
section {
  margin-bottom: 40px;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
  background-color: white;
}
.eventCard {
  margin: 20px 0;
  padding: 15px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
input:focus,
textarea:focus,
select:focus {
  outline: 3px solid #007bff;
  outline-offset: 2px;
}
.hidden-element {
  visibility: hidden; /* Element is invisible but still occupies space */
}

.removed-element {
  display: none; /* Element is removed from the layout */
}

9. Multiple Columns in Text
Scenario: The community bulletin needs to be displayed like a newspaper.
Objective: Use CSS3 multi-column layout.
Task:
• Create a news article section and apply:
column-count: 2;
column-gap: 30px;
column-rule: 1px solid gray;

.news-article {
  column-count: 2;               
  column-gap: 30px;              
  column-rule: 1px solid gray;   
  padding: 20px;                 
  background-color: #fff;        
  border-radius: 8px;            
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); 
  font-family: 'Georgia', serif; 
  line-height: 1.6;              
}

10. Responsive Web Design with Media Queries
Scenario: Users will access the portal on phones, tablets, and desktops.
Objective: Apply media queries for responsiveness.
Task:
• Add a media query for screens smaller than 768px
• Stack navigation links vertically instead of horizontally
• Reduce image sizes and font sizes
• Use %, vw, vh for flexible layouts
• Bonus: Try Flexbox or Grid for responsive layouts
@media only screen and (max-width: 768px) {
}
@media only screen and (max-width: 768px) {
  nav ul {
    display: block;
    text-align: center;
  }

  nav ul li {
    display: block;
    margin: 10px 0;
  }
}
@media only screen and (max-width: 768px) {
  img {
    width: 100%;
    height: auto;
  }

  body {
    font-size: 14px;
  }
}
.container {
  width: 100%;
  padding: 5%;
}

.header {
  height: 10vh;
}
@media only screen and (max-width: 768px) {
  .flex-container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .flex-item {
    width: 90%;
    margin: 10px 0;
  }
}

11. Debug and Test with Dev Tools and VS Code
Scenario: Some users report layout breaking on smaller screens.
Objective: Use DevTools to test styles and debug.
Task:
• Use Chrome’s device toolbar to simulate different screen sizes
• Inspect applied styles and test different values live
• Use the Network tab to check if the external CSS is loaded
🛠️ Debugging with Chrome DevTools
1. Simulate Different Screen Sizes
Open Chrome DevTools by pressing Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (Mac).

Click the Toggle Device Toolbar button or press Ctrl + Shift + M (Windows/Linux) or Cmd + Shift + M (Mac) to enter device emulation mode.
DevTools Tips
+1
Tutkit.com
+1

Use the Dimensions drop-down to select a specific device or enter custom width and height values. 
Chrome for Developers
+1
DebugBear
+1

To view media query breakpoints, click the More options (three dots) in the device toolbar and select Show media queries. 
Chrome for Developers
+1
DebugBear
+1

2. Inspect Applied Styles
In the Elements panel, select the element you want to inspect.
Chrome for Developers

In the Styles pane, review the applied CSS rules.

To test different values live, modify the CSS properties directly in the Styles pane.

3. Check if External CSS is Loaded
Go to the Network tab in DevTools.
web.dev
+1
Google Help
+1

Reload the page.

Look for your external CSS file (e.g., styles.css) in the list of network requests.

If the file is not listed, ensure that the <link> tag in your HTML file correctly references the CSS file's path.

Testing Responsiveness in Visual Studio Code
1. Use Live Server Extension
Install the Live Server extension from the VS Code Marketplace.
Ritwick Dey

Right-click on your index.html file and select Open with Live Server.

This will launch a local development server and open your webpage in the browser.

As you make changes to your code, the browser will automatically refresh to reflect the updates.

2. Preview in Different Devices
While your page is open in the browser, use the browser's developer tools to simulate different devices and screen sizes, as described in the Chrome DevTools section above

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Module 1-HTML 5

HTML5 Exercises
Project Theme: Local Community Event Portal

A local city council wants a lightweight, browser-based portal to help residents register for
events, check locations, and access basic services.

1. Create the HTML5 Base Template
Scenario: You’re setting up the base document that every page on the portal will use.
Objective: Ensure semantic structure and compatibility across browsers.
Task:
• Use <!DOCTYPE html>, <html lang="en">, <meta charset="UTF-8">
• Add comments to label sections like "Navigation", "Main", "Footer"
• Save as index.html and open it in Chrome
• Inspect the document structure in Chrome Dev Tools
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Local Community Event Portal</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <!-- Navigation -->
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#events">Events</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <main id="home">
    <section id="events">
      <h2>Upcoming Events</h2>
      <!-- Event details go here -->
    </section>
    <section id="contact">
      <h2>Contact Us</h2>
      <!-- Contact form goes here -->
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Local Community Council</p>
  </footer>

</body>
</html>


2. Navigation and Linking
Scenario: Users should navigate between "Home", "Events", and "Contact" sections.
Objective: Provide intuitive navigation and section-based references.
Task:
• Use <nav> with anchor tags <a href="#events">Events</a>
• Define matching IDs for each section like <section id="events">
• Add a link to an external help document using <a href="help.html" target="_blank">
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#events">Events</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="help.html" target="_blank">Help</a></li>
  </ul>
</nav>

3. Welcome Message with Styling and ID/Class
Scenario: Display a welcome banner styled uniquely for a logged-in user.
Objective: Practice block/inline tags and differentiate id and class
Task:
• Use <div id="welcomeBanner"> and apply a blue background via internal CSS
• Use inline styles for a special offer <span> (e.g., color red, bold)
• Apply the .highlight class to certain elements for visual emphasis
<div id="welcomeBanner">
  <h1>Welcome to the Local Community Event Portal</h1>
  <p>Explore upcoming events and connect with your community.</p>
</div>

<p>Special Offer: <span class="highlight">Register now and get a free community guide!</span></p>

4. Image Gallery for Community Events
Scenario: Show images from past events in a table layout.
Objective: Work with <img>, tables, and formatting tags.
Task:
• Use a <table> with 2 rows and 3 columns of <img> tags
• Include alt, title, and style each image with borders using a class
• Add a caption to describe each event
<table>
  <caption>Past Community Events</caption>
  <tr>
    <td><img src="event1.jpg" alt="Community Picnic" title="Community Picnic" class="event-img"></td>
    <td><img src="event2.jpg" alt="Charity Run" title="Charity Run" class="event-img"></td>
    <td><img src="event3.jpg" alt="Art Exhibition" title="Art Exhibition" class="event-img"></td>
  </tr>
  <tr>
    <td><img src="event4.jpg" alt="Food Drive" title="Food Drive" class="event-img"></td>
    <td><img src="event5.jpg" alt="Music Festival" title="Music Festival" class="event-img"></td>
    <td><img src="event6.jpg" alt="Community Clean-up" title="Community Clean-up" class="event-img"></td>
  </tr>
</table>

5. Event Registration Form
Scenario: Residents need to register for events.
Objective: Practice input types, validation, placeholder, autofocus, and output
Task:
• Include fields: name (text), email (email), date (date), event type (select), message
(textarea)
• Add placeholder, required, and autofocus
• Display a confirmation message using <output> when the form is submitted
• Style the form using CSS
<form id="registrationForm">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Your Name" required autofocus><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Your Email" required><br><br>

  <label for="eventType">Event Type:</label>
  <select id="eventType" name="eventType">
    <option value="workshop">Workshop</option>
    <option value="seminar">Seminar</option>
    <option value="webinar">Webinar</option>
  </select><br><br>

  <label for="message">Message:</label><br>
  <textarea id="message" name="message" rows="4" cols="50" placeholder="Your Message"></textarea><br><br>

  <input type="submit" value="Register">
</form>

<output id="confirmationMessage"></output>

6. Event Feedback with Events Handling
Scenario: Collect real-time feedback and interactions from the user.
Objective: Handle blur, change, click, double-click, and keyboard events.
Task:
• Use onblur to validate a phone number field
• Use onchange on a dropdown to display the selected event fee
• onclick on a submit button to show a confirmation
• ondblclick on an image to enlarge it
• Capture key events in the feedback textarea and count characters
<form id="feedbackForm">
  <label for="phone">Phone Number:</label>
  <input type="tel" id="phone" name="phone" onblur="validatePhone()"><br><br>

  <label for="eventFee">Event Fee:</label>
  <select id="eventFee" name="eventFee" onchange="displayFee()">
    <option value="free">Free</option>
    <option value="paid">Paid</option>
  </select><br><br>

  <label for="feedback">Feedback:</label><br>
  <textarea id="feedback" name="feedback" rows="4" cols="50" oninput="countCharacters()"></textarea><br><br>

  <input type="submit" value="Submit">
</form>

<p id="phoneValidation"></p>
<p id="feeDisplay"></p>
<p id="charCount">Characters: 0</p>

7. Video Invite with Media Events
Scenario: Show a short event promo video.
Objective: Work with <video> and oncanplay event
Task:
• Insert a <video> element with source and controls
• Use oncanplay to display a message like "Video ready to play"
• Use onbeforeunload to warn users if they try to leave the form page unfinished
<video id="promoVideo" width="320" height="240" controls oncanplay="videoReady()">
  <source src="promo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<script>
  function videoReady() {
    alert("Video is ready to play!");
  }
</script>

8. Saving User Preferences
Scenario: Store preferred event type for returning users.
Objective: Work with localStorage, sessionStorage, and deletion
Task:
• Save selected event type in localStorage
• On reload, retrieve and pre-select it
• Add a "Clear Preferences" button that clears both localStorage and sessionStorage
<select id="eventType" onchange="savePreference()">
  <option value="workshop">Workshop</option>
  <option value="seminar">Seminar</option>
  <option value="webinar">Webinar</option>
</select>

<button onclick="clearPreferences()">Clear Preferences</button>

<script>
  window.onload = function() {
    const savedPreference = localStorage.getItem('preferredEventType');
    if (savedPreference) {
      document.getElementById('eventType').value = savedPreference;
    }
  };

  function savePreference() {
    const selectedEventType = document.getElementById('eventType').value;
    localStorage.setItem('preferredEventType', selectedEventType);
  }

  function clearPreferences() {
    localStorage.removeItem('preferredEventType');
    sessionStorage.clear();
    alert("Preferences cleared!");
  }
</script>

9. Geolocation for Event Mapping
Scenario: Locate the nearest event to the user.
Objective: Practice geolocation.getCurrentPosition, error handling, and options
Task:
• Create a button “Find Nearby Events”
• On click, use getCurrentPosition to get and display coordinates
• Handle permission denial and timeouts
• Use high accuracy options

::contentReference[oaicite:138]{index=138}
 
10.Debugging with Chrome DevTools
Scenario: A few users report layout issues and script errors.
Objective: Use Chrome DevTools and VS Code features to debug.
Task:
• Use “Inspect Element” to modify styles and experiment live
• Use the Console tab to view logs from your <script>
• Add breakpoints in JS and reload the page to watch variable values
Debugging with Chrome DevTools
1. Inspect and Modify Styles Live
Open DevTools: Press Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (Mac).

Navigate to the Elements Panel: Here, you can select any element on your page to view and edit its HTML and CSS.

Edit Styles: In the Styles pane, modify CSS properties to see changes in real-time. This helps in adjusting margins, padding, colors, and more to fix layout issues.

2. Monitor JavaScript Errors
Access the Console Panel: Switch to the Console tab to view any JavaScript errors or warnings.

Log Outputs: Use console.log() in your scripts to output variable values and track the flow of execution.

Clear Console: Click the trash can icon to clear the console for fresh logs.
DEV Community

3. Set Breakpoints and Step Through Code
Open the Sources Panel: Locate your JavaScript file in the file navigator.

Add Breakpoints: Click on the line number where you want to pause execution.

Control Execution: Use the buttons to step over, step into, or resume script execution.

Inspect Variables: Check the Scope and Watch panels to view variable values and call stack.
DEV Community
+1
CoderPad
+1
HappyFox
+3
Buddy
+3
DEV Community
+3

 Debugging with Visual Studio Code
1. Set Up Browser Debugging
Install Chrome Debugger Extension: In VS Code, go to the Extensions view (Ctrl + Shift + X), search for "Debugger for Chrome," and install it.

Configure Launch Settings: Create a launch.json file in the .vscode folder with the following configuration:
Visual Studio Code

json
Copy
Edit
  {
    "version": "0.2.0",
    "configurations": [
      {
        "type": "chrome",
        "request": "launch",
        "name": "Launch Chrome against localhost",
        "url": "http://localhost:3000",
        "webRoot": "${workspaceFolder}"
      }
    ]
  }
Replace "http://localhost:3000" with the URL of your local development server.

2. Start Debugging
Launch Debugger: Press F5 or click on the green play button in the Run and Debug panel.

Set Breakpoints: Click on the gutter next to line numbers in your JavaScript files to set breakpoints.

Inspect Variables: Use the Variables and Watch panels to monitor variable values during execution.

Debug Console: View outputs and errors in the Debug Console.
Visual Studio Code
+3
Stack Overflow
+3
Zapier
+3

Practical Tips
Reproduce the Issue: Consistently reproduce the bug to understand its behavior.

Use Conditional Breakpoints: Right-click a breakpoint and select "Edit breakpoint" to add conditions, pausing execution only when specific criteria are met.

Monitor Network Requests: Use the Network panel to view API calls and responses, ensuring data is fetched correctly.

Check for Layout Shifts: Utilize the Performance panel to record and analyze layout shifts and rendering issues
Module 1-HTML 5
HTML5 Exercises
Project Theme: Local Community Event Portal
A local city council wants a lightweight, browser-based portal to help residents register for
events, check locations, and access basic services.
1. Create the HTML5 Base Template
Scenario: You’re setting up the base document that every page on the portal will use.
Objective: Ensure semantic structure and compatibility across browsers.
Task:
• Use <!DOCTYPE html>, <html lang="en">, <meta charset="UTF-8">
• Add comments to label sections like "Navigation", "Main", "Footer"
• Save as index.html and open it in Chrome
• Inspect the document structure in Chrome Dev Tools
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Local Community Event Portal</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <!-- Navigation -->
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#events">Events</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <main id="home">
    <section id="events">
      <h2>Upcoming Events</h2>
      <!-- Event details go here -->
    </section>
    <section id="contact">
      <h2>Contact Us</h2>
      <!-- Contact form goes here -->
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Local Community Council</p>
  </footer>

</body>
</html>


2. Navigation and Linking
Scenario: Users should navigate between "Home", "Events", and "Contact" sections.
Objective: Provide intuitive navigation and section-based references.
Task:
• Use <nav> with anchor tags <a href="#events">Events</a>
• Define matching IDs for each section like <section id="events">
• Add a link to an external help document using <a href="help.html" target="_blank">
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#events">Events</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="help.html" target="_blank">Help</a></li>
  </ul>
</nav>

3. Welcome Message with Styling and ID/Class
Scenario: Display a welcome banner styled uniquely for a logged-in user.
Objective: Practice block/inline tags and differentiate id and class
Task:
• Use <div id="welcomeBanner"> and apply a blue background via internal CSS
• Use inline styles for a special offer <span> (e.g., color red, bold)
• Apply the .highlight class to certain elements for visual emphasis
<div id="welcomeBanner">
  <h1>Welcome to the Local Community Event Portal</h1>
  <p>Explore upcoming events and connect with your community.</p>
</div>

<p>Special Offer: <span class="highlight">Register now and get a free community guide!</span></p>
4. Image Gallery for Community Events
Scenario: Show images from past events in a table layout.
Objective: Work with <img>, tables, and formatting tags.
Task:
• Use a <table> with 2 rows and 3 columns of <img> tags
• Include alt, title, and style each image with borders using a class
• Add a caption to describe each event
<table>
  <caption>Past Community Events</caption>
  <tr>
    <td><img src="event1.jpg" alt="Community Picnic" title="Community Picnic" class="event-img"></td>
    <td><img src="event2.jpg" alt="Charity Run" title="Charity Run" class="event-img"></td>
    <td><img src="event3.jpg" alt="Art Exhibition" title="Art Exhibition" class="event-img"></td>
  </tr>
  <tr>
    <td><img src="event4.jpg" alt="Food Drive" title="Food Drive" class="event-img"></td>
    <td><img src="event5.jpg" alt="Music Festival" title="Music Festival" class="event-img"></td>
    <td><img src="event6.jpg" alt="Community Clean-up" title="Community Clean-up" class="event-img"></td>
  </tr>
</table>
5. Event Registration Form
Scenario: Residents need to register for events.
Objective: Practice input types, validation, placeholder, autofocus, and output
Task:
• Include fields: name (text), email (email), date (date), event type (select), message
(textarea)
• Add placeholder, required, and autofocus
• Display a confirmation message using <output> when the form is submitted
• Style the form using CSS
<form id="registrationForm">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Your Name" required autofocus><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Your Email" required><br><br>

  <label for="eventType">Event Type:</label>
  <select id="eventType" name="eventType">
    <option value="workshop">Workshop</option>
    <option value="seminar">Seminar</option>
    <option value="webinar">Webinar</option>
  </select><br><br>

  <label for="message">Message:</label><br>
  <textarea id="message" name="message" rows="4" cols="50" placeholder="Your Message"></textarea><br><br>

  <input type="submit" value="Register">
</form>

<output id="confirmationMessage"></output>
6. Event Feedback with Events Handling
Scenario: Collect real-time feedback and interactions from the user.
Objective: Handle blur, change, click, double-click, and keyboard events.
Task:
• Use onblur to validate a phone number field
• Use onchange on a dropdown to display the selected event fee
• onclick on a submit button to show a confirmation
• ondblclick on an image to enlarge it
• Capture key events in the feedback textarea and count characters
<form id="feedbackForm">
  <label for="phone">Phone Number:</label>
  <input type="tel" id="phone" name="phone" onblur="validatePhone()"><br><br>

  <label for="eventFee">Event Fee:</label>
  <select id="eventFee" name="eventFee" onchange="displayFee()">
    <option value="free">Free</option>
    <option value="paid">Paid</option>
  </select><br><br>

  <label for="feedback">Feedback:</label><br>
  <textarea id="feedback" name="feedback" rows="4" cols="50" oninput="countCharacters()"></textarea><br><br>

  <input type="submit" value="Submit">
</form>

<p id="phoneValidation"></p>
<p id="feeDisplay"></p>
<p id="charCount">Characters: 0</p>
7. Video Invite with Media Events
Scenario: Show a short event promo video.
Objective: Work with <video> and oncanplay event
Task:
• Insert a <video> element with source and controls
• Use oncanplay to display a message like "Video ready to play"
• Use onbeforeunload to warn users if they try to leave the form page unfinished
<video id="promoVideo" width="320" height="240" controls oncanplay="videoReady()">
  <source src="promo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<script>
  function videoReady() {
    alert("Video is ready to play!");
  }
</script>
8. Saving User Preferences
Scenario: Store preferred event type for returning users.
Objective: Work with localStorage, sessionStorage, and deletion
Task:
• Save selected event type in localStorage
• On reload, retrieve and pre-select it
• Add a "Clear Preferences" button that clears both localStorage and sessionStorage
<select id="eventType" onchange="savePreference()">
  <option value="workshop">Workshop</option>
  <option value="seminar">Seminar</option>
  <option value="webinar">Webinar</option>
</select>

<button onclick="clearPreferences()">Clear Preferences</button>

<script>
  window.onload = function() {
    const savedPreference = localStorage.getItem('preferredEventType');
    if (savedPreference) {
      document.getElementById('eventType').value = savedPreference;
    }
  };

  function savePreference() {
    const selectedEventType = document.getElementById('eventType').value;
    localStorage.setItem('preferredEventType', selectedEventType);
  }

  function clearPreferences() {
    localStorage.removeItem('preferredEventType');
    sessionStorage.clear();
    alert("Preferences cleared!");
  }
</script>
9. Geolocation for Event Mapping
Scenario: Locate the nearest event to the user.
Objective: Practice geolocation.getCurrentPosition, error handling, and options
Task:
• Create a button “Find Nearby Events”
• On click, use getCurrentPosition to get and display coordinates
• Handle permission denial and timeouts
• Use high accuracy options

::contentReference[oaicite:138]{index=138}
 
10.Debugging with Chrome DevTools
Scenario: A few users report layout issues and script errors.
Objective: Use Chrome DevTools and VS Code features to debug.
Task:
• Use “Inspect Element” to modify styles and experiment live
• Use the Console tab to view logs from your <script>
• Add breakpoints in JS and reload the page to watch variable values
Debugging with Chrome DevTools
1. Inspect and Modify Styles Live
Open DevTools: Press Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (Mac).

Navigate to the Elements Panel: Here, you can select any element on your page to view and edit its HTML and CSS.

Edit Styles: In the Styles pane, modify CSS properties to see changes in real-time. This helps in adjusting margins, padding, colors, and more to fix layout issues.

2. Monitor JavaScript Errors
Access the Console Panel: Switch to the Console tab to view any JavaScript errors or warnings.

Log Outputs: Use console.log() in your scripts to output variable values and track the flow of execution.

Clear Console: Click the trash can icon to clear the console for fresh logs.
DEV Community

3. Set Breakpoints and Step Through Code
Open the Sources Panel: Locate your JavaScript file in the file navigator.

Add Breakpoints: Click on the line number where you want to pause execution.

Control Execution: Use the buttons to step over, step into, or resume script execution.

Inspect Variables: Check the Scope and Watch panels to view variable values and call stack.
DEV Community
+1
CoderPad
+1
HappyFox
+3
Buddy
+3
DEV Community
+3

🖥 Debugging with Visual Studio Code
1. Set Up Browser Debugging
Install Chrome Debugger Extension: In VS Code, go to the Extensions view (Ctrl + Shift + X), search for "Debugger for Chrome," and install it.

Configure Launch Settings: Create a launch.json file in the .vscode folder with the following configuration:
Visual Studio Code

json
Copy
Edit
  {
    "version": "0.2.0",
    "configurations": [
      {
        "type": "chrome",
        "request": "launch",
        "name": "Launch Chrome against localhost",
        "url": "http://localhost:3000",
        "webRoot": "${workspaceFolder}"
      }
    ]
  }
Replace "http://localhost:3000" with the URL of your local development server.

2. Start Debugging
Launch Debugger: Press F5 or click on the green play button in the Run and Debug panel.

Set Breakpoints: Click on the gutter next to line numbers in your JavaScript files to set breakpoints.

Inspect Variables: Use the Variables and Watch panels to monitor variable values during execution.

Debug Console: View outputs and errors in the Debug Console.
Visual Studio Code
+3
Stack Overflow
+3
Zapier
+3

Practical Tips
Reproduce the Issue: Consistently reproduce the bug to understand its behavior.

Use Conditional Breakpoints: Right-click a breakpoint and select "Edit breakpoint" to add conditions, pausing execution only when specific criteria are met.

Monitor Network Requests: Use the Network panel to view API calls and responses, ensuring data is fetched correctly.

Check for Layout Shifts: Utilize the Performance panel to record and analyze layout shifts and rendering issues

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Module-1 JavaScript
Project Theme: "Local Community Event Portal" 
Users can view upcoming events, register, filter events by category or location, and interact 
dynamically with the portal. 
1. JavaScript Basics & Setup 
Scenario: Set up your community portal to use JavaScript. 
Objective: Configure environment and test basic script functionality. 
Task: 
• Use <script src="main.js"></script> in HTML 
• Log "Welcome to the Community Portal" using console.log() 
• Use an alert to notify when the page is fully loaded
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Community Portal</title>
  <script src="main.js" defer></script>
</head>
<body>
  <h1>Community Events</h1>
</body>
</html>
console.log("Welcome to the Community Portal");

window.onload = () => {
  alert("Page is fully loaded");
};

2. Syntax, Data Types, and Operators 
Scenario: Store event details like name, date, and available seats. 
Objective: Use proper data types and operations. 
Task: 
• Use const for event name and date, let for seats 
• Concatenate event info using template literals 
• Use ++ or -- to manage seat count on registration
const eventName = "Music Night";
const eventDate = "2025-06-15";
let seats = 30;

console.log(`Event: ${eventName} on ${eventDate}, Seats left: ${seats}`);

// Simulate registration
seats--;
console.log(`Seats after registration: ${seats}`);

3. Conditionals, Loops, and Error Handling 
Scenario: Only show valid events and limit registrations. 
Objective: Apply conditions and handle invalid data. 
User Story: As a user, I want only upcoming events with seats to be displayed. 
Task: 
• Use if-else to hide past or full events 
• Loop through the event list and display using forEach() 
• Wrap registration logic in try-catch to handle errors
const events = [
  { name: "Yoga Class", date: "2025-06-01", seats: 10 },
  { name: "Art Fair", date: "2025-05-01", seats: 0 },
];

const today = new Date("2025-05-23");

events.forEach(event => {
  const eventDate = new Date(event.date);
  if (eventDate > today && event.seats > 0) {
    console.log(`Upcoming Event: ${event.name}`);
  } else {
    console.log(`Skipping: ${event.name}`);
  }
});

function register(event) {
  try {
    if (event.seats > 0) {
      event.seats--;
      console.log(`Registered for ${event.name}. Seats left: ${event.seats}`);
    } else {
      throw new Error("No seats available");
    }
  } catch (e) {
    console.error(e.message);
  }
}

4. Functions, Scope, Closures, Higher-Order Functions 
Scenario: Create reusable functions for event operations. 
Objective: Encapsulate logic and use closures. 
Task: 
• Create addEvent(), registerUser(), filterEventsByCategory() 
• Use closure to track total registrations for a category 
• Pass callbacks to filter functions for dynamic search
function addEvent(events, newEvent) {
  events.push(newEvent);
}

function registerUser(event) {
  event.seats--;
}

function filterEventsByCategory(events, category) {
  return events.filter(e => e.category === category);
}

function categoryCounter() {
  let count = 0;
  return function () {
    count++;
    return count;
  };
}

const musicCounter = categoryCounter();

function dynamicFilter(events, callback) {
  return events.filter(callback);
}

5. Objects and Prototypes 
Scenario: Each event is an object with properties and methods. 
Objective: Model real-world entities using objects. 
Task: 
• Define Event constructor or class 
• Add checkAvailability() to prototype 
• List object keys and values using Object.entries()
function Event(name, date, seats) {
  this.name = name;
  this.date = date;
  this.seats = seats;
}

Event.prototype.checkAvailability = function () {
  return this.seats > 0;
};

const yoga = new Event("Yoga", "2025-06-01", 10);

console.log(Object.entries(yoga));

6. Arrays and Methods 
Scenario: Manage an array of all community events. 
Objective: Use array methods for CRUD operations. 
Task: 
• Add new events using .push() 
• Use .filter() to show only music events 
• Use .map() to format display cards (e.g., "Workshop on Baking")
const allEvents = [];

allEvents.push({ name: "Baking Workshop", category: "Food" });

const musicEvents = allEvents.filter(e => e.category === "Music");

const displayCards = allEvents.map(e => `Event: ${e.name}`);
console.log(displayCards);

7. DOM Manipulation 
Scenario: Display all events dynamically on the webpage. 
Objective: Render events using JS. 
Task: 
• Access DOM elements using querySelector() 
• Create and append event cards using createElement() 
• Update UI when user registers or cancels
const eventContainer = document.querySelector("#eventContainer");

function renderEvent(event) {
  const div = document.createElement("div");
  div.textContent = `${event.name} - ${event.date}`;
  eventContainer.appendChild(div);
}

8. Event Handling 
Scenario: Add interactive elements like buttons and filters. 
Objective: Respond to user actions. 
Task: 
• Use onclick for "Register" buttons 
• Use onchange to filter events by category 
• Use keydown to allow quick search by name
document.querySelector("#registerBtn").onclick = () => {
  alert("You registered!");
};

document.querySelector("#categoryFilter").onchange = (e) => {
  filterEventsByCategory(allEvents, e.target.value);
};

document.querySelector("#search").onkeydown = (e) => {
  if (e.key === "Enter") {
    dynamicFilter(allEvents, ev => ev.name.includes(e.target.value));
  }
};

9. Async JS, Promises, Async/Await 
Scenario: Fetch event data from a mock API. 
Objective: Use asynchronous logic for remote operations. 
Task: 
• Fetch events from a mock JSON endpoint 
• Use .then() and .catch() to handle results 
• Rewrite using async/await and show loading spinner 
// Using .then()
fetch("events.json")
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error(err));

// Using async/await
async function fetchEvents() {
  document.querySelector("#loading").style.display = "block";
  try {
    const res = await fetch("events.json");
    const data = await res.json();
    console.log(data);
  } finally {
    document.querySelector("#loading").style.display = "none";
  }
}

10. Modern JavaScript Features 
Scenario: Refactor code to be concise and maintainable. 
Objective: Use ES6+ features. 
Task: 
• Use let, const, default parameters in functions 
• Use destructuring to extract event details 
• Use spread operator to clone event list before filtering
function greetUser(name = "Guest") {
  return `Hello, ${name}`;
}

const { name, date, seats } = { name: "Dance Night", date: "2025-06-15", seats: 20 };

const clonedEvents = [...allEvents];

11. Working with Forms 
Scenario: Create a registration form for event sign-up. 
Objective: Connect form inputs to JavaScript. 
Task: 
• Capture name, email, and selected event using form.elements 
• Prevent default form behavior using event.preventDefault() 
• Validate inputs and show errors inline
<form id="registrationForm">
  <input name="name" />
  <input name="email" />
  <select name="event"></select>
  <button type="submit">Register</button>
</form>

12. AJAX & Fetch API 
Scenario: Send user registration to the server. 
Objective: Simulate backend communication. 
Task: 
• Use fetch() to POST user data to a mock API 
• Show success/failure message after submission 
• Use setTimeout() to simulate a delayed response
function submitRegistration(data) {
  setTimeout(() => {
    fetch("https://mockapi.io/register", {
      method: "POST",
      body: JSON.stringify(data),
      headers: { "Content-Type": "application/json" },
    })
      .then(res => res.json())
      .then(() => alert("Registered successfully"))
      .catch(() => alert("Registration failed"));
  }, 1000);
}

13. Debugging and Testing 
Scenario: Registration is failing silently. You need to debug. 
Objective: Use browser tools to inspect and fix issues. 
Task: 
• Use Chrome Dev Tools Console and Network tab 
• Add breakpoints and inspect variables 
• Log form submission steps and check fetch request payload
console.log("Form submitted with: ", data);
debugger;

14. jQuery and JS Frameworks 
Scenario: Use jQuery to simplify DOM tasks. 
Objective: Understand and use jQuery. 
Task: 
• Use $('#registerBtn').click(...) to handle click events 
• Use .fadeIn() and .fadeOut() for event cards 
• Mention one benefit of moving to frameworks like React or Vue
// Using jQuery
$('#registerBtn').click(() => {
  alert("You clicked register!");
});

$('.eventCard').fadeIn();

// Framework Benefit:

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



