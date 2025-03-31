# **Hupia TODO**

This file outlines the tasks required to build **Hupia**, a terminal-based web browser with ASCII and terminal theme rendering, AI integration, and Lua scripting. The tasks are divided into **phases** and **modules** to ensure a structured development process.

---

## **Phase 1: Core Browser**
### **Networking**
- [ ] Implement HTTP/HTTPS requests using `libcurl` or `zig-http`.
- [ ] Handle cookies, headers, and redirects.
- [ ] Add support for fetching HTML, CSS, images, and videos.

### **HTML/CSS Parsing**
- [ ] Integrate `gumbo-parser` for HTML parsing.
- [ ] Extract text, links, images, and videos from HTML.
- [ ] Add basic CSS support for styling (optional).

### **Rendering Engine**
- [ ] Render plain text in the terminal.
- [ ] Implement scrolling and pagination for long pages.
- [ ] Add support for basic formatting (e.g., bold, italics).

### **User Interface**
- [ ] Create a basic terminal UI using `ncurses` or a Zig library.
- [ ] Add keyboard shortcuts for navigation (e.g., back, forward, refresh).
- [ ] Display a status bar with the current URL and loading status.

---

## **Phase 2: Image and Video Rendering**
### **Image Rendering**
- [ ] Integrate `libcaca` for ASCII/ANSI art rendering of images.
- [ ] *Add support for rendering images in terminal colors.*
- [ ] *Allow users to toggle between ASCII and terminal color modes.*

### **Video Rendering**
- [ ] Render video frames as ASCII/ANSI art.
- [ ] *Integrate `ffmpeg` for video decoding.*
- [ ] *Add playback controls (e.g., play, pause, stop).*

### **Configuration**
- [ ] Create a `config.toml` file for user preferences.
- [ ] Add options for image and video rendering modes.

---

## **Phase 3: Lua Scripting**
### **Lua Interpreter**
- [ ] Embed a Lua interpreter (e.g., via `lua.h` or a Zig binding).
- [ ] Expose browser APIs to Lua scripts (e.g., fetch content, render text).

### **Script Hooks**
- [ ] Add hooks for Lua scripts (e.g., on page load, on user input).
- [ ] Create a `scripts/` directory for user scripts.

### **Documentation**
- [ ] Write a guide for writing and using Lua scripts.
- [ ] Provide example scripts for common tasks.

---

## **Phase 4: Polish and Extensibility**
### **Configuration**
- [ ] Add more options to `config.toml` (e.g., AI API keys, rendering preferences).
- [ ] Allow users to enable/disable features (e.g., AI, Lua scripting).

### **Plugin System**
- [ ] Design a plugin system for adding new functionality.
- [ ] Provide a template for creating plugins.

### **Performance Optimization**
- [ ] Optimize rendering for large pages and videos.
- [ ] Reduce memory usage and improve responsiveness.

### **Documentation**
- [ ] Write a comprehensive user guide.
- [ ] Add API documentation for developers.
---

## ***Phase 5: Parental Controls***

### ***Basic Parental Controls***
- [ ] Add a configuration file for parental controls (parental.toml).
- [ ] Implement website blocking (e.g., blocklist).
- [ ] Add time limits for browsing.

### ***Advanced Parental Controls***
- [ ] Integrate a content filtering API (e.g., CleanBrowsing).
- [ ] Add password protection for parental controls.
- [ ] Create a UI for managing parental controls.

---

## ***Phase 6: AI Integration***
### ***Smart Search***
- [ ] Integrate OpenAI GPT or a local LLM for contextual search.
- [ ] Add a command to query the AI and display results in the terminal.

### ***Content Summarization***
- [ ] Extract text from web pages.
- [ ] Send text to an LLM for summarization.
- [ ] Display summaries in a popup or sidebar.

### ***Image/Video Analysis***
- [ ] Integrate a computer vision model (e.g., CLIP or YOLO).
- [ ] Analyze images and videos and display descriptions.

### ***Voice Commands***
- [ ] Integrate Whisper for speech recognition.
- [ ] Add support for voice commands (e.g., "Search for terminal browsers").

### ***Text-to-Speech (TTS)***
- [ ] Integrate a TTS model (e.g., Coqui AI or Google TTS).
- [ ] Add a command to read selected text aloud.

---

## **Phase 7: Community and Collaboration**
### **Contributing Guidelines**
- [ ] Write a `CONTRIBUTING.md` file.
- [ ] Set up a code of conduct.

### **Testing**
- [ ] Add unit tests for core modules.
- [ ] Set up continuous integration (CI) for automated testing.

### **Release**
- [ ] Create a release checklist.
- [ ] Publish binaries for major platforms (Linux, macOS, Windows).

---

## **Stretch Goals**
### **Advanced AI Features**
- [ ] Add support for personalized recommendations.
- [ ] *Integrate a chatbot for interactive assistance.*

### **Advanced Rendering**
- [ ] Add support for animated ASCII art.
- [ ] Implement custom color palettes for terminal rendering.

### **Cross-Platform Support**
- [ ] Add support for mobile terminals.
- [ ] *Optimize for low-resource environments (e.g., RISC-V).*

---

## **Notes**
- Tasks marked with [ ] are incomplete.
- Tasks marked with [x] are complete.
- *Tasks in italics are Pay options.*
- Prioritize tasks based on your goals and available time.
