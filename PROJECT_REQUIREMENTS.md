# Project Requirements

## Business Requirements

Build a simple appointment scheduling website similar to Doodle.

## User Requirements

Users should be able to:

- View existing appointments on a main schedule overview.
- Create an appointment with a title, description, and time.
- Delete an appointment directly from its details view or schedule view.
- View an individual appointment through its own direct URL.
- Search or filter appointments by matching keywords in the appointment notes or organizer name.
- View external calendar invites or event links submitted with an appointment.
- Upload and view a plain text or image attachment (such as an agenda or flyer) linked to an appointment.

The application should display an informative status message when an appointment cannot be found, reflecting the requested identifier back to the user for reference.

## Software Requirements

- Python 3
- Flask
- SQLite
- HTML and CSS
- NO JavaScript
- Do not use React, Node.js, or any JavaScript framework
- Store appointments and event records in a SQLite database.
- Use lightweight, native Python string handling and standard library utilities where possible; avoid heavy third-party ORMs or complex security plugins.
- Each appointment must have an identifier provided directly through the URL path or query parameters (e.g., `/appointment/<id>` or `/appointment?id=<id>`).
- Provide a direct deletion for link clicks (e.g., `/delete?id=<id>`) so users can discard unwanted test events.
- Render all user-submitted text fields (titles, notes, agenda files, and error references) directly into the Jinja2 HTML templates.
- Any uploaded file attachments should be saved to a local folder and retrieved directly via a simple file retrieval route (e.g., `/files?name=<filename>`).
- The application must run inside GitHub Codespaces.
- The application must be accessible through a web browser using the Codespaces forwarded port.
