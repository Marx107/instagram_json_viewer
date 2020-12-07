# Instagram Data Download Viewer

This script transforms Instagram's data - [that you get via the Data Download Tool](https://www.cnet.com/how-to/how-to-download-all-your-instagram-data/) - to a readable format!

## Features

- Transforms profile information, media and messages to a more readable format in Rmarkdown
- Possibility to create a nicely structured PDF-file with a table of contents for easy navigation

## Requirements

- Python (version 3.0 and above)
- An R installation that can process Rmarkdown (knitr, working LaTeX processor, ...)

## Data Download

Here you can download your data: [Instagram](https://www.instagram.com/download/request/)

## Usage

Tutorial Video: [https://www.youtube.com/watch?v=w-uz1AfLCk8](https://www.youtube.com/watch?v=w-uz1AfLCk8)

- Put "instaview.py" and "instaview.R" into the data directory (e.g. where the all json-files are!)
- Back up your instagram data before you run anything!
- Run "instaview.py" via commandline or doubleclick!
- If R can't process the Rmarkdown:
  - try opening it in RStudio and manually knitting it 
  - OR try running the code from "instaview.R" manually in Rstudio!"

## Issues

- I didn't find a proper way of processing all the strings that contain emoji and other weird characters, so I created a function that removes most of the special characters. This sometimes creates really ugly captions!
- I didn't include contacts.json and likes.json, since I didn't sync my contacts and therefore had no data available on that. When it comes to likes.json I didn't find it very important since there is no information what exactly was liked! Feel free to extend the script to your needs!
- This is rather experimental since I only had my own data to test this with, there's no guarantee that this also works with your data!
