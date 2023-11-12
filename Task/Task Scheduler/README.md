# Task Scheduler
## Intro
A scheduler that schedules for tasks (such as automatically execute the task at specified time.)

## NOTICE 
Due to security issue, the Windows 11 OS does not allow me to take screenshots when some specific apps are opened. (such as Task Scheduler).

Thus, I may not demo it with screenshot. Sorry.

## Will learn
### How to create scheduled tasks?

Step 0:

Write a batch file then save it.

Step 1:

Type the keyword "Task Scheduler" in search box in Start Menu.

![image](https://github.com/40843245/Windows/assets/75050655/6083137b-acba-4252-bb3b-9a3c91741891)

Step 2:

On the left pane, select "Task Scheduler Library".

Step 3:

On the right pane, click "Create Task".

Step 4:

In the create task dialog, provide some basic infos. Including:

1. names (In General tab)
2. trigger (In Triggers tab) :

Add a new trigger by clicking "New" button on Triggers tab. Finally click "Ok" button in "New Trigger" dialog.

3. action (In Actions tab) :

Add a new action by clicking "New" button on Actions tab. Finally click "Ok" button in "New Action" dialog.

4. condition  (In Conditions tab) :

Add a new condition by clicking "New" button on Conditions tab. Finally click "Ok" button in "New Condition" dialog.

5. settings (In Settings tab) :

Set the Additional settings for scheduled task.

For more details about infos, see the "Info in Create Task Dialog" in "Detailed" sections.

Step 5:

Click "Ok" to apply the change.

Step 6:

Check the task is fully scheduled. 

That's done.

## Detailed 
### Info in Create Task Dialog
There are five tabs in create task dialog:

1. General tab
2. Triggers tab
3. Actions tab
4. Conditions tab
5. Setting tab
    
#### General tab
##### Name
Required.

Name of scheduled task.

##### Location
Required. (Defaults to '/')

Location of scheduled task.

##### Description
Optional.

Description of scheduled task. Like comments in code.

#### Triggers tab
In New Trigger Dialog, you will see:

##### Begin the task
Required. (Defaults to option 'On a schedule')

When to begin the task.

##### Settings
There are these single-selected choices:

1. One time
2. Daily
3. Weekly
4. Monthly

##### Advanced settings
There includes these checkboxes.

1. Delay task for up to (random delay)
2. Repeat task every
3. Stop the task if it runs longer than
4. Expire
5. Enabled :

Notice that to tick this checkbox to enable these advanced settings. Fortunately, it is ticked by default.

#### Actions tab
There includes these components.

1. Action :

Determine what kind of actions will be performed. There are these options:

Start a Program, 

Send an e-mail,

Display a message.

2. Settings. See below

##### Settings

For settings when Actions is set to "Start a Program",

1. Program/script :
   
What script will be executed for when the scheduled task is executed.

2. Add arguments :
   
Optional. 

The arguments for the script that will be executed.

3. Starts in :

Optional.

#### Conditions tab

Determines the conditions to perform the scheduled task.

We skip the intro since there are too many things to introduce.

#### Settings tab

For additional settings.

We also skip the intro since there are too many things to introduce.

### Additional Reference

The reply on stackexchange.

https://superuser.com/questions/15596/automatically-run-a-script-when-i-log-on-to-windows

https://superuser.com/questions/302194/automatically-executing-commands-when-a-command-prompt-is-opened#:~:text=You%20can%20do%20it%20this%20way%3A%201%20Create,HKCU%5CSOFTWARE%5CMicrosoft%5CCommand%20Processor%20value%3A%20AutoRun%20type%3A%20REG_EXPAND_SZ%20data%3A%20%22%25AppData%25%5Caliases.cmd%22
