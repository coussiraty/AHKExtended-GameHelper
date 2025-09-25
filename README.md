# AHKExtended - Advanced AutoHotKey Plugin for GameHelper2

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/your-username/AHKExtended-GameHelper/releases)
[![.NET](https://img.shields.io/badge/.NET-8.0-purple.svg)](https://dotnet.microsoft.com/download/dotnet/8.0)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

An advanced AutoHotKey plugin for GameHelper2 with modern UI, enhanced key binding support, and powerful automation features.

## 🚀 Features

### Modern User Interface
- **Tab-based Interface** - Clean, organized UI similar to VS Code
- **Profile Management** - Multiple configuration profiles with easy switching
- **Real-time Key Capture** - Click-and-capture key binding system
- **Visual Feedback** - Immediate response for all interactions

### Advanced Key Binding Support
- **Full Keyboard Support** - All standard keys (A-Z, 0-9, F1-F12, etc.)
- **Mouse Button Support** - Left, Right, Middle mouse buttons
- **Modifier Keys** - Ctrl, Alt, Shift, Windows key combinations
- **Special Keys** - Arrow keys, Home, End, Page Up/Down, Insert, Delete

### Dynamic Conditions System
- **Expression-based Logic** - Write custom conditions using C# syntax
- **Real-time Compilation** - Conditions are compiled and executed dynamically
- **Rich Context** - Access to player stats, buffs, flask info, and more
- **Template System** - Pre-built templates for common scenarios

### Automation Features
- **Rule-based Actions** - Define complex automation rules
- **Conditional Execution** - Actions execute only when conditions are met
- **Key Sequences** - Chain multiple key presses with timing
- **Auto-quit Protection** - Safety features to prevent unwanted logouts

## 🛠️ Installation

### Prerequisites
- **GameHelper2** - This plugin requires GameHelper2 to be installed
- **.NET 8.0 Runtime** - Required for execution
- **Windows 10/11** - 64-bit architecture

### Installation Steps
1. **Download** the latest release from [Releases](https://github.com/your-username/AHKExtended-GameHelper/releases)
2. **Extract** the plugin files to your GameHelper2 plugins directory:
   ```
   GameHelper2/Plugins/AHKExtended/
   ```
3. **Restart** GameHelper2
4. The plugin will appear in the plugins list

### Manual Build (Advanced)
```bash
git clone https://github.com/your-username/AHKExtended-GameHelper.git
cd AHKExtended-GameHelper
dotnet build --configuration Release
```

## 📖 Usage

### Creating Profiles
1. Click the **"+"** button to create a new profile
2. Enter a profile name
3. Configure rules and conditions for your profile
4. Switch between profiles using the tab interface

### Setting Up Key Bindings
1. Click on a key binding field
2. The interface will show **"Press any key..."**
3. Press the desired key combination
4. The binding is automatically captured and saved

### Creating Dynamic Conditions
1. Use the **"Add New Condition"** button
2. Choose from pre-built templates or write custom expressions
3. Examples:
   ```csharp
   // Health-based condition
   PlayerVitals.HP.Percent <= 30
   
   // Key press condition
   IsKeyPressedForAction(VK.RBUTTON)
   
   // Flask charges condition
   PlayerFlasks.FlaskInfo[0].CurrentCharges < 5
   
   // Buff condition
   PlayerBuffs.HasBuff("Flask Effect")
   ```

### Advanced Features
- **Profile Cloning** - Duplicate existing profiles for quick setup
- **Import/Export** - Share configurations with other users
- **Debug Mode** - Monitor rule execution in real-time
- **Conditional Logic** - Combine multiple conditions with AND/OR logic

## 🎯 Use Cases

### Combat Automation
- **Emergency Flask Usage** - Automatically use flasks when health is low
- **Buff Maintenance** - Keep important buffs active
- **Skill Rotation** - Execute skill sequences based on conditions

### Quality of Life
- **Auto-logout** - Safe logout when dangerous conditions are met
- **Inventory Management** - Automate item sorting and usage
- **Resource Monitoring** - Track flask charges, mana, etc.

### Advanced Macros
- **Complex Key Sequences** - Chain multiple actions with precise timing
- **Conditional Execution** - Actions that depend on game state
- **Mouse Integration** - Combine keyboard and mouse actions

## 🔧 Configuration

### File Structure
```
AHKExtended/
├── config/
│   └── settings.txt          # Main configuration
├── profiles/
│   ├── profile1.json         # Individual profile configs
│   └── profile2.json
└── AHKExtended.dll          # Main plugin file
```

### Settings Format
Settings are stored in JSON format with automatic backup and validation.

## 🐛 Troubleshooting

### Common Issues
- **Plugin not loading**: Ensure GameHelper2 is updated to the latest version
- **Key capture not working**: Check for conflicting key bindings
- **Conditions not executing**: Verify syntax in the dynamic condition editor

### Debug Mode
Enable debug mode in settings to see:
- Real-time condition evaluation
- Rule execution logs
- Performance metrics
- Error messages

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

### Development Setup
1. Clone the repository
2. Ensure GameHelper2 development environment is set up
3. Build with `dotnet build`
4. Test with GameHelper2

## 📝 Changelog

### v1.0.0 (Current)
- ✅ Modern tab-based user interface
- ✅ Enhanced key binding system with mouse support
- ✅ Dynamic conditions with real-time compilation
- ✅ Profile management system
- ✅ Advanced automation rules
- ✅ Template system for common scenarios
- ✅ Debug mode and error handling
- ✅ Performance optimizations

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **GameHelper2 Team** - For the excellent framework
- **Community Contributors** - For testing and feedback
- **ImGui.NET** - For the immediate mode GUI framework

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/your-username/AHKExtended-GameHelper/issues)
- **Discord**: Join the GameHelper2 community
- **Wiki**: [Documentation Wiki](https://github.com/your-username/AHKExtended-GameHelper/wiki)

---

**Made with ❤️ for the GameHelper2 community**