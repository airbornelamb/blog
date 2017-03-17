

# Using TaskWarrior

Taskwarrior is a command-line linux application which is both simple to use and highly complex to configure. Below are some easy examples to get your feet wet.

**Create and Manipulate Tasks**

To add a simple task:

`task add mow the lawn`

To add a more complex task:

`task add Mow the Lawn project:HomeMaintenance due:2017-04-01 +lawncare`

Notice that this creates a task which is assigned to a particular project and has an assigned Year-Month-Day due date with an associated tag. Due dates can also be assigned naturally, such as due:1d for one day from now, or due:2month for two months from now.

The wonderful feature of taskwarrior is that it attempts to be smart about how

To list your tasks:

`task next`

This report will list the next actions. The wonderful feature of taskwarrior is that it attempts to be smart about what you need to do next. It will assign a numerical weight based on if a task is tagged, assigned, to a project, near a deadline, has a defined priority, or is overdue. These all combine to show which actions are listed next.

`task list`

This will list all open tasks

`task timesheet`

This will list a timesheet of all tasks which have been completed during this workweek.

`task summary`

This will produce a bar chart of the progress you have made according to each open project.

To complete a task:
Find out the number using the "task list" or "task next" commands and then you can modify it.

`task 1 done`

This can also be used with multiple tasks at once.

`task 1 2 3 done`

To modify a task:

`task 1 modify TYPE ANY CHANGES`

To delete a task:

`task 1 delete`

A 30-second tutorial can be found here https://taskwarrior.org/docs/30second.html
For more detailed instructions, the official documentation is here https://taskwarrior.org/docs/
