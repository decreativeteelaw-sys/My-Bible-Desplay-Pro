# **Bible Display Pro**

An offline-first KJV Bible presentation tool designed for use with OBS Studio. It allows you to search, preview, style, and display Bible passages during live presentations.

## **Important: GitHub Pages vs. Local Hosting**

Bible Display Pro uses a local Python server to communicate between the controller and the OBS display.

**GitHub Pages cannot run this application by itself.** GitHub Pages is designed for static websites. It cannot run the Python server or the local WebSocket communication required by Bible Display Pro.

GitHub is still useful for:

- Storing and managing the project's source code.
- Keeping backups and tracking changes.
- Sharing the project with others.
- Distributing downloadable releases.

The application should run locally on the Windows computer connected to OBS Studio.

## **Requirements**

- Windows computer
- Python installed
- OBS Studio
- Internet connection for the initial download of the KJV database and fonts

After the required database and fonts have been downloaded, the application is designed to work offline.

## **Quick Start**

1. Download or extract the project folder.
2. Open the extracted folder.
3. Run `start.bat`.
4. Allow the setup process to complete.
5. Open the controller using the provided launcher.

The local application addresses are:

**Controller:**\
`http://127.0.0.1:8765/index.html`

**OBS Browser Source:**\
`http://127.0.0.1:8765/output.html`

Keep the local server running while using the application.

## **Features**

- KJV Bible search.
- Search by book, chapter, verse, or keyword.
- Previous and next verse navigation.
- Display individual verses or verse ranges.
- Preview passages before displaying them.
- GO LIVE control positioned beside the passage search area.
- Transparent Bible output for OBS.
- Customizable text appearance and positioning.
- Saved presentation styles and presets.
- Local Bible database storage.

## **First-Time Setup**

The ZIP package contains setup scripts but does not include the complete KJV database or downloaded font files.

The setup scripts are provided to obtain the required resources during the initial setup.

If the Bible database is missing or damaged, run:

`Repair_KJV_Database.bat`

## **Project Structure**

- `index.html` — Main controller interface.
- `output.html` — OBS display page.
- `server.py` — Local application server.
- `assets/app.js` — Controller functionality.
- `assets/output.js` — Scripture output functionality.
- `assets/style.css` — Application styling.
- `assets/fonts.css` — Font configuration.
- `start.bat` — Application launcher.
- `Open_Controller.bat` — Opens the controller.
- `Open_Output_Test.bat` — Opens the output test page.
- `setup_kjv.py` — KJV database setup.
- `setup_fonts.py` — Font setup.
- `validate_kjv.py` — Database validation.

## **Important Notes**

- Use the controller and OBS on the same Windows computer.
- Do not close the local server while presenting.
- Use the GO LIVE button to send the prepared passage to the OBS output.
- The OBS output is designed to have a transparent background.

## **Project Status**
**Note:** I reconstructed this from the README content and project details available in our previous discussion. I couldn't access the earlier temporary file itself, so I can't guarantee this is a byte-for-byte copy of that original draft.
