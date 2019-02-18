# "How-to" for creating a proper config file (Client.cuo) with ConfigurationEditor.exe

# Main

![main](http://www.imageup.ru/img206/2570280/ce1.png)

1) Client version which'll be sent to your server. When you're typing a version number, configurator searches for matches and picks right encryption keys, stadart map sizes and verdata usage flag when there's a match. After you've entered your desirable client version, you can edit those values manually.

2) Client's encryption type.

No Crypt - No encryption.

Old Blowfish - For truly ancient client versions only.

Blowfish (1.25.36 client) - This version only encryption.

Blowfish - For client up to 2.0.0 versions (with the exception of the above one).

Blowfish + Twofish (2.0.3) - For 2.0.0 - 2.0.3 clients.

Twofish - For clients above 2.0.3

3) Version of clients protocol. This toggles on/off different packet changes which EA's made over the years. This should correlate with client version.

For example:

If your client version is 2.0.3 - protocol version should be >= 2.0.0

Client version 4.0.3b - client protocol version >= 4.0.0b (because client version is lower than 4.0.5a)

Client version 6.0.14.1 - client protocol version >= 6.0.6.0 (minor's patch version lacked 1 to make 6.0.14.2 viable)

Client version 6.0.14.2 or 6.0.14.3 - client protocol version >= 6.0.14.2

Client version 7.0.29.2 - client protocol version >= 7.0.24.0

4) Manual crypto key input. Use  this only if you have changed encryption keys on your server and you know what you're doing. 

5) Text input for crypto keys.

6) Map size.

7) Client type. At this moment this is only being sent the server when creating a character.

8) Toggle to make OrionUO read (Verdata.mul) and *.mul files only. If you're willing to use latest client versions which contain *.uop files, you need to toggle this off.

9) Create file with current config. It will be created in the same directory with this exe.

10) Load config file.



## Plugin

![plugin](http://www.imageup.ru/img204/2562847/ce2.png)

1) List of enabled plug-ins.

2) Plug-in file name.

3) Main function from the dll to trigger the install.

4) Available functions for data transfer between client and server.

5) Create plug-in with current config.

6) Refresh selected plug-ins config.

7) Delete selected plug-in.