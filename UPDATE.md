####1.6.4 27.03.2016
Fixed constructor of Template class did not load the source file properly. Template loader and cache were not affected.

####1.6.3 11.03.2016
Fixed a compilation error.
Added missing implementation of HttpRequest::getPeerAddress().

####1.6.2 06.03.2016
Added mime types for some file extensions.

####1.6.1 25.01.2016
Fixed parser of boundary value in multi-part request, which caused that QHttpMultipart did not work on client side.

####1.6.0 29.12.2015
Much better output buffering, reduces the number of small IP packages.

####1.5.13 29.12.2015
Add support for old HTTP 1.0 clients.
Add HttpResponse::flush() and HttpResponse::isConnected() which are helpful to support SSE from HTML 5 specification.

####1.5.12 11.12.2015
Fix program crash when using SSL with a variable sized thread pool on Windows.
Changed name of HttpSessionStore::timerEvent() to fix compiler warnings since Qt 5.0.
Add HttpRequest::getRawPath().
HttpSessionStore::sessions is now protected.

####1.5.11 21.11.2015
Fix project file for Mac OS.
Add HttpRequest::getPeerAddress() and HttpResponse::getStatusCode().

####1.5.10 01.09.2015
Modified StaticFileController to support ressource files (path starting with ":/" or "qrc://").

####1.5.9 06.08.2015
New listen() method, to restart listening after close.
Add missing include for QObject in logger.h.
Add a call to flush() before closing connections, which solves an issue with nginx.

####1.5.8 26.07.2015
Fixed segmentation fault error when closing the application while a HTTP request is in progress.
New HttpListener::close() method to simplifly proper shutdown.

####1.5.7 20.07.2015
Fix Qt 5.5 compatibility issue.

####1.5.6 22.06.2015
Fixed compilation error if Qt does not support OpenSsl.

####1.5.5 16.06.2015
Improved performance of SSL connections.

####1.5.4 15.06.2015
Support for Qt versions without OpenSsl.

####1.5.3 22.05.2015
Fixed Windows issue: QsslSocket cannot be closed from other threads than it was created in.

####1.5.2 12.05.2015
Fixed Windows issue: QSslSocket cannot send signals to another thread than it was created in.

####1.5.1 13.04.2015
Add support for pipelining.

####1.5.0 03.04.2015
Add support for HTTPS.
...

####1.4.0 14.03.2015
Add support the creation of a shared library (*.dll or *.so).
...

####1.3.0 20.04.2013
Add support for logging source file name, line number and function name.
...

####1.2.0 05.12.2010 
Add a controller that serves static files, with cacheing.
...

####1.1.0 19.10.2010
Add support for sessions.
...

####1.0.0 17.10.2010
First release
