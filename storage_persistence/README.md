This is the chrome App used for testing webview Tag's storage persistence. To
use this app, first host the 'page.html' file on one or more local ports.
  python -m SimpleHTTPServer 9000
  python -m SimpleHTTPServer 9001

Then inside the app, provide the port for Pre Test and Test.

During Pre Test, the app will write some cookies on various types of paritions
(un-named, named, persistent - shared, persist).

Then, close the browser, and re-open and start the app but this time, run the
Test on some port where the page is hosted. It should pass. To see the log,
check console.
