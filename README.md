
#### Building the C version  gstwebrtc demos on TEGRA machine

* Build the sources in the `gst/` directory on your TEGRA machine. Use `make` or
$ gcc webrtc-sendrecv.c $(pkg-config --cflags --libs gstreamer-webrtc-1.0 gstreamer-sdp-1.0 libsoup-2.4 json-glib-1.0) -o webrtc-sendrecv
```

#### Run Browser and C version gstwebrtc demos

* Open http://122.112.211.178:8080 from browser, a page shall show with Our id is `ID`

* Run `./webrtc-sendrecv --config=CONFIG_FILE --peer-id=ID` with the `CONFIG_FILE` of the name of config file ( there is a sample config file in the folder )
  with the `ID` from the browser. You will see state changes and an SDP exchange.

