Interactive Map Management Guide
1. How to Update and Maintain the Google Sheets Database
Accessing Your Google Sheets:
•	Go to Google Sheets.
•	Sign in with the sanctuary@madhucentre.ca Google account.
•	Open the spreadsheet provided, titled Community Resources Map.

Adding New Entries:
•	Locate the bottom of your data in the spreadsheet.
•	Enter new information row by row in the corresponding columns.
•	Map icons are generated based on the Category field, so ensure new entries use the same.

Editing Existing Entries:
•	Navigate to the data entry you wish to update.
•	Click on the cell and start typing to make changes.

Deleting Entries:
•	Click on the row number on the left to select the entire row.
•	Right-click and select "Delete row" from the context menu.

________________________________________

2. Switching to the 211 API
Before You Begin:
•	Ensure you have obtained the necessary permissions and API access credentials from the NB 211 service provider.

Steps to Integrate the 211 API:
•	Find the section in your map’s code that handles data fetching.
•	Replace the Google Sheets API endpoint with the NB 211 API endpoint provided.
•	Update the data parsing logic to accommodate the data structure returned by the 211 API.
•	Test the integration thoroughly to ensure that the map displays the new data correctly.

Handling API Changes:
•	Keep documentation of both the Google Sheets and 211 API for reference.
•	Monitor the functioning of the map regularly to catch and resolve any issues due to API updates or data changes.

________________________________________

3. Integrating the Map into a Squarespace Website
Embedding the Map:
•	Log in to your Squarespace dashboard.
•	Navigate to the page where you want to embed the map.
•	Click an insertion point and select "Embed" from the menu.
•	Click the "</>" icon in the URL field, switch to code input mode, and paste the HTML code for the map (Appendix A).
•	Press Apply to save and display the map.

Customizing Map Appearance:
•	Adjust the width and height parameters in the HTML code to match your website layout.
•	Use Squarespace's design options to further refine the appearance and placement.

________________________________________

4. Managing Geocoding: Converting Street Addresses to Map Points
Understanding Geocoding:
•	The Google Geocoding API is used to convert street addresses from your Google Sheets into geographic coordinates (latitude and longitude). These coordinates are necessary for placing the markers on the map.

Using Geocoding:
•	When Adding or Updating Entries: When you input a new address or update an existing one in the Google Sheets, the map's script automatically sends this address to the Google Geocoding API to retrieve the corresponding coordinates.
•	Map Update: Once the coordinates are retrieved, they are used to place or update markers on the map according to their accurate geographical position.

Testing Geocoding:
•	After adding or updating addresses in the spreadsheet, view your map to ensure the markers appear in the correct locations. If markers do not appear or are in incorrect locations, check the accuracy and formatting of the addresses entered.

Adjusting Your Map’s Code if Switching to the 211 API:
•	If the 211 API provides geographic coordinates, disable the Google Geocoding API.
•	Modify the map’s script to directly use the coordinates provided by the 211 API.
•	Thoroughly test the map to ensure all data points are correctly plotted.

________________________________________

5. Updating Map Features
Customizing Markers and Other Features:
•	Access the map’s JavaScript code.
•	Modify the attributes of markers or paths directly in the code.
•	Use the Google Maps JavaScript API documentation for reference on additional features you can implement.

Adding New Functionalities:
•	Explore the Google Maps API for new functionalities like traffic layers, street view, or custom controls.
•	Implement them by adding the respective JavaScript code snippets to your map setup.

________________________________________

6. Managing APIs and Billing in Google Cloud
Navigating Google Cloud Console:
•	Visit the Google Cloud Console.
•	Select your project linked to the map.
•	Navigate to "APIs & Services" to view or modify your API configurations, titled Community Resources Map.

Updating API Keys:
•	Go to "Credentials".
•	View details of your existing API keys.
•	Set restrictions or regenerate keys as needed to keep your application secure.

Managing Billing:
•	Switch to the "Billing" section via the console.
•	Check your current billing status and set up budget alerts.
•	Update payment methods to ensure uninterrupted service.
•	Be sure to update payment method upon integration.

For Further Assistance:
•	If you encounter any complexities or require clarification, contact Courtney le Roux at CourtneyEleRoux@gmail.com or 1 506 608 8923.
