# Youtube Video Uploader from AWS S3 Using Python
This code is a script for uploading videos from AWS S3 to YouTube using Python.

## Prerequisites
- A project in the Google Developers Console with the YouTube Data API v3 enabled
- A YouTube channel
- An IAM user with necessary permissions to read and list objects in your S3 bucket
- AWS Access Key and Secret Key
- S3 Bucket name
## Installation
1. Clone this repository
```
git clone https://github.com/Elton997/youtube-video-upload.git
```
2. Install the required dependencies
```
pip install -r requirements.txt
```
## Usage
1. Replace the following placeholders in the code with your own credentials:
```
"client_id": "YOUR_CLIENT_ID",
"client_secret": "YOUR_CLIENT_SECRET",
"refresh_token": "YOUR_REFRESH_TOKEN",
"aws_access_key_id": "YOUR_AWS_ACCESS_KEY",
"aws_secret_access_key": "YOUR_AWS_SECRET_KEY",
"Bucket":"YOUR_S3_BUCKET_NAME"
```
2. Run the script
```
python3 video_uploader.py
```
3. The function upload_video_to_youtube(video_file_name, video_title, video_description) takes in three arguments:
- video_file_name: The name of the video file in S3.
- video_title: The title of the video on YouTube.
- video_description: The description of the video on YouTube.

## Note
The script will upload the video with unlisted privacy status.

## Disclaimer
This script is for demonstration purposes only and should not be used in production without proper testing and modification to fit your use case.

## Author
Elton Dcunha

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License.
