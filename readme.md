# Kids Game Day Dashboard

## Project Overview

The Kids Game Day event, organized by Fort Worth Game Night,
features a variety of board games available for borrowing. This project 
aims to provide a comprehensive view of the games checked in and out during the event,
helping to understand trends and manage inventory effectively.

## Files Overview
- **Anon_Data_Cleaning_KGD.ipynb** - Jupyter Notebook detailing the cleaning process. 
- **clean_data_anonymized.csv** - a version of the clean data with PII removed. 
- **index.html** - ['embedded'](https://lmhan122.github.io/Kids-Game-Day-Board-Game-Library/) view of Tableau dashboard. [Can also be found online here.](https://public.tableau.com/views/KidsGameDay2024-FortWorthGameNight/MYFINALFORMATDASHBOARD?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)
- **requirements.txt**

### Dataset Overview

The dataset used in this project includes detailed information about each board game borrowed during the event.
Fort Worth Game Night provided 'KidsGameDayLibrary2024.pdf' which was a hand written form showing all avaliable 
games.

Key columns in the dataset include:

- **Game Name**
- **Copy Number**
- **Time Out**
- **Time In**
- **Name**

Initial cleaning and formatting were performed in Excel, followed by further refinement using Python in a Jupyter Notebook.

### Data Cleaning Steps

1. **Initial Preparation in Excel:**
   - Downloaded the "FWGN Kids Game Day Volunteers March 16 2024" file.
   - Retained only the "Game Check Out Sheet" and renamed the file to "Game List."
   - Added a new column "Copy" and moved copy numbers from the "Game Name" column to the "Copy" column.
   - Switched the "Time Out" and "Time In" column names to align with the form in the "KidsGameDayLibrary2024.pdf."
   - Manually filled in missing data from the scanned copy of "KidsGameDayLibrary2024.pdf."
   - For unclear check-ins/outs with empty fields, adjusted the time to be checked out for one minute.
   - Verified handwritten game names on BoardGameGeek.com when possible.
   - Used "Guest" for missing names.

2. **Further Cleaning in Python:**
   - Imported the cleaned CSV file into a Jupyter Notebook.
   - Applied additional cleaning techniques using Pandas and NumPy to handle any remaining issues and standardize the data.

### Why Use Python for Data Cleaning?

While initial data cleaning in tools like Excel and Google Sheets is convenient, Python offers a more scalable and reproducible approach. By scripting the cleaning processes, we can:

- Automate repetitive tasks.
- Handle larger datasets efficiently.
- Maintain a clear and documented record of all cleaning steps.

### Dashboard Features

The dashboard provides the following features:
- **Overview of Check-in and Check-out Activities:** Visualize the number of games borrowed and returned.
- **Game Popularity:** Identify the most frequently borrowed games.
- **Borrower Analysis:** Insights into borrowing patterns and frequencies.
- **Time Analysis:** Understand peak times for borrowing and returning games.

### Conclusion

This project showcases the end-to-end process of data cleaning and visualization,
providing valuable insights into the board game borrowing activities at the Kids Game Day event.

## License

This project is licensed under the Creative Commons Zero (CC0) License. 
This means you can copy, modify, distribute, and perform the work without asking permission.
For more information, please visit the [Creative Commons website](https://creativecommons.org/publicdomain/zero/1.0/).

