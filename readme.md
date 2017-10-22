# Inroduction
This Project use minicap and tornador implements an android screenshare web app.
tornador is a excellent python library with async io feature, kind of like nodejs. It can be used as a stand alone web server or as an async io library. This project used it in both way.
Server side:
    An web server implemented with tornador, it read image uploaded from device, and deliver the same image to web page. The connection between server and device is an tcp connection, while the connection between web page and server is websocket and normal http.

Client side:
    include two participant: web page user intende to view device screen, and local device screen capture program run on a computer which is connecting to an android device.
    web page is an simple html page, include some js code to trigger an websocket connection.
    local side is implemented with tornador and minicap library. minicap is also an open source library for android testing, it can get screencap from android with a relativly high speed, up to 10+ per second.

