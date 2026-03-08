================================================================================
                        MODERN PORTFOLIO TEMPLATE
                        Complete Setup Guide
================================================================================

Created by: [Your Name]
Version: 1.0
Last Updated: 2024

================================================================================
                              QUICK START
================================================================================

1. Download and extract the ZIP file
2. Open 'index.html' in any text editor (VS Code, Sublime Text, Notepad++)
3. Find and replace the placeholder content (see CUSTOMIZATION section below)
4. Save the file
5. Upload to any web host (Netlify, Vercel, GitHub Pages) or open in browser
6. Done! Your portfolio is live.

================================================================================
                           WHAT'S INCLUDED
================================================================================

✓ index.html - Complete portfolio website (HTML + CSS + JavaScript in one file)
✓ Responsive design - Works perfectly on mobile, tablet, and desktop
✓ Dark/Light mode - Automatic toggle with memory
✓ Smooth animations - Scroll effects, hover states, and transitions
✓ Contact form - Ready for client inquiries
✓ Professional sections: Hero, About, Projects, Skills, Contact
✓ No external dependencies (except Font Awesome icons via CDN)

================================================================================
                          CUSTOMIZATION GUIDE
================================================================================

------------------------------ STEP 1: YOUR INFO ------------------------------

Open index.html and find these placeholders using Ctrl+F (Windows) or Cmd+F (Mac):

YOUR NAME:
Find: John Doe
Replace with: Your Full Name
(Appears in: Hero section, Footer copyright)

YOUR EMAIL:
Find: john.doe@example.com
Replace with: your.email@example.com
(Appears in: Contact section)

YOUR PHONE:
Find: +1 (555) 123-4567
Replace with: Your Phone Number
(Appears in: Contact section)

YOUR LOCATION:
Find: San Francisco, CA
Replace with: Your City, Country
(Appears in: Contact section)

YOUR PHOTO:
Find: https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d
Replace with: URL to your photo, or local image path
Recommended size: 400x400 pixels or larger
(Appears in: Hero section)

----------------------------- STEP 2: ABOUT YOU -----------------------------

Find the About section and replace:

YOUR BIO:
Find the paragraphs starting with "I'm a passionate developer..."
Replace with your own story, background, and experience

YOUR STATS:
Find: data-target="50" (Projects Completed)
Change to your actual number

Find: data-target="30" (Happy Clients)
Change to your actual number

Find: data-target="5" (Years Experience)
Change to your actual number

--------------------------- STEP 3: YOUR PROJECTS ---------------------------

Find the Projects section. There are 3 project cards. For each card:

PROJECT TITLE:
Find: E-Commerce Platform / Task Management App / Data Visualization Dashboard
Replace with your project names

PROJECT DESCRIPTION:
Replace the description text with details about your project

PROJECT TAGS:
Change the technology tags (React, Node.js, etc.) to match your stack

PROJECT LINKS:
Find: href="#"
Replace with your actual live demo URL and GitHub repository URL

TO ADD MORE PROJECTS:
Copy a complete project-card div block and paste it after the last one
TO REMOVE PROJECTS:
Delete an entire project-card div block

--------------------------- STEP 4: YOUR SKILLS ---------------------------

Find the Skills section. Three categories are included:

FRONTEND SKILLS:
- HTML5 & CSS3 (95%)
- JavaScript (ES6+) (90%)
- React.js (85%)
- Vue.js (80%)

BACKEND SKILLS:
- Node.js (85%)
- Python (75%)
- PostgreSQL (80%)
- MongoDB (75%)

TOOLS & OTHERS:
- Git & GitHub (90%)
- Figma (85%)
- Docker (70%)
- AWS (65%)

TO CHANGE SKILL NAME:
Replace the text inside <span class="skill-name">

TO CHANGE PERCENTAGE:
Replace data-width="95%" with your desired percentage
Replace the text inside <span class="skill-percent"> to match

TO ADD MORE SKILLS:
Copy a skill-item div block and paste inside the category

TO ADD NEW CATEGORY:
Copy an entire skill-category div and customize

------------------------- STEP 5: SOCIAL LINKS -------------------------

Find the Footer section. Replace the # with your actual URLs:

GitHub:     href="#"  →  href="https://github.com/yourusername"
LinkedIn:   href="#"  →  href="https://linkedin.com/in/yourprofile"
Twitter:    href="#"  →  href="https://twitter.com/yourhandle"
Dribbble:   href="#"  →  href="https://dribbble.com/yourusername"
Instagram:  href="#"  →  href="https://instagram.com/yourhandle"

TO REMOVE A SOCIAL LINK:
Delete the entire <a> tag for that platform
TO ADD MORE:
Copy a social-link <a> tag and change the icon class and URL

================================================================================
                         CUSTOMIZATION (ADVANCED)
================================================================================

--------------------------- CHANGE COLORS ---------------------------

Find the :root CSS variables (near the top of the file):

--primary-color: #6366f1;    (Main purple - change to your brand color)
--secondary-color: #8b5cf6;  (Secondary purple - slightly different shade)

Replace the hex codes with your preferred colors.
Examples:
- Blue: #3b82f6 / #2563eb
- Green: #10b981 / #059669
- Red: #ef4444 / #dc2626
- Orange: #f97316 / #ea580c

--------------------------- CHANGE FONTS ---------------------------

Find: font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

Replace with your preferred font. Options:
- Google Fonts: Import a font from fonts.google.com and replace
- System fonts: 'Arial', 'Helvetica', 'Georgia', etc.

--------------------------- META INFORMATION ---------------------------

Find the <title> tag and change:
<title>John Doe - Creative Developer</title>
To: <title>Your Name - Your Title</title>

Find the <meta name="description"> tag and update the content for SEO.

================================================================================
                           HOW TO DEPLOY
================================================================================

--------------------------- OPTION 1: NETLIFY (FREE) ---------------------------

1. Go to https://www.netlify.com
2. Sign up for free account
3. Drag and drop your index.html file onto the dashboard
4. Get instant custom URL (yoursite.netlify.app)
5. Optional: Connect custom domain

--------------------------- OPTION 2: VERCEL (FREE) ---------------------------

1. Go to https://vercel.com
2. Sign up with GitHub account
3. Click "New Project"
4. Import GitHub repo OR upload files directly
5. Deploy automatically

--------------------------- OPTION 3: GITHUB PAGES (FREE) ---------------------------

1. Create GitHub account at https://github.com
2. Create new repository (name: yourusername.github.io)
3. Upload index.html to repository
4. Go to Settings > Pages
5. Select branch "main", folder "/ (root)"
6. Your site is live at https://yourusername.github.io

--------------------------- OPTION 4: TRADITIONAL HOSTING ---------------------------

1. Purchase hosting (Bluehost, HostGator, SiteGround, etc.)
2. Access cPanel or FTP
3. Upload index.html to public_html folder
4. Access via your domain name

================================================================================
                           TROUBLESHOOTING
================================================================================

PROBLEM: Images not showing
SOLUTION: Check that image URLs are correct and accessible. For local images,
          ensure they're in the same folder as index.html or use correct path.

PROBLEM: Dark mode not working
SOLUTION: Make sure you haven't deleted the JavaScript code at the bottom.
          The theme toggle requires the script section to function.

PROBLEM: Contact form not sending emails
SOLUTION: This template uses a simulated form. To make it functional, you need:
          - Netlify Forms (add netlify attribute to <form>)
          - Formspree (action="https://formspree.io/f/YOUR_ID")
          - Or connect to your own backend

PROBLEM: Skills bars not animating
SOLUTION: Ensure the JavaScript is intact. The animation triggers when you
          scroll to the skills section.

PROBLEM: Changes not showing
SOLUTION: Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
          or try opening in incognito mode.

================================================================================
                           TIPS FOR SUCCESS
================================================================================

✓ Use high-quality profile photo (professional headshot recommended)
✓ Keep project descriptions concise but impactful
✓ Use real project screenshots instead of icons when possible
✓ Update regularly with new projects and skills
✓ Test on multiple devices before publishing
✓ Keep your contact information current
✓ Share your portfolio on LinkedIn, Twitter, and job applications

================================================================================
                           LICENSE & TERMS
================================================================================

[Choose and keep only ONE option below:]

--- OPTION A: Personal Use Only ---
This template is licensed for personal use only. You may use it for your own
portfolio but cannot resell, redistribute, or use for commercial client projects.

--- OPTION B: Commercial Use Allowed ---
This template includes a commercial license. You may use it for personal
portfolios and client projects. Reselling the template itself is prohibited.

--- OPTION C: Extended License ---
This template can be used for unlimited personal and commercial projects.
Modification and redistribution is allowed. Reselling as a template is prohibited.

================================================================================
                              SUPPORT
================================================================================

For questions, issues, or customization requests:

Email: [your-support-email@example.com]
Website: [your-website.com]
Twitter: [@yourhandle]

Response time: 24-48 hours

================================================================================
                          THANK YOU!
================================================================================

Thank you for purchasing this template! If you found it useful, please consider:

⭐ Leaving a review on Gumroad
📢 Sharing with friends and colleagues
💬 Providing feedback for future improvements

Good luck with your portfolio!

================================================================================
