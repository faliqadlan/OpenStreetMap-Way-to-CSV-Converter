# OpenStreetMap Way to CSV Converter (Google Colab)

A simple yet powerful Google Colab notebook to download geographic data for specific **'ways'** (like roads, paths, or building outlines) from the OpenStreetMap (OSM) API and save the coordinates of all constituent points (nodes) into a clean, easy-to-use CSV file.

This tool runs entirely in your browser, so no local Python installation is required. It's designed to be accessible for everyone, including users with **no programming experience**.

[![Run in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/faliqadlan/OpenStreetMap-Way-to-CSV-Converter/blob/main/OSM_API_to_CSV_Converter.ipynb)

---

## Key Features

-   **Runs in Your Browser**: No setup needed, thanks to Google Colab.
-   **Easy to Use**: Just edit a single list in the code cell to input the OSM Way IDs you want to process.
-   **Batch Processing**: Download data for multiple ways in a single run.
-   **Descriptive Filenaming**: Automatically names the output CSV file using all the way's tags and its unique ID (e.g., `highway_path-name_Some_Trail_12345_nodes.csv`).
-   **Informative Output**: See progress and information about each way as the script runs.

---

## How to Use (Step-by-Step Guide)

Follow these steps to get your CSV files.

### Step 1: Find the OSM Way ID

1.  Go to **[www.openstreetmap.org](https://www.openstreetmap.org/)**.
2.  Search for a location and find the road, path, park, or building you are interested in.
3.  Click on the feature. The details will appear in a panel on the left.
4.  Make sure it says **"Way"** at the top to confirm you've selected the right type of object.
5.  The **Way ID** is the large number shown right below the word "Way".

<img width="1755" height="848" alt="image" src="https://github.com/user-attachments/assets/32693451-7908-4299-b62d-57bc8683bb95" />

### Step 2: Open the Notebook and Add IDs

1.  Click the **"Run in Google Colab"** button at the top of this README.
2.  The notebook will open. Find the code cell titled **"Process OpenStreetMap Way IDs and Generate CSV Files"**.
3.  Locate the list named `way_ids_to_process` at the very top of that cell.
4.  Edit the list to include the Way ID(s) you found. Make sure each ID is a string (inside quotes `""`) and separated by a comma.

**Example:**

<img width="607" height="158" alt="image" src="https://github.com/user-attachments/assets/bf69d0a6-62d8-4afb-a965-0ffc4d63167b" />

### Step 3: Run the Code

1.  Run the code cell by clicking the "play" button next to it or by pressing **`Shift` + `Enter`**.
2.  The script will now fetch the data and create your files, printing its progress below the cell.

### Step 4: Download Your Files

1.  Once the script finishes, look at the left sidebar in Google Colab and click the **folder icon** 📁.
2.  Your new `.csv` files will be listed there.
3.  Click the three dots (**⋮**) next to each filename and choose **Download** to save it to your computer.

<img width="442" height="296" alt="image" src="https://github.com/user-attachments/assets/0378ce8b-6d40-4026-b9b6-2e713180da59" />

---
