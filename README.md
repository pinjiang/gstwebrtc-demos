
#### Running the C version

* Build the sources in the `gst/` directory on your machine. Use `make` or

```console
$ gcc webrtc-sendrecv.c $(pkg-config --cflags --libs gstreamer-webrtc-1.0 gstreamer-sdp-1.0 libsoup-2.4 json-glib-1.0) -o webrtc-sendrecv
```

* Run `./webrtc-sendrecv --config=CONFIG_FILE --peer-id=ID` with the `CONFIG_FILE` to config file, there is a config file in the folder
  with the `ID` from the browser. You will see state changes and an SDP exchange.

