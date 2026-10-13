FILM & MEDIA HOMEWORK PORTAL — LOCAL VS CODE VERSION
====================================================

This version does NOT use Supabase, APIs, subscriptions, or a backend.
It is a local prototype that you can open and edit using Visual Studio Code.

OPEN IT
-------
1. Extract this ZIP to a folder, for example Desktop\vscode-homework-portal.
2. Open Visual Studio Code.
3. Choose File > Open Folder and select the extracted folder.
4. Open index.html and use your browser to open it. Recommended: install the free
   VS Code extension called Live Server if you want automatic refresh, but it is optional.
5. Use the Teacher access button on the page.

DEFAULT TEACHER LOGIN
---------------------
Teacher ID: teacher
Password: ChangeThis123!

Change these in js/config.js before using the teacher screen:
  teacherId: "teacher",
  teacherPassword: "ChangeThis123!",

LOGO / BRANDING
---------------
1. Put your logo file in the assets folder, for example assets/my-logo.png.
2. Open js/config.js.
3. Change logoPath to "assets/my-logo.png".
4. Change brandName to your preferred name.
The logo file can be PNG, JPG, SVG, or WebP supported by your browser.

BATCHES AND CLASSES
-------------------
- Initial batch: PVE 2606
- It initially has 0 unlocked classes. The teacher can unlock classes in Batch management.
- Students enter only their batch number, no student password.
- There are 29 class slots in Homework library.
- Teachers can add batches, change unlock limits, activate/deactivate batches, and edit lesson details.
- Each lesson can contain text and links to PDFs/images/videos. This version does not upload files.
- Export a JSON backup from Teacher access > Settings & backup before changing computers.

IMPORTANT LIMITATIONS — PLEASE READ
----------------------------------
This version is intentionally simple and local-only:
- Data is stored in the current browser's localStorage, not in a shared online database.
- A batch/lesson edit on your computer will NOT automatically appear on a student's phone/computer.
- Teacher ID and password are in js/config.js and can be seen by anyone who can inspect the website files.
- Batch unlock rules are client-side and can be bypassed by a technically skilled student.
- Students on different devices cannot share a central dataset without some kind of server or hosting/data service.

Therefore use this version to build and test the design and workflow locally. To share the portal online
with real students and have central batch controls, some hosting/server or managed data service is
unavoidable. This package does not pretend otherwise.
