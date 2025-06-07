# modtextbuilder
A simple tool to compile new text files for Impossible Creatures.

Version 1.0<br>
Developed by Renee Peterson

**Basic Usage:**

**LOCALE Path:** This should point to your mod's locale folder, where the file **ModText.dll** is stored.<br>
**BACKUP Path:** This can be a folder of your choosing. When you build your .DLL file, a backup of the old one will be saved here.<br>
**RC File:** The resource file that contains your mod's text. Manual path selection is available, but in most cases you should let the tool set this for you. See below.

**Generate .RC File:** Clicking this will automatically create a .RC resource from your existing ModText file inside the LOCALE Path. This is the file you will edit to modify your mod's text. It is possible to obtain a .RC file from other sources, but for the highest degree of compatibility with the tool and with IC, you should use this feature to generate your file. Clicking this will also automatically set the **RC File** path to the location of the generated file. You should only need to do this step once per project. You must set the LOCALE Path before this button becomes available.

**Open .RC File:** Opens the selected .RC file using your system's default program. This button becomes available after you have selected a valid .RC file.

**Build .DLL:** Click this to compile your .RC resource into a new ModText.dll file to be read by IC. All three paths must be set before you can build.

The white box at the bottom of the window will display errors and general messages.

Unfortunately, at the time of writing, the tool only fully supports English language files. Multi-language support is under investigation.

The executable must be in the same folder as the MinGW32 toolchain. Don't move it unless you know what you are doing.

Note: Running ModTextBuilder.exe will likely trigger Windows Defender SmartScreen. To proceed to the tool, you can click on "More info" and "Run anyway". If you'd like to avoid this warning, you can create an exception in Windows Defender.

