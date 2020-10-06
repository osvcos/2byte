# 2byte

2byte is a tool developed in python whose to convert an array of hex characters (05 0a 70 89 ...) and give a file as an output, composed of the bytes represented by that array. The array of bytes can be the ones seen in a hex editor.

## Uses

There are two ways in which 2byte can be used:

### Input from file

In this case, you have an array of bytes, you copy and paste those in a new file, you name that file bytes.txt, and the you execute:

    2byte bytes.txt output.raw

### Input from clipboard

In this case, you copy an array of bytes to your system's clipboard, and then execute:

    2byte --from-clipboard output.raw

2byte access the clipboard through native binaries (subprocess). Currently Linux (X11), macOS and Windows (not tested) are supported.
