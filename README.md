WebRTC Voice Chat Application with Admin and User

This application allows USER (customer) to connect with an ADMIN (Virtual Agent/ service provider) for a voice chat via WebRTC. The application includes login functionality for both admin and users, call initiation, and call termination features.

Features
Admin and User Login: Admins log in with a specific ID, while users can log in without an ID.
Voice Call: Users can initiate a call that connects directly to the admin. [[[condition: iff admin is available on server]]]
Call Control: Both users and admin can end the call at any time.

Workflow

Admin Login:

Admin clicks the "Admin Login" button.
Admin enters their ID (admin123).
Admin's microphone access is requested and enabled.
Admin is marked as available for calls.
User Login:

User clicks the "User Login" button.
User is notified if the admin is available.
Start Call and End Call buttons are enabled.
Starting a Call:

User clicks the "Start Call" button.
User's microphone access is requested and enabled.
WebRTC connection is established, and an offer is sent to the admin.
_ NOTE: Call connects if and only if the admin is available to take calls (i.e. admin should be logged in)_
Handling the Call:

Admin receives the offer, creates an answer, and establishes the connection.
Only User can initiate the call

Ending the Call:

Either the user or the admin can end the call by clicking the "End Call" button.
WebRTC connection is closed, and audio streams are stopped.

**Deployed Link of the following Application : ** https://webrtc-admin.onrender.com
