# ROS 2 Workspace Adventure ✨

A comprehensive ROS 2 learning workspace containing source code, experiments, documentation, and tools for robotics development and exploration.

## 📋 Overview

This repository serves as a personal ROS 2 workspace for storing and organizing various robotics projects, learning materials, and experimental implementations. It follows the standard ROS 2 workspace structure and is designed to evolve continuously as new projects, improvements, and solutions are developed.

### Purpose

- **Source Code**: ROS 2 scripts, nodes, and packages for robotics projects
- **Experiments & Tests**: Test cases and example implementations for verifying package functionality
- **Documentation**: Guides, tutorials, and configuration notes for ROS 2 development
- **Utilities**: Helper scripts and tools to streamline development workflows and task automation

## 📁 Workspace Structure

```
ros2_ws_adventure/
├── src/                    # ROS 2 packages directory
│   ├── package_1/
│   ├── package_2/
│   └── ...
└── README.md              # This file
```

Each package in the `src/` directory contains the actual ROS 2 code organized by functionality and purpose.

## 🚀 Quick Start

### Prerequisites

- ROS 2 installed (Humble, Iron, or Jazzy recommended)
- Python 3.9+ or C++ build tools depending on package implementations
- Git for version control

### Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/richy-gs/ros2_ws_adventure.git
   cd ros2_ws_adventure
   ```

2. **Install dependencies**:
   ```bash
   rosdep install --from-paths src --ignore-src -r -y
   ```

3. **Build the workspace**:
   ```bash
   colcon build
   ```

4. **Source the workspace**:
   ```bash
   source install/setup.bash
   ```

## 📦 Packages

This workspace includes various packages organized by learning objectives and project scope. Each package contains:

- **Source files**: Python or C++ implementations
- **Launch files**: ROS 2 launch configurations
- **Package metadata**: `package.xml` for package definition
- **Examples**: Sample code demonstrating package functionality

For detailed information about each package, refer to individual package READMEs in their respective directories.

## 💡 Usage Examples

### Building a Specific Package

```bash
colcon build --packages-select <package_name>
```

### Running a Node

```bash
ros2 run <package_name> <node_name>
```

### Launching a Launch File

```bash
ros2 launch <package_name> <launch_file>.launch.py
```

### Viewing the ROS 2 Graph

```bash
rqt_graph
```

## 🛠️ Development Workflow

1. Create new packages in the `src/` directory
2. Implement nodes, services, and topics following ROS 2 best practices
3. Write launch files for complex multi-node systems
4. Test locally before committing
5. Update this README with new package descriptions as they're added

## 📚 Learning Resources

- [Official ROS 2 Documentation](https://docs.ros.org/en/humble/)
- [ROS 2 Tutorials](https://docs.ros.org/en/humble/Tutorials.html)
- [ROS 2 Design Patterns](https://docs.ros.org/en/humble/Concepts/Advanced/About-Executors.html)

## ⚙️ Common Commands

| Command | Purpose |
|---------|---------|
| `colcon build` | Build all packages in the workspace |
| `colcon test` | Run tests for all packages |
| `ros2 node list` | List all active ROS 2 nodes |
| `ros2 topic list` | List all active topics |
| `ros2 service list` | List all available services |
| `ros2 interface show <interface>` | Display interface details |

## 🔧 Troubleshooting

- **Build failures**: Ensure all dependencies are installed with `rosdep install`
- **Source not found**: Make sure to source the setup script after building
- **Node not found**: Verify the package is built and the node name is correct
- **Topic/Service errors**: Use `ros2 topic list` and `ros2 service list` to debug

## 📝 Contributing & Evolution

This workspace is actively maintained and continuously updated with:

- New package implementations
- Improved solutions to common problems
- Documentation updates
- Experimental features and prototypes

<!-- ## 📄 License

Specify your license here (e.g., MIT, Apache 2.0, etc.) -->

## 👤 Author

**Ricardo García** - [@richy-gs](https://github.com/richy-gs)

---

**Last Updated**: October 2025

*Happy ROS 2 learning! 🚀*