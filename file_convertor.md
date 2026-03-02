## Design file convertor

### Functional Requirements
- User uploads a video file strictly in (.mp4, .mkv) format and system converts it into audio file in (.mp3 or .wav) format.
- Once processed, user must be able to securely download the converted file.
- User should see clear states of file upload, processing and download. If any error occured will see clear error message.
- For access control, unauthenticated or guest users will be restricted to uplaod a file upto 10mb limit.
- For data lifecycle management to control storage cost. We enforce a strict 24-hour retention policy where both uploaded and
  downloaded file will be permanently deleted.
- Optional - support for uploading multiple files at a time.
  
### Non Functional Requirements
- High Availability: Our frontend API and upload ingestion server must be highly available to server user.
- Scalability: System needs to support high throughput, handles thousands of concurrent users can upload files at a time.
- Fault tolerance: Once file is uploaded successfully, it must be processed even after server restart.
- Large file processing should not block small file processing --> one 5GB file should not block nine 100mb file processing

### System Design

<img width="2838" height="1977" alt="image" src="https://github.com/user-attachments/assets/ba1ad815-97e0-4a37-ab9f-ba6a83b41b3c" />
