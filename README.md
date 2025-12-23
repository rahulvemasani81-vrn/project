# Project Responsive Web Design using Bootstrap
# Date:
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Showcase</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --dark-bg: #121212;
            --card-bg: #1e1e1e;
            --text-primary: #ffffff;
            --text-secondary: #aaaaaa;
            --accent: #4a6fa5;
        }
    
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background-color: var(--dark-bg);
        color: var(--text-primary);
    }
    
    .navbar {
        background-color: var(--card-bg);
        border-bottom: 1px solid #333;
    }
    
    .navbar-brand {
        font-weight: bold;
        color: var(--text-primary) !important;
    }
    
    .btn-primary {
        background-color: var(--accent);
        border-color: var(--accent);
    }
    
    .btn-outline-secondary {
        border-color: var(--text-secondary);
        color: var(--text-secondary);
    }
    
    .btn-outline-secondary:hover {
        background-color: transparent;
        border-color: var(--text-primary);
        color: var(--text-primary);
    }
    
    .hero-section {
        background-color: var(--dark-bg);
        padding: 80px 0;
        border-bottom: 1px solid #333;
    }
    
    .shot-card {
        background-color: var(--card-bg);
        border-radius: 8px;
        padding: 20px;
        margin-bottom: 20px;
        border: 1px solid #333;
        height: 100%;
    }
    
    .shot-placeholder {
        background-color: #2a2a2a;
        height: 200px;
        display: flex;
        align-items: center;
        justify-content: center;
        margin-bottom: 15px;
        border-radius: 4px;
        color: var(--text-secondary);
    }
    
    .user-avatar {
        width: 30px;
        height: 30px;
        border-radius: 50%;
        background-color: #333;
        display: inline-flex;
        align-items: center;
        justify-content: center;
        margin-right: 10px;
        color: var(--text-secondary);
        font-size: 12px;
    }
    
    footer {
        background-color: #0a0a0a;
        padding: 50px 0 20px;
        border-top: 1px solid #333;
    }
    
    .footer-links a {
        color: var(--text-secondary);
        text-decoration: none;
        display: block;
        margin-bottom: 8px;
    }
    
    .footer-links a:hover {
        color: var(--text-primary);
    }
    
    @media (max-width: 768px) {
        .hero-section {
            text-align: center;
            padding: 60px 0;
        }
        
        .navbar-collapse {
            background-color: var(--card-bg);
            padding: 15px;
            margin-top: 10px;
            border-radius: 4px;
        }
    }
</style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">DesignHub</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Inspiration</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Find Work</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Learn Design</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Pro Features</a>
                    </li>
                </ul>
                <div class="d-flex">
                    <div class="input-group me-3">
                        <input type="text" class="form-control bg-dark text-light border-dark" placeholder="Search...">
                        <button class="btn btn-outline-secondary" type="button">
                            <i class="fas fa-search"></i>
                        </button>
                    </div>
                    <a href="#" class="btn btn-primary me-2">Upload</a>
                    <a href="#" class="btn btn-outline-secondary">Sign In</a>
                </div>
            </div>
        </div>
    </nav>

<!-- Hero Section -->
<section class="hero-section">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-md-6">
                <h1 class="display-4 fw-bold mb-4">Discover creative design work</h1>
                <p class="lead mb-4 text-secondary">Browse thousands of design projects from top creatives worldwide.</p>
                <a href="#" class="btn btn-primary btn-lg">Get Started</a>
            </div>
            <div class="col-md-6">
                <div class="shot-placeholder">
                    [Featured Design Work]
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Featured Shots Section -->
<section class="py-5">
    <div class="container">
        <div class="d-flex justify-content-between align-items-center mb-4">
            <h2>Popular Design Projects</h2>
            <a href="#" class="text-decoration-none">View all <i class="fas fa-arrow-right"></i></a>
        </div>
        
        <div class="row">
            <!-- Shot 1 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        UI Design Project
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">JD</span>
                            <span>John Designer</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Shot 2 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        Mobile App Concept
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">AD</span>
                            <span>Anna Designer</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Shot 3 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        Brand Identity
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">CD</span>
                            <span>Creative Director</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Shot 4 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        Web Design
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">WD</span>
                            <span>Web Designer</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Shot 5 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        Illustration
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">IL</span>
                            <span>Illustrator</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Shot 6 -->
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="shot-card">
                    <div class="shot-placeholder">
                        Typography
                    </div>
                    <div class="shot-info">
                        <div class="d-flex align-items-center">
                            <span class="user-avatar">TY</span>
                            <span>Type Designer</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Call to Action -->
<section class="py-5 bg-dark">
    <div class="container text-center">
        <h2 class="mb-4">Ready to showcase your work?</h2>
        <p class="lead mb-4 text-secondary">Join our community of professional designers and creatives.</p>
        <a href="#" class="btn btn-primary btn-lg">Sign Up Now</a>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="container">
        <div class="row">
            <div class="col-md-3 mb-4">
                <h5 class="mb-4">DesignHub</h5>
                <p class="text-secondary">The leading platform for designers to showcase their work and connect with clients.</p>
            </div>
            <div class="col-md-3 mb-4">
                <h5 class="mb-4">For Designers</h5>
                <div class="footer-links">
                    <a href="#">Explore work</a>
                    <a href="#">Design blog</a>
                    <a href="#">Weekly resources</a>
                    <a href="#">Design jobs</a>
                </div>
            </div>
            <div class="col-md-3 mb-4">
                <h5 class="mb-4">Hire Designers</h5>
                <div class="footer-links">
                    <a href="#">Post a project</a>
                    <a href="#">Browse designers</a>
                    <a href="#">Pricing</a>
                </div>
            </div>
            <div class="col-md-3 mb-4">
                <h5 class="mb-4">Company</h5>
                <div class="footer-links">
                    <a href="#">About</a>
                    <a href="#">Careers</a>
                    <a href="#">Support</a>
                    <a href="#">Terms</a>
                    <a href="#">Privacy</a>
                </div>
            </div>
        </div>
        <hr class="mt-4 mb-4" style="border-color: #333;">
        <div class="row">
            <div class="col-md-6">
                <p class="text-secondary small">© 2023 DesignHub. All rights reserved.</p>
            </div>
            <div class="col-md-6 text-md-end">
                <p class="text-secondary small">15,328 design projects shared</p>
            </div>
        </div>
    </div>
</footer>

<!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
# OUTPUT:
<img width="798" height="572" alt="image" src="https://github.com/user-attachments/assets/e5b4c2c9-2fb2-422d-bf2b-128980363fac" />

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
