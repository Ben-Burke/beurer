# Beurer interconnects for Chrome web-bluetooth

This repo contains javascript code to interface with various Beurer devices. At the time of writing, we support the PO60 and FT95

There are no examples provided by Beurer - only a couple of protocol descriptions (which are included in this repo). 

A certain amount of guesswork has been required to implement the basic functions required by a project we are working on. 

In brief, those requirements are to pull in a single 'result' from each device as a part of a larger set of medical 'tests'.

It would seem that the Beurer devices are not really designed for this. For example, the PO60 transmits up to 10 'results' at a time. The data structure returned is larger than the BLE standard 20 byte array, which alings with the Javascript Uint8Array.

This is a placeholder for publicly shared code
