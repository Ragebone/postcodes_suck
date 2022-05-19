# POST codes suck!


##  What are POST codes? 
POST codes are hexadecimal numbers that change throughout the startup and boot process of a computer and server. 
They come in two varieties: 
Checkpoint or Progress and Error Codes.

The first change on reaching a certain point of the process that can be compared to mile or section markers on a highway. 
Error codes are only set once and as the last code to indicate the detection of an error or fault.
Usually those faults prevent the system from further progression of the process and reaching the Bios or OS.

Those codes get set by the systems firmware aka Bios and are dependent on and specific to that firmware and its developer. 

TODO Explain the bus and port they get send on. 
TODO explain where the meaning can be found
TODO explain that its more then just two digits. 

Commonly they get displayed through two or more 7 segment LED indicators on the motherboard.

## Why they suck
POST codes as they are now suck for multiple reasons.

### No indication of an ERROR Code
Commonly, there is no way to identify the shown code as an Error code.

### Reuse of the LED display for CPU temperature
Some higher end Desktop motherboards use those LED displays to display the CPU temperature.
The point at which they do that, is usually not indicated in any way.

If a problem occurs that late in the process, there is no way to figure out what the problem is. 
One my waste time looking up nonsensical codes that are temperatures instead.
Why the fuck is my system stuck before the Bios at code 33? 

### Reuse of codes
For some reason, codes can appear multiple times throughout the process with different meanings.
There usually is no indicated way to differentiate between those.

One reason for this on AMD Zen based systems is that their codes are up to 8 digits long with clear differences between codes and as well as codes usually being unique.
All of that gets discard when only two digits are displayed.

### Unreliable display of codes
Most servers and even some desktops display the current postcode in a corner of the Monitor once it displays a picture.
There might be additional information on what the system is currently doing including clearer error messages and progress outputs.

From recent experience i can say that both can lack substantially behind what the system is displaying through other means.
That can be very confusing, is the problem now indicated by code B0 or code 53?

### Ambiguous meaning of codes
Reading through most published lists of codes and their meaning leads to nothing concrete.
In the worst case they are wrong and absolutely useless. 

### Quick changes of codes
Codes may change quicker then they can be displayed.
To rule out issues with for instance the installed Memory, one can look for codes expected to occur before during and after that step in the process.

But the displayed codes can change quick enough that it is impossible to distinguish between individual codes and codes shown between power-on and the issue code occurring.
For example, a system might power on, quickly go through a number of codes and then get stuck on a code like A2.
One could look for the occurrence of known memory training codes with the ability to rule out obvious memory issues once the last of those codes was seen.

A history of codes would also allow for that.
If there were a history, or the history were explained and usable.

