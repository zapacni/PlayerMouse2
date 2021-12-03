# PlayerMouse2 Documentation

Welcome to the PlayerMouse2 documentation!
PlayerMouse2 is an elegant, modern alternative to the PlayerMouse.

## Properties

### Delta: Vector2
Describes the change in the mouse position since the last frame. Only works if mouse is locked in place.

### Hit: CFrame
Describes a `CFrame` of the mouse position in the 3D world. This property respects the `TargetFilter`.

### IconEnabled: boolean
Describes a boolean that determines if the mouse icon is enabled or not.

### Normal: Vector3
Describes the surface normal the mouse is on, as a Vector3. Returns a blank identity Vector3 if there is no `Target`.

### Origin: CFrame
Describes a CFrame that starts at the camera's `CFrame.Position` that orients towards the mouse's `Hit.Position`.

### Position: Vector2
Describes the 2D coordinates 

### Sensitivity: number
Describes the delta sensitivity of the mouse

### Target: BasePart?
Describes the part the mouse is currently hovering over. Nil if pointing at the sky/an ignored part.

### TargetFilter: { Instance }
Describes a list of instances to ignore. Ignores the `Player.Character` by default.

### UnitRay: Ray
Describes a unit ray positioned at the camera directed towards the mouse's `Hit.Position`.

### MaxTargetDistance: number
Describes the maximum distance the mouse can reach. Default value is 1000.

## Events

### LeftPressed()
Fires when the left mouse button is pressed.

###	LeftClicked()
Fires when a full left mouse button click is finished.

###	LeftReleased()
Fires when the left mouse button is released (fires after `LeftClicked`).

###	RightPressed()
Fires when the right mouse button is pressed.

###	RightClicked()
Fires when a full right mouse button click is finished.

###	RightReleased()
Fires when the right mouse button is released (fires after `RightClicked`).

###	Moved(delta: Vector2)
Fires when the mouse moves, and passes the mouse delta as an argument to its listeners.

###	WheelScrolled(direction: number)
Fires when the mouse wheel is scrolled, and passes the scroll direction as an argument to its listeners (1 = scroll up, -1 = scroll down).

###	WheelReleased()
Fires when the mouse wheel is released.

###	WheelClicked()
Fires when a full mouse wheel click is finished.

### WheelPressed()
Fires when the mouse wheel is pressed.
