# google-timeline-urls
generated URLs to download Google timeline historical data before Dec. 1, 2024

# Quick Start:
## WARNING - this is an extremly tedious solution and will consume many hours of your time. The process needs to be watched nearly constantly as multiple server requests eventually lock you out of maps.google.com and you need to unlock it. It's also the only solution I'm aware of. 

1. Save the 2010.01.01-2024.11.30.json and sample.json files somewhere. The main file covers dates from January 1, 2010 through November 30, 2024.
2. Edit the saved file to remove unnecessary ranges. You do not want to download years' of empty .kml files. Verify what data you need by checking in timeline.google.com to see the earliest date you need. Delete the rest.
3. Install DownloadThemAll: https://www.downthemall.net/
4. Set your browser to not ask where to download each time. Settings --> Download
5. Open a tab to https://timeline.google.com/ and authenticate if necessary. Leave this tab open to click Refresh and then "I am not a robot" every few minutes.
6. Open the extension and click Manager: <img align="middle" src="https://github.com/user-attachments/assets/8c4cab5e-3317-4c17-81d2-72e10a9a3ec1" width=20% height=20%>
7. Right-click and choose Import from file: <img align="middle" src="https://github.com/user-attachments/assets/55a715b6-c8f0-47bd-89ef-b134f88e19c7" width=30% height=30%>
8. Select the .json file. You may want to try first with sample.json to see that it all works before using the file with the full date range.
9. Enter a destination folder if you need: <img align="middle" src="https://github.com/user-attachments/assets/ebc56efc-016d-4b68-beb4-7ca3d8eabbcc" width=80% height=80%>
8. Select all and click Start
9. Now the fun begins. Go to your timeline.google.com page and click refresh. After a few minutes click refresh agiain. It will eventually present a robot challenge: <img align="middle" src="https://github.com/user-attachments/assets/552869e6-d6fc-4033-a2d2-766269ce6488" width=20% height=20%>
10. After proving you're a human go back to the DownloadThemAll list and Select all and click Resume. You may choose to delete completed downloads from the list.
11. Rinse and repeat. 

----

This is solution was based off of this Reddit thread:
https://old.reddit.com/r/GoogleMaps/comments/1g1mbbo/guide_to_massbatch_download_all_your/

There were several other resources used that I lost track of. One of them was a Google Sheets Apps Script that converts a spreadsheet to JSON.

I run Firefox so needed a different plug-in than the Chrome-based one. Found that DownloadThemAll works well in Firefox. Inspiration from:
https://www.leniel.net/2010/07/automate-batch-download-mass-list-urls.html

Link to my spreadsheet:
https://docs.google.com/spreadsheets/d/1smeI897Y_DpSqu_2v1v2ranV3koTR4tGEDzB6WJWAWU/edit?usp=sharing

The Export JSON project was found here:
https://dev.to/oschertar/how-to-export-your-data-from-google-sheets-to-json-3ih8
Built from code shared by Pamela Fox: https://github.com/pamelafox
