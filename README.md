I was using Taskwarrior before but I found it has too much feature for my usage.

I was using Todo.txt before but the interface didn't fill my expectations.

I create a very very small bash script that I'm using every day at work to help me track my current and future tasks.

### Features:
- task never change ID (not like Taskwarrior)
- 3 fields per tasks: project, title and an optional description
- human readable/editable data file (tab-separated-value)
- complete a task didn't remove it, but comment it in the data file
- colorized by project
- list can be filtered, search term is highlighted
- priority: if project name use upper case, the task will be printed in bold

### Install:

Copy the file somewhere and make it available for your PATH environment variable.

### Syntaxe:

* create a task:

  ```
  todo @<project> <title>
  todo @<project> <title>. <desc>
  ```
  
  The dot (.) is used as a separator for the description

* list task:

  ```
  todo
  todo <filter>
  ```

* show task:

  ```
  todo <id>
  ```

* complete a task:

  ```
  todo <id> ok|done
  ```

* edit the data file:

  ```
  todo ed
  ```
### Usage:

Because the arguments are used to create the title and the description, in some case You will need to quotes the text (or escape the special chars).
