# Windows Compatibility Notes

Agent Lightning currently depends on Gunicorn for server launching.
Gunicorn relies on the Unix-only `fcntl` module, which is not available
on Windows systems.

As a result, CLI-based execution may fail on Windows environments.
Recommended solutions:
- Use WSL (Windows Subsystem for Linux)
- Use Linux or macOS for full functionality
