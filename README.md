## Transport Mode Macro Summary

This set of macros is designed to secure your printer for transport and manage the transport mode efficiently. It includes features for setting, resetting, and checking the transport state, with optional LED/Neopixel feedback.

### Features:
1. **Transport Position Macro (`TRANSPORT_POSITION`)**
   - Moves the printer to a predefined position for mounting transportation brackets.
   - Disables steppers for safe handling.
   - Saves the transport state and activates LED/Neopixel indicators.

2. **Reset Transport Position Macro (`RESET_TRANSPORT_POSITION`)**
   - Resets the transport state after removing the brackets.
   - Restores the printer to normal operation.
   - Stops LED/Neopixel feedback.

3. **Transport State Check (`_TRANSPORT_CHECK`)**
   - Verifies the current transport state and updates LED/Neopixel indicators or displays status messages on the LCD.

4. **Menu Integration**
   - Provides an LCD menu entry to toggle transport mode directly.
   - Displays the current transport state as "ON" or "OFF."

### Notes:
- Uncomment and adjust the LED/Neopixel settings if used.
- Add the following to your `printer.cfg` to enable saving variables:
  ```gcode
  [save_variables]
  filename: ~/printer_data/config/saved_variables.cfg
