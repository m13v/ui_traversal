# UI traversal script for macOS

A powerful macOS accessibility script that monitors and captures UI changes in real-time, designed as part of the [ScreenPipe](https://github.com/screenpipe/screenpipe) project.

![UI Monitoring Demo](https://github.com/user-attachments/assets/3d60a001-2c92-4c74-9558-a18c6f214273)

## What is it?

This Swift script provides comprehensive UI monitoring capabilities by:
- Capturing text content from any application window
- Tracking UI element changes in real-time
- Maintaining hierarchical relationships between elements
- Storing data efficiently in a SQLite database
- Managing memory usage automatically
- Supporting accessibility features

## Use Cases

- **AI Training Data**: Collect rich UI interaction data for training AI models
- **Application Testing**: Monitor UI changes for testing and debugging
- **Accessibility Testing**: Verify application accessibility compliance
- **User Experience Research**: Track how users interact with applications
- **Documentation**: Automatically document UI flows and content

## Getting Started

1. **Prerequisites**
   ```bash
   # Install Swift if not already installed
   xcode-select --install
   ```

2. **Permissions**
   - Grant Accessibility permissions in System Preferences > Security & Privacy > Privacy > Accessibility
   - The script will prompt for permissions on first run

3. **Run the Script**
   ```bash
   swift ui_monitoring_macos.swift
   ```

4. **Integration**
   ```swift
   // Use as a library in your Swift project
   let monitor = UIMonitor.getInstance()
   monitor.start()
   
   // Get current UI content
   let content = monitor.getCurrentOutput(app: "safari")
   ```

## Features

- 🚀 Real-time UI change detection
- 📊 Hierarchical element tracking
- 💾 Efficient SQLite storage
- 🧠 Smart deduplication
- 🎯 Focused monitoring of active windows
- 🔄 Automatic state management
- 🛡️ Memory-safe implementation

## Rach out

happy to chat
i@m13v.com
discord: https://discord.gg/AvGe8FJr
Matthew Diakonov

## Contributing

We welcome contributions! Feel free to:
- Open issues for bugs or feature requests
- Submit pull requests
- Improve documentation
- Share use cases and feedback

## Next steps, to-do list
- set output location for the db
- landing page
- cli interface
- windows
- linux
- implementation in Rust
- app

## License

MIT License - feel free to use in your own projects!

---

⭐ If you find this useful, please star the [ScreenPipe repository](https://github.com/screenpipe/screenpipe)!

Part of the [screenpipe](https://github.com/mediar-ai/screenpipe) project - Recording screens & mics 24/7, extracting UI dom, OCR & STT, saving to local db, connecting to AI.