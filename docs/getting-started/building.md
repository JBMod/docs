# Building JBMod

JBMod is built using a modified Source Engine branch. Follow the instructions below for your operating system.

!!! Prerequisite
    You must have JBMod installed via Steam on the **github** branch for these instructions to work correctly.

=== "Windows"

    ### Requirements

    - **JBMod installed via Steam** (on the github branch)    
    - **Visual Studio 2022** with the following workload and components:
        - Desktop development with C++
        - MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest)
        - Windows 11 SDK (10.0.22621.0) or Windows 10 SDK (10.0.19041.1)
    - **Python 3.13** or later

    ### Steps
    
    1.  Navigate to the `src` directory.
    2.  Run `createallprojects.bat` to generate the Visual Studio solution.
    3.  Open `everything.sln` and build the solution (**Build** > **Build Solution**).
    4.  **To run**: Set the client project (e.g., `Client (JBMod)`) as the startup project and start the debugger.

=== "Linux"

    ### Requirements
    
    - **JBMod installed via Steam** (on the github branch)
    - **Podman**

    ### Steps
    
    1.  Navigate to the `src` directory.
    2.  Run `./buildallprojects` to build against the Steam Runtime.
    3.  Launch the game from the game directory using the generated launcher (e.g., `./jbmod.sh`).

---

## Troubleshooting

- **Missing SDK**: Ensure you have exactly the Windows 10/11 versions listed above.
- **Python version**: Double-check `python --version` to ensure it is 3.13+.
- **Podman on Linux**: Ensure your user has permissions to run Podman containers.
