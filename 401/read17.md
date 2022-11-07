# Day 17

## Automation

### Regular Expressions in Python

In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

`import re`

The re library in Python provides several functions that make it a skill worth mastering.

### Basic Patterns: Ordinary Characters

You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

Examples are 'A', 'a', 'X', '5'.

Ordinary characters can be used to perform simple exact matches:

    pattern = r"Cookie"

    sequence = "Cookie"

    if re.match(pattern, sequence):

        print("Match!")

    else: print("Not a match!")

    `Match!`

### Wild Card Characters: Special Characters

Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

### Repetitions

It becomes quite tedious if you are looking to find long patterns in a sequence. Fortunately, the re module handles repetitions using the following special characters:

`+ -` Checks if the preceding character appears one or more times starting from that position.

    re.search(r'Co+kie', 'Cooookie').group()

    'Cooookie'

### Grouping in Regular Expressions

The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.

## Refrences

1- https://www.datacamp.com/tutorial/python-regular-expression-tutorial