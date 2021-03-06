# HLSL_ST3
HLSL syntax highlighting for Sublime Text 3

I'm just trying to provide a better, more fully featured syntax definition for HLSL.

A large part of that is hooking up various things to Sublime's symbol indexer, making them work with GoToDefinition.  So far I have functions and structs working, and I have function definitions separated from call-sites in an effort to keep the symbol list a little cleaner.  The eventual goal is to make everything properly indexed in a way that it's reasonable to create scope-aware autocompletions and really be able to look at Sublime as a real HLSL IDE.  And until I finally get there, I'm just hoping to provide people with a better HLSL writing experience.

This works best when all of your shared shader source is in your active sublime-project file.  Then GoToDefinition will work across everything in the project.  Otherwise it will only work across currently opened files.

Best with my HLSL-centric theme, Rocklobster:  https://github.com/MattSutherlin/RockLobster_ST3Theme
