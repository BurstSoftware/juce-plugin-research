How do I start a VST plugin project with JUCE?

Great question! Let’s start from the very beginning 🚀

JUCE provides a tool called the Projucer, which is used to set up your plugin project. The Projucer generates all the boilerplate code, organizes dependencies, and creates project files for IDEs like Visual Studio, Xcode, or CLion.

Here’s a step-by-step outline for starting a new VST plugin project in JUCE:

📝 Step 1: Install JUCE
Download JUCE from juce.com.
Extract or install it somewhere on your machine.
Inside JUCE, you’ll find the Projucer app (that’s what we’ll use).
📝 Step 2: Open the Projucer
Launch the Projucer application.
Click New Project.
📝 Step 3: Choose Project Type
From the templates, select Audio Plug-In.
This template gives you all the necessary files to start a VST, AU, or AAX plugin.
📝 Step 4: Configure Your Project
Enter your Project Name (important, because it sets up class names, filenames, and plugin identifiers).
Choose the folder where the project will live.
Select your preferred IDE exporter (Visual Studio, Xcode, CLion, etc.).
📝 Step 5: Enable Plugin Formats
In the Projucer, go to the Config tab.
Under Plugin Formats, enable the ones you need:
✅ VST3 (recommended, since VST2 is deprecated).
✅ AU (if you’re on macOS and want Logic compatibility).
✅ AAX (if you’re targeting Pro Tools).
Make sure “VST (Legacy)” is unchecked (Steinberg no longer allows new VST2 licensing).
📝 Step 6: Save and Open in IDE
Hit Save Project and Open in IDE.
This will generate the necessary project files and open your IDE with the JUCE project loaded.
📝 Step 7: Build the Plugin
Compile the project in your IDE.
The resulting binary will be your plugin (a .vst3 file on Windows/macOS).

✅ At this point, you’ll have a working “Hello World” audio plugin that does basic pass-through of audio. From here, we can start customizing it by adding DSP code, parameters, and a GUI.

👉 Do you already have a plugin idea in mind (like an EQ, compressor, synth, or effect)?
Or should we start with a simple project name so I can set up the class structure for you?

Does the juce software cost money 

Good question 👍

JUCE has both free and paid options, depending on what you want to do with your plugin:

💡 JUCE Licensing
Free (JUCE Personal)
You can use JUCE for free if your revenue (or funding) is under $50k per year.
The only limitation: your plugin will show a small JUCE splash screen when the UI first opens.
This is fine for learning, hobby projects, or even small commercial plugins.
JUCE Indie (~$40/month or $400/year)
For individuals or companies making under $500k per year.
Removes the splash screen.
JUCE Pro (~$130/month or $1,300/year)
For larger companies with revenue over $500k/year.
Includes full commercial rights, no splash screen, and extra support.
🎯 What This Means for You
If you’re just starting out, learning, or making small plugins → the free tier is perfect.
If you later decide to sell plugins commercially and want a polished look (no splash screen) → you can upgrade.
