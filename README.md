# todo-command

This is a simple tool for making and organizing a To Do list.

# Instructions
## - add
First add items to the todo list using add.
add takes at least two elements, a flag and a string.
The flag indicates a header (-h), a task (-t), or a subtask (-s).
The string is what is put inside the flagged element.
Headers create a new item in the list.
Tasks and subtasks append to the current header.
The user can do many flag and string combinations in a row.
### Example
todo add -h "The first thing I need to do" -t "Call Tom" -s "cell: 555-555-5555" -s "home: 545-545-4545"

## - addto
using Addto you can specify a header to append tasks and subtasks to using the list items number in the list.
Usage is the same as add, but a number goes before the flag specifying the header.
### Example
todo addto 2 -t "don't forget" -s "nap time is at 3 pm"

## - rm
rm deletes the list item you specify by list number.
### Example
todo rm 2 4 5

## - swap
swap helps reorganize the list by letting you swap two items in the list.
### Example
todo swap 1 2

## - header
header lets the user change what the title of the todo list is.
### Example
todo header "This is now the title of the todo list"
