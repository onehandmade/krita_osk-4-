  
### **Core Purpose & Overview**

The program is an accessibility-focused utility built in **AutoHotkey v2**. It provides a floating, always-on-top software control bar designed to assist digital artists using **Krita**. Its primary purpose is to eliminate the need for complex multi-key physical keyboard combinations or simultaneous physical inputs through features like **"Sticky Modifiers"** and an optional **"Hover Mode"**.

---

### **Key Features & Functionality**

1. **Sticky Modifiers (Ctrl, Shift, Alt):**
* Users can click/toggle modifier buttons (`Ctrl`, `Shift`, `Alt`) on the interface ahead of time.


* Once a modifier is set to "ON" (indicated visually by color changes), the next button command clicked will automatically prepend the corresponding modifier (`^`, `+`, `!`) to the input action.


* Modifiers automatically reset to "OFF" immediately after a command is dispatched.




2. **Command Grid Layout:**
* Features a 4-row button layout covering frequent Krita shortcuts:


* *Row 1:* Undo, Redo, Copy, Paste, Backspace.


* *Row 2:* Brush, Eraser, Picker, Fill, Select All.


* *Row 3:* Brush Size control, Zoom In/Out, Reset Zoom.


* *Row 4:* Mirror, Rotate Reset, Pan Canvas, Zoom/Rotate, Escape.




* Includes specialized handlers for canvas navigation tools like panning and zooming/rotating.




3. **Hover Activation Mode:**
* Can be toggled on via the interface (`Hover: On/Off`).


* Uses a timer-based mouse monitor (`HoverCheck`) that tracks when the cursor lingers over a specific assistant button for a configurable delay (default `700ms`), automatically triggering the command without requiring a physical click.




4. **Dynamic GUI & Positioning:**
* Automatically adapts and responds to window resizing (`OnResize`, `BuildKeys`).


* Includes a helper function to snap the control bar to the bottom center of the active monitor work area.


* Built with transparency (`WinSetTransparent`) and DPI awareness enabled (`SetProcessDpiAwarenessContext`).
