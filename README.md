# picture_metadata
The provided notebook script orchestrates a multi-step process to download an image, extract metadata, and save the metadata. Here is a summary of what each part of the script achieves:

Logging Configuration:

Sets up logging to a file in the /dbfs/tmp/logs directory.
Ensures the log directory exists and creates a log file with a timestamp.
Step 1: Download Image Data:

Runs the Download_Image_Data notebook to download the latest image file from a specified container.
Logs the path of the downloaded image data.
Handles any exceptions that occur during the notebook run.
Step 2: Extract Metadata:

Runs the Extract_Metadata notebook to extract metadata from the downloaded image.
Passes the imageDataPath to the notebook.
Logs the extracted metadata.
Handles any exceptions that occur during the notebook run.
Step 3: Save Metadata:

Runs the Save_Metadata notebook to save the extracted metadata.
Passes the metadata and imageDataPath to the notebook.
Handles any exceptions that occur during the notebook run.