# Installation Guide

## Prerequisites

- CMake 3.15 or higher
- C++17 compatible compiler
- Visual Studio 2019 or higher (Windows)
- Git
- Python 3.6 or higher (for scripts)
- Conan (C++ package manager)

## Installing Dependencies

Before building the project, you need to install the required dependencies using Conan:

```bash
pip install conan
conan install . --install-folder=build --build=missing
```

## Building from Source

1. Clone the repository:
```bash
git clone https://github.com/yourusername/DEngine-pcsx4.git
cd DEngine-pcsx4
```

2. Create a build directory:
```bash
mkdir build
cd build
```

3. Configure with CMake:
```bash
cmake .. -DCMAKE_BUILD_TYPE=Release
```

4. Build the project:
- On Windows:
  ```bash
  cmake --build . --config Release
  ```
- On Linux/macOS:
  ```bash
  make
  ```

## Running Tests

To run the test suite:
```bash
ctest --output-on-failure
```

## Troubleshooting

If you encounter any issues during installation, please:
1. Ensure all prerequisites are installed
2. Check the error logs
3. Open an issue on the GitHub repository

## License

See the LICENSE file for details.
