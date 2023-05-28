the heading of a bash script should always include:
   
						#!/bin/bash

that is how the shell knows how to run the script.


echo  :is used to print words directly to the screen

variable="NAME"  :is th e way to declare variables 

use $ in front of variables to avoid name collision. also its mandatory.

For example:  $variable   will print out the word NAME

in order to send the output of a command to a a variable use

VARIABLE=$(COMMAND)

$() allows command to be rum in the background (sub shell)















