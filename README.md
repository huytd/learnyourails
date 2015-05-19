# Learn You Rails

**LearnYouRails** is an interactive course for learning **Ruby On Rails**.

Inspired by **NodeSchool** (learnyounode,...)

![](http://i.imgur.com/Me9ZnET.png)

# How to run

To run **LearnYouRails**, you need to config system path to this folder, for example:

```
nano ~/.bash_profile
export PATH=$PATH:"~/Code/learnyourails"
```
```
source ~/.bash_profile
```

Then you can run **LearnYouRails** anywhere via Terminal, to see challenge content:

```
railsme
```

or 

```
railsme challenge
```

To verify your challenge submission:

```
railsme verify
```

# How to create challenge

The challenges are stored in `challenges` folder. In this folder, we have the challenge number (01, 02, 03,...)

Each challenge has 2 files:
- **challenge.txt**: contains content of the challenge
- **verify.txt**: contains the verify rules for this challenge

### Challenge Content

The challenge content is a simple text file, support some markup color:
- `<red></red>`: Red color
- `<yellow></yellow>`: Yellow color
- `<blue></blue>`: Blue color
- `<cyan></cyan>`: Green color
- `<green></green>`: Green color
- `<light></light>`: Make the color lighter
- `<u></u>`: Underline

### Verify Rules

The verify rules contains 2 parts:
- **Rule header**: The first line of the rule file, define type of rule
- **Rule check**: Next lines define the checking condition for the rule

Implemented rules:
- **@run**: Run the command, then use `@output` to check the output
- **@file_check**: Check the folder struct with `@file` and `@folder`