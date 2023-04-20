[Ressurected] BlueChat (AKA Fire Chat)
======================

Bluetooth instant messaging app for Android, 



How it works:
  - To send messages and images, we transmit them in formatted byte arrays in the following format:
      <blockquote>
      [ Message Type, Sender Name Length, ...Body Length**..., Sender ID, Sender Name, Body ]
      </blockquote>
      
    ** The Body Length is separated into tens digits (from least to most significant digit) just in case the body length exceeds the size of a byte.

Notes:
  - If having connection problems, make sure the host creates a room before a client tries to join 
  - Make sure Higher API Level (Higher Android Version) Creates the Room.
  
Current Bugs:
  - Sometimes quitting and rejoining a chatroom is a bit buggy (Fixed)
  - Sometimes rooms made by lower API cannot be joined by higher API. Workaround - Make sure Higher API Level (Higher Android       Version) Creates the Room.


