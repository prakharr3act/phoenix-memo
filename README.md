#  phoenix-memo

A minimalist, high-security themed web interface designed to simulate a classified "Project Phoenix" intelligence document.

##  Overview
The **Phoenix Memo** is a lightweight HTML template for creating "Confidential Memos." It provides a professional structure for internal-style briefings, specifically themed around an espionage or high-clearance narrative.

## Features
* **Status Banners:** Pre-defined IDs for `CONFIDENTIAL` and `TOP SECRET` clearance levels.
* **Redaction Logic:** Uses a `.blurred` class to hide sensitive data like agent names, coordinates, and project details.
* **Semantic Structure:** Clean HTML5 layout wrapped in a `<main id="email">` container for easy styling.

##  Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/prakharr3act/phoenix-memo.git](https://github.com/prakharr3act/phoenix-memo.git)

### 1. index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Confidential Memo</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <main id="email">
        <div id="confidential">CONFIDENTIAL</div>
        <div id="top-secret">TOP SECRET</div>

        <p>
            The meeting regarding <span class="blurred">Project Phoenix</span> has been moved to a 
            secure location. Please ensure that <span class="blurred">Agent Smith</span> is notified 
            immediately.
        </p>

        <p>
            The coordinates for the drop-off are <span class="blurred">38.8977° N, 77.0365° W</span>. 
            Do not share this information over unsecured channels.
        </p>

        <p>
            Failure to comply with these protocols will result in <span class="blurred">immediate termination</span> 
            of your clearance level.
        </p>
    </main>
</body>
</html>
