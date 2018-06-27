# openpilot ui proposal
This is just my vision for what I'd love to see openpilot "look" like and how it should work.

## Screens

### Boot
This is only shown when EON powers on and openpilot is starting. 
It's pretty much the same as the original.

### Uploading your drives
This is kind of a redesign of the existing "Home screen" but is only shown when it is currently uploading your drives.

### Connect EON to Panda
This screen is shown whenever you're not uploading and you're not connected to a vehicle.

### Openpilot is ready
Will be shown after EON is connected to Panda and it is paired without errors.
It goes away when you start your engine.

### Openpilot is not ready
Will be shown when there were errors, or services did not quite start.
Possibly could show exceptions that were thrown during initialization.

### Drive
This screen will be the overlay / HUD related information that will be shown during drives and engagements.

It doesn't need a video output anymore, it could just be some sort of HUD information about speed, lane tracking status indication, GPS information, whether we're on an HD Mapped Route for instance might be nice, etc.

#### Drive / Engaged
#### Drive / Disengaged
#### Drive / Error


## Contributing
To contribute, you are welcome to load the `.fig` file on your computer and save changes back to that `.fig` file and commit it up in a pull request.

I'm also open to doing live design sessions in Figma with others that are interested in contributing and see what we can come up with together.