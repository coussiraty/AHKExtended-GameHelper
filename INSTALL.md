# Installation Instructions

## Quick Setup

1. **Download the latest release** from the [Releases page](https://github.com/your-username/AHKExtended-GameHelper/releases)

2. **Extract to GameHelper2 Plugins folder**:
   ```
   GameHelper2/
   └── Plugins/
       └── AHKExtended/
           ├── AHKExtended.dll
           ├── StatusEffectGroup.json
           └── System.Linq.Dynamic.Core.dll
   ```

3. **Restart GameHelper2**

4. **Enable the plugin** in GameHelper2's plugin manager

## Building from Source

### Prerequisites
- .NET 8.0 SDK
- GameHelper2 installed
- Visual Studio 2022 or VS Code (optional)

### Steps
```bash
git clone https://github.com/your-username/AHKExtended-GameHelper.git
cd AHKExtended-GameHelper
dotnet restore
dotnet build --configuration Release
```

### Dependencies
The plugin requires these GameHelper2 assemblies:
- `GameHelper.dll`
- `GameOffsets.dll`

These should be available in your GameHelper2 installation.

## Configuration

After installation, the plugin will create:
- `config/settings.txt` - Main configuration file
- `profiles/` - Directory for profile configurations

## Troubleshooting

### Plugin not loading
- Ensure GameHelper2 is up to date
- Check that all dependencies are present
- Verify .NET 8.0 runtime is installed

### Build errors
- Make sure GameHelper2 assemblies are accessible
- Update NuGet packages if needed
- Check that all source files are properly copied

### Runtime issues
- Enable debug mode in plugin settings
- Check GameHelper2 logs for error messages
- Ensure no conflicting plugins are installed