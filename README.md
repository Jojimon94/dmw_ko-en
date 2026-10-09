Jojimon's Tool - User Guide
Introduction

Jojimon's Tool is designed to apply English translations to the original Korean version of the Convert.jk file used by Digimon World 2000.

The program works by comparing the Korean strings contained in the original Convert.jk file with the Korean strings listed in a translation file. When a match is found, the Korean text is replaced with the corresponding English text from the translation file.

Requirements

Before using Jojimon's Tool, make sure you have:

The original Korean Convert.jk file.
A compatible translation file (see below the content and structure of the file)

Without the original Korean Convert.jk, the tool will not work correctly.


Download and Preparation

To use Jojimon's Tool as demonstrated in the tutorial video on my YouTube channel:

Download the file:
jojimon_tool.dat

Rename it to:
jojimon_tool.exe

Launch the executable.

Once renamed, the application can be used normally.

How to Use Jojimon's Tool
Step 1 - Load the Translation File

After starting the program, the first action is to load the translation file.

The translation file must contain the following columns:

- Originale_ko		Original Korean strings
- testo splittato2	English translations

The tool uses this file as its translation database.

Step 2 - Load the Original Convert.jk

Open the original Korean Convert.jk file.

The tool will scan all text entries contained in the file and compare them against the Korean strings found in the translation file.

Step 3 - Generate the Translation

Start the conversion process.

For each Korean string found in Convert.jk:

If a matching Korean string exists in the translation file, it will be replaced with the English text found in the second column.
If no match is found, the original Korean string will remain unchanged.

It is highly recommended to keep a backup of the original Korean file.

Important Notes About the Translation File

To ensure proper operation of Jojimon's Tool, do not modify the structure or layout of the translation file.

The program expects the file to remain in its original format.

Translation Editing Rules

When modifying translations:

✅ Edit only the text contained in the second column.

❌ Do not modify the Korean strings in the first column.

❌ Do not add or remove columns.

❌ Do not change the overall file structure.

The first column is used by the tool to identify the original strings that must be replaced.

Variables and Control Codes

Special attention must be paid to variables and control codes embedded in the text.

For example:

C06$NC01

These values are interpreted by the game engine and must remain exactly as they are.

Do Not:
Delete variables.
Modify variable names.
Change character order.
Move variables to a different position unless you fully understand their purpose.
Example

Correct:

Welcome, C06$NC01!

Incorrect:

Welcome, Player!

Incorrect:

Welcome, NC01$C06!

Altering these codes may cause text corruption, missing dialogue, scripting issues, or crashes.

Best Practices
Always keep a backup of the original Convert.jk.
Edit only the second column of the translation file.
Preserve all variables and control codes.
Do not alter the structure of the translation file.
Test changes frequently in-game.
Review untranslated entries after conversion.

Disclaimer
The accuracy and completeness of the translated output depend entirely on the quality of the translation file provided by the user. Any Korean string not present in the translation file will remain untranslated in the generated Convert.jk.