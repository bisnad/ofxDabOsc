## ofxDabOsc

**Author**: Daniel Bisig - Coventry University, UK - [ad5041@coventry.ac.uk](ad5041@coventry.ac.uk) - Zurich University of the Arts, CH - [daniel.bisig@zhdk.ch](daniel.bisig@zhdk.ch)

**Dependencies**: [ofxDabBase](https://bitbucket.org/dbisig/ofxdabbase_011/src/master/), [oscpack](http://www.rossbencina.com/code/oscpack) (included)

---

## Summary

ofxDabOsc provides functionality for sending and receiving OSC messages. This addon makes heavy use of OSC blobs for handling large number of values. To specify and communicate the value types contained in a blob. the addon extends the standard OSC message format by introducing additional tags. In addition, the addon can also handle the sending and receiving of data that exceeds the amount of data that can fit into a single OSC message. For this purpose, the addon automatically splits large messages into multiple messages before sending, and fuses multiple messages into a single message after receiving. The code is compatible with OpenFrameworks 0.11 and has been tested on Windows and MacOS. The following classes are available.

**OscArg**: a wrapper for an array of values of arbitrary data type.

**OscMessage**: an OSC message that supports type tags for Blobs

**MultiOscMessage**: an OSC message that is bigger than a regular message and constructs itself from or into multiple smaller messages.

**OscSender**: a sender for OSC messages

**OscReceiver**: a receiver for OSC messages

**OscMessenger**: master class that manages all OSC senders and receivers