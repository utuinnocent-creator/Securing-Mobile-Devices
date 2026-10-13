
### Instructions for Submission
1.  Create your project folder.
2.  Save your final python script as `mobile_final.py`.
3.  Save the text above as `README.md`.
4.  Submit `mobile_final.py` to CodeGrade.
5.  Keep the `README.md` for your portfolio to demonstrate your understanding of mobile security tools and documentation.

### Tips for Your Script Implementation
Since you are building the actual logic:
- Use the `subprocess` module to run `adb` commands (e.g., `adb shell getprop`, `adb shell pm list packages`).
- For root detection, check for the existence of files like `/system/bin/su` or properties like `ro.secure`.
- For port scanning, you can use `adb shell netstat` or `ss` if available on the device, or attempt to bind to ports to see if they are in use.
- Ensure your script handles cases where ADB is not installed or no device is connected gracefully with clear error messages.
