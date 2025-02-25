# log-viewer
The Log Viewer will allow users to upload, parse, filter, and display logs in a structured way. Logs could come from server applications, APIs, or general system logs.

## Core Goals:

✅ Read and parse log files efficiently.
✅ Display logs in a structured, easy-to-read format.
✅ Implement filtering (e.g., search by date, severity, keyword).
✅ Provide a simple UI for users to upload and view logs.
✅ Store logs in SQLite/PostgreSQL for persistence.

## Project Breakdown
### Define Scope & Set Up Project

✅ Goals:

    Plan out the Log Viewer’s features & functionality.
    Initialize the project folder structure.
    Set up the Go project with dependencies (go mod init).

✅ Tasks:

    Define how logs will be formatted (e.g., timestamp | severity | message).
    Sketch a rough UI wireframe (file upload button, log table, filters).
    Set up main.go and dependencies like gin (for backend) and gorm (for DB).

📌 Deliverable: Project is initialized & scope is well-defined.

### Handle File Uploads

✅ Goals:

    Enable users to upload log files (.txt, .log).
    Store logs temporarily before processing them.

✅ Tasks:

    Implement a backend endpoint (/upload) to accept log files.
    Parse the uploaded file and extract log entries.
    Display raw logs in the UI.

📌 Deliverable: Users can upload a log file, and it appears in the UI.

### Parse and Structure Logs

✅ Goals:

    Process log files and store structured log entries in SQLite/PostgreSQL.

✅ Tasks:

    Create a database schema for logs (e.g., id, timestamp, severity, message).
    Write Go functions to parse logs and extract relevant fields.
    Store extracted logs in the database.
    Implement error handling (e.g., invalid log formats).

📌 Deliverable: Logs are now structured and stored in a database.

### Build the UI

✅ Goals:

    Create a simple frontend to display logs.

✅ Tasks:

    Set up an HTML template with a table layout for logs.
    Display stored logs in the UI.
    Add a basic CSS layout for a clean design.

📌 Deliverable: Users can see structured logs in the UI instead of raw text.

### Implement Filtering & Searching

✅ Goals:

    Allow users to filter logs by date, severity, or keyword.

✅ Tasks:

    Implement search functionality (search by message).
    Add date filtering (e.g., logs from last 24 hours).
    Add severity filtering (INFO, WARNING, ERROR).

📌 Deliverable: Users can now filter logs dynamically in the UI.

### Final Touches & Performance Optimization

✅ Goals:

    Improve log loading performance and UI responsiveness.

✅ Tasks:

    Optimize database queries for better performance.
    Implement pagination (load logs in chunks instead of all at once).
    Improve UI with loading spinners and clean error messages.

📌 Deliverable: A faster, more user-friendly Log Viewer.

### Testing & Wrap-Up

✅ Goals:

    Test the entire system and fix bugs.
    Record content for social media.

✅ Tasks:

    Test log parsing with different file formats.
    Fix UI bugs and refine styling.
    Record a recap video showing how the Log Viewer works.

📌 Deliverable: Final working Log Viewer ready for deployment & content creation.
