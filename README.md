Escape Code is a simple web page designed to display a dynamically updated access code and provide users with a download link to the latest panel.

Features
Live Code Display: Fetches the latest access code dynamically from a JSON file (code.json).
Download Button: A centered button that redirects users to download the latest panel from MEGA.
Glowing Navigation Bar: A smooth, blurred glowing effect at the bottom of the navbar.
Responsive Design: The webpage is styled for a clean and modern look.
Setup and Usage
Upload the index.html file to your web server or local environment.
Ensure you have a code.json file that contains the latest access code in the following format:
json
Copy
Edit
{
  "code": "1234"
}
The webpage will automatically fetch and update the displayed access code every 10 seconds.

How It Works
The fetchCode() function in the JavaScript script fetches the latest access code from code.json and updates the webpage.
The MEGA download button (#download-button) redirects users to your provided MEGA folder link.
The last updated text (#update-time) can be manually updated to show the last change made to the MEGA folder.

Customization
Change the MEGA Link: Update the href attribute inside the <button> element in index.html.
Modify the Style: Edit the CSS inside the <style> tag to change colors, fonts, or layouts.
Change Code Fetching Interval: Modify setInterval(fetchCode, 10000); in the script section to adjust the update frequency.
