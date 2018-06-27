# The Proposal
This is just my vision for what I'd love to see openpilot look and how it should work in future versions of the system.  This is unofficial and not affiliated with Comma.ui, Inc.

## Todos
- [ ] openpilot is [ready|not ready]
  - [ ] ready screen
    - [x] create & present basic concept
    - [ ] add additional state information on the left / right of the start button (within reason)
      - [ ] display any accessories / modules that it detects in the CAN with icon
        - [ ] create & present concept showing the Comma Pedal being detected for instance
        - [ ] future versions might need to show status of external cameras, sensors, etc.
  - [ ] not ready screen
    - [ ] show reasons, make it obvious that something is wrong
    - [ ] have options to expand out more information about what happened
    - [ ] suggest reasons why it may have happened
- [ ] connect eon to panda
  - [x] create & present basic concept
  - [ ] ideally would have additional states as well
  - [ ] should transition to a (possibly green) connected screen, maybe even animate the connection happening, possibly audible sound, then dump into the `openpilot is ready` screen
- [ ] drive
  - [ ] engaged
    - [ ] create & present basic concept
  - [ ] disengaged
    - [ ] create & present basic concept
- [ ] settings
  - [ ] shows fingerprint detected
    - [ ] drills down into which CAN information is labeled in opendbc possibly?
    - [ ] possibly have ON/OFF or GREEN/RED UI state when those things are detected

## Thoughts & Ideas
### Boot
This is only shown when EON powers on and openpilot is starting. 
It's pretty much the same as the original.

### Global UI
The `overlay` image is the text overlayed over the entire OS.
The large text at the bottom can be called upon at any time to display state.
It should be a singleton.

Anytime we need some text shown to the user, we can use this area.

### Uploading your drives
This is kind of a redesign of the existing "Home screen" but is only shown when it is currently uploading your drives.

### Connect EON to Panda
This screen is shown whenever you're not uploading and you're not connected to a vehicle.
I envision an abstract icon-like version of the panda plugging into an abstract icon-like version on the EON via a nice and clean white USB cable.  Could even be animated.

### Openpilot is ready
Will be shown after EON is connected to Panda and it is paired without errors.
It goes away when you start your engine.

The bubble at the top would be used to display the linked fingerprint.
This is mainly just for "looks" but also reassures the user that a fingerprint has been found in better UX-y way... that's like sexy but UX.

### Openpilot is not ready
Will be shown when there were errors, or services did not quite start.
Possibly could show exceptions that were thrown during initialization.

### Drive
This screen will be the overlay / HUD related information that will be shown during drives and engagements.

It doesn't need a video output anymore, it could just be some sort of HUD information about speed, lane tracking status indication, GPS information, whether we're on an HD Mapped Route for instance might be nice, etc.

#### Drive / Engaged
TBD
#### Drive / Disengaged
TBD
#### Drive / Error
TBD

## Contributing
To contribute, you are welcome to load the `.fig` file on your computer and save changes back to that `.fig` file and commit it up in a pull request.

I'm also open to doing live design sessions in Figma with others that are interested in contributing and see what we can come up with together.