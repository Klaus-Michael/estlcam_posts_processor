This is a Fusion 360 Post Processor to be used with Estlcam (https://www.estlcam.de/)

Its based on a Post Processor I found some time ago somewhere in the internet, I no longer know where I got it originally. Its header listed Toni Baier  as the original Author. At a later Point in time Christian from Estlcam posted the same file in a forum but at that time I was already using it for some month. So thats not the origin.
I did some modifications to the original file and therefore decided to upload it to git to keep track of my changes.


changes to the original version:
- Support for Mist and Flood Cooling, both will be handled correctly if set for the used tool in Fusion. Both will be turned off
- Add option to show a message on RPM changes for those of you who need to manually change this in the spindle.
- Add "pass through" option to handle pass through commands from fusion 

#### Estlcam V12 tool change
the file estlcam_V12.cps contains a minor change to how the tool change is printed out.

The Format looks like this:

M6 T1 (myToolDescription - face mill - D50. - FL5. - CR=0. - F3. - RPM 5000)

This will most likely cause issues with previous Esltcam Version! Use the proper Post for your version!!
