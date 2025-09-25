# AHKExtended - GameHelper2 Plugin# AHKExtended


Advanced AutoHotKey plugin with modern interface for GameHelper2.


## ⚡ Quick InstallationAdvanced AutoHotKey plugin with modern interface for GameHelper2.

1. **Download the `AHKExtended` folder** from releases

2. **Place it inside `GameHelper2/Plugins/`**

3. **Restart GameHelper2**## ⚡ Quick Installation##


Correct structure:

```

GameHelper2/1. **Download the `AHKExtended` folder** from releases.

└── Plugins/

    └── AHKExtended/          ← Place here2. **Place it inside `GameHelper2/Plugins/`**2.
        ├── AHKExtended.dll

        └── StatusEffectGroup.json3. **Restart GameHelper2**

```

## 🔧 For Developers

Correct structure:Estrutura correta:

### How to Compile

``````

**IMPORTANT**: The plugin must be inside GameHelper2 structure to compile.

GameHelper2/GameHelper2/

```bash

# 1. Have complete GameHelper2└── Plugins/└── Plugins/

GameHelper2/

├── GameHelper/    └── AHKExtended/          ← Place here    └── AHKExtended/          ← Cole aqui

├── GameOffsets/

└── Plugins/        ├── AHKExtended.dll        ├── AHKExtended.dll



# 2. Clone this plugin into Plugins folder        └── StatusEffectGroup.json        └── StatusEffectGroup.json

cd GameHelper2/Plugins

git clone https://github.com/coussiraty/AHKExtended-GameHelper.git AHKExtended``````



# 3. Compile

cd AHKExtended

dotnet build --configuration Release## 🔧 For Developers## � Para Desenvolvedores

```


### Why inside the structure?

### How to Compile### Como Compilar

The plugin needs GameHelper2 references (`GameHelper.dll` and `GameOffsets.dll`) to compile. That's why it must be inside the `Plugins/` folder of GameHelper2.



## 📋 Features

**IMPORTANT**: The plugin must be inside GameHelper2 structure to compile.

- ✅ Modern tabbed interface

- ✅ Key capture (mouse and keyboard)

- ✅ Profile system

- ✅ Dynamic rules

- ✅ Customizable hotkeys

# 1. Have complete GameHelper2

## 🎯 How to Use

GameHelper2/GameHelper2/

1. Open GameHelper2

2. Go to Plugins → AHKExtended

3. Configure your profiles in tabs:

   - **Profiles**: Manage profile

   - **Rules**: Configure rules

   - **Hotkeys**: Define shortcuts



## 🐛 Issues?



- Make sure plugin is in `GameHelper2/Plugins/AHKExtended/`

- Restart GameHelper2

- Check if you have .NET 8.0cd GameHelper2/Pluginscd GameHelper2/Plugins



## 📄 Licensegit clone https://github.com/coussiraty/AHKExtended-GameHelper.git AHKExtended 



MIT License - Use freely!

# 3. Compile

cd AHKExtended

dotnet build --configuration Release

``````


### Why inside the structure?

The plugin needs GameHelper2 references (`GameHelper.dll` and `GameOffsets.dll`) to compile. That's why it must be inside the `Plugins/` folder of GameHelper2.

## 📋 Features

- ✅ Modern tabbed interface

- ✅ Key capture (mouse and keyboard)

- ✅ Profile system

- ✅ Dynamic rules

- ✅ Customizable hotkeys


## 🎯 How to Use#

1. Open GameHelper2.

2. Go to Plugins → AHKExtended2.

3. Configure your profiles in tabs:

   - **Profiles**: Manage profiles

   - **Rules**: Configure rules

   - **Hotkeys**: Define shortcuts


## 🐛 Issues?## 


- Make sure plugin is in `GameHelper2/Plugins/AHKExtended/`

- Restart GameHelper2

- Check if you have .NET 8.0


## 📄 License## 📄 Licença



MIT License - Use freely!

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

- **Issues**: [GitHub Issues](https://github.com/coussiraty/AHKExtended-GameHelper/issues)
- **Discord**: [GameHelper2 Community](https://discord.gg/RShVpaEBV3)
- **Wiki**: [Documentation Wiki](https://github.com/coussiraty/AHKExtended-GameHelper/wiki)

---

**Made with ❤️ for the GameHelper2 community**