# Crowdsource server

This subdirectory contains a simple server for the radarhub plugin written in python. This server implements the full protocol, but just dumps all received tracks to disk in geojson format. It can be used as a simple shore based VDR, but mostly serves as an example base for anyone wanting to build a more elaborate server side setup.

To run it:

```
virtualenv myenv
source myenv/bin/activate
pip install -r requirements.txt
python server.py
```

Note that the server uses a relative path to open the avro protocol specification file, and so relies on this subdirectory being the current directory when run.
