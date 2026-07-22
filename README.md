# Linux Shell Emulator

A web-based Linux shell emulator that simulates a Linux CLI environment in your browser.

## Features

- 🖥️ **Terminal Interface**: Full terminal emulation with xterm.js
- 📁 **Virtual File System**: Simulated Linux file system with common directories
- 🔧 **Common Commands**: Support for essential Linux commands (ls, cd, pwd, cat, mkdir, etc.)
- 🎨 **Modern UI**: React-based frontend with responsive design
- ⚡ **Real-time Execution**: Instant command execution and feedback

## Tech Stack

- **Frontend**: React 18, xterm.js, Tailwind CSS
- **Backend**: Node.js, Express
- **File System**: In-memory virtual file system
- **Build Tools**: Vite (frontend), Node (backend)

## Project Structure

```
linux-shell-emulator/
├── frontend/              # React frontend application
│   ├── src/
│   │   ├── components/   # React components
│   │   ├���─ lib/          # Utilities and helpers
│   │   └── App.jsx
│   └── package.json
├── backend/               # Node.js backend API
│   ├── src/
│   │   ├── routes/       # API routes
│   │   ├── controllers/  # Command handlers
│   │   ├── fileSystem/   # Virtual file system
│   │   └── index.js
│   └── package.json
├── package.json           # Root package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js 16+
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/xantemp/linux-shell-emulator.git
cd linux-shell-emulator
```

2. Install dependencies:
```bash
npm install
```

3. Install frontend and backend dependencies:
```bash
npm run install:all
```

### Development

Start both frontend and backend in development mode:
```bash
npm run dev
```

Or start them separately:
```bash
# Terminal 1: Start backend
npm run dev:backend

# Terminal 2: Start frontend
npm run dev:frontend
```

The application will be available at `http://localhost:5173`

### Build

```bash
npm run build
```

## Supported Commands

- `ls` - List directory contents
- `cd` - Change directory
- `pwd` - Print working directory
- `cat` - Display file contents
- `mkdir` - Create directory
- `touch` - Create file
- `rm` - Remove file/directory
- `cp` - Copy file
- `mv` - Move/rename file
- `echo` - Print text
- `clear` - Clear terminal
- `help` - Show available commands
- And more!

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

MIT
