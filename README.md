# KBART_oclc_lookup

Using OpenRefine and OCLC's WorldCat Search APIs, the process searches and suggest good matching OCLC number for WorldCat knowledge base KBART file.

# What you need
1. OpenRefine (openrefine.org)
2. Your own WSKey (https://www.oclc.org/developer/develop/authentication/how-to-request-a-wskey.en.html)
3. WorldShare Collection Manager KBART file 

# Steps
1. Replace {YOUR_WSKEY} with your own WSKey in KBART_oclc_lookup.txt.
2. Open OpenRefine and create a new project.
3. Once your spreadsheet is uploaded, go to Undo/Redo tab, click "Apply."
4. Copy the entire JSON code in KBART_oclc_lookup.txt and paste it into the pop-up window.
5. Click "Perform Operations."

The process adds a new column called "Suggested_OCLC_Number." If the search fails, it returns "Check manually." If the search finds an OCLC number that is same as the existing OCLC number in the "oclc_number" column, it returns "Good". If the OCLC number is not same as the existing OCLC number, it suggests the OCLC number. 

# Demo
https://youtu.be/zQ6_OFPAdNg