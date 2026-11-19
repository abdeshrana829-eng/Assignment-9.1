1. Project Structure
Create the following files:


text
Assignment-9.1/
│
├── index.html
└── style.css
2. HTML Code (index.html)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Photo Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>My Photo Gallery</h1>
        <p>Explore Beautiful Moments</p>
    </header>

    <nav>
        <a href="#">Home</a>
        <a href="#">Gallery</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>

    <main>
        <h2>My Gallery</h2>

        <section class="gallery">
            <div class="card">
                <img src="https://picsum.photos/id/1015/500/350" alt="Mountain landscape">
                <h3>Mountain View</h3>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1018/500/350" alt="Nature landscape">
                <h3>Beautiful Nature</h3>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1019/500/350" alt="Forest">
                <h3>Green Forest</h3>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1020/500/350" alt="Wildlife">
                <h3>Wildlife</h3>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1024/500/350" alt="Animal">
                <h3>Beautiful Animal</h3>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1035/500/350" alt="River">
                <h3>River View</h3>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2026 My Photo Gallery. All Rights Reserved.</p>
    </footer>

</body>
</html>
3. CSS Code (style.css)
This CSS follows a mobile-first approach and includes two breakpoints.


css

/* General Styling */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header */
header {
    background-color: #243b55;
    color: white;
    text-align: center;
    padding: 25px 10px;
}

/* Navigation */
nav {
    display: flex;
    flex-direction: column;
    text-align: center;
    background-color: #141e30;
}

nav a {
    color: white;
    text-decoration: none;
    padding: 12px;
}

/* Main Section */
main {
    padding: 20px;
}

h2 {
    text-align: center;
    margin-bottom: 20px;
}

/* Mobile First Gallery */
.gallery {
    display: grid;
    grid-template-columns: 1fr;
    gap: 20px;
}

.card {
    background-color: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 2px 8px rgba(0,0,0,0.15);
}

.card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    display: block;
}

.card h3 {
    padding: 15px;
    text-align: center;
}

/* Footer */
footer {
    background-color: #141e30;
    color: white;
    text-align: center;
    padding: 20px;
}

/* Tablet Breakpoint */
@media (min-width: 600px) {
    nav {
        flex-direction: row;
        justify-content: center;
    }

    .gallery {
        grid-template-columns: repeat(2, 1fr);
    }
}

/* Desktop Breakpoint */
@media (min-width: 992px) {
    .gallery {
        grid-template-columns: repeat(3, 1fr);
    }

    main {
        max-width: 1200px;
        margin: auto;
    }

    header {
        padding: 40px;
    }
}
4. Responsive Layout
Mobile view
Below 600px · 1 column

My Photo Gallery

Explore Beautiful Moments

Home · Gallery · About · Contact
Mountain View

Beautiful Nature

Green Forest

Tablet view
600px–991px · 2 columns

Mountain View

Beautiful Nature

Green Forest

Wildlife

Desktop view
992px and above · 3 columns

Mountain

Nature

Forest

Wildlife

Animal

River

5. Breakpoints Used
Device

Screen width

Gallery columns

Mobile

Below 600px

1

Tablet

600px–991px

2

Desktop

992px and above

3

6. Testing Using Chrome DevTools
Open index.html in Google Chrome.

Right-click the webpage and select Inspect.

Click the Toggle Device Toolbar icon.

Select different devices or enter custom widths.

Test mobile, tablet, and desktop layouts.

Check for horizontal scrolling and overlapping elements.

7. Submission Screenshots
Take these three screenshots and save them in your assignment folder:

Screenshot 1: Mobile View

Set viewport width to 375px.

Screenshot 2: Tablet View

Set viewport width to 768px.

Screenshot 3: Desktop View

Set viewport width to 1366px.

8. Final Submission Checklist

Updated index.html

Updated style.css

Viewport meta tag added

Mobile-first CSS implemented

At least two media query breakpoints added

Responsive navigation implemented

Horizontal overflow fixed

Mobile screenshot captured

Tablet screenshot captured

Desktop screenshot captured