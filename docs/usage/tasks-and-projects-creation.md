# Tasks and projects creation

## All Docs Index
- [Usage](./README.md)

## Markdown tasks

### Create a task
You may write tasks *almost* everywhere in the vault using the shortcut `CTRL` +
`ALT` + `Q`, or simply typing a markdown task.

Excluded folders:

- `sources`, You don't want online links tasks to be shown as tasks.
- `templates`, Template files are excluded as well.

The tasks will then be shown in the obsidian-tasks queries inside the **daily**
and **periodic** notes.

### Create a project
A project is just a task enclosed in double brackets like that: `[[TASK_NAME]]`.

Example:

```md
- [ ] [[TASK_NAME]] ➕ 2023-05-07 📅 2024-01-31
```

This way, you may create a project note by clicking on the task link, and add some
tasks inside!

Projects are supposed to be created within an `Area` file of choice in the
`02 - Areas` folder. While there's no obligation, it just helps focusing on the
right things.

Don't forget to move project notes to the `01 - Projects` folder for easier
management.

#### WARNING
The markdown tasks using the obsidian-tasks properties holds a note in place of
the `task.description`. In other words, when a project is done, the project task
should be marked as done, and the project note(s) should be moved from the
`01 - Projects` folder to the `04 - Archives` folder.

### Create something using QuickAdd
You may use the QuickAdd plugin to create a task or a project.

Simply click on the QuickAdd button `Create Something` in the left ribbon and
select the type of task you want to create:

- Create Project -> Create a project in an `Area` file of choice in `02 - Areas`.
- Create One-Off Task -> Create a task in the `Notes` part of today's daily note
- Someday Maybe -> Create a list item in the Someday maybe inbox.

- Create Passion -> Create a new passion/media in the `Passions Backlog 🎮`
kanban board

### Import todoist tasks
You may import todoist tasks using the `Import from Todoist` QuickAdd button in
the left ribbon. You then just need to select the tasks you want.

This required to have the obsidian-todoist plugin configured. Please refer to the
[installation instructions][1].

You will have access to the same choices as the `Create Something` button, while
also being able to:

- Import selected Todoist tasks at the current cursor position as well.

## Tasks locations
- **One-off tasks**: Tasks created in the `Notes 📝` part of today's daily note
are considered as `one-off tasks`, meaning tasks that are not part of a project.

- **Project tasks**: Tasks created in a project note are considered as
`project tasks`, meaning tasks that are part of a project. To be fair, every tasks
not in a daily-note are considered as project tasks.

- **Focus 🔥 & Goals 🎯**: Tasks created in the `PERIOD Focus 🔥 & Goals 🎯
 section of a daily or periodic notes will be considered as stuff you want to
 focus on during the period, or goals you want to achieve.

- **Passions Backlog 🎮**: Tasks created in the `Passions Backlog 🎮` kanban
board are considered as `passion tasks`, meaning medias to watch, play, read, etc.

- **Someday maybe 💭**: Tasks created in the `Someday maybe` file are not really
tasks but just list items. They will one day be moved to action somewhere.

## Tasks properties
A task always have:

- A `status`

A task can have:
- A `created date`
- A `start date`
- A `scheduled date`
- A `due date`
- A `done date`
- A `cancelled date`
- A `reccurence rule`
- A `priority`
- One or many `tags` (using the `#` symbol)

Tags should come after the `task.description` and before the `task.properties`:

```md
- [ ] TASK_NAME #tag1 #tag2 #tag3 PRIORITY_ICON 🔁 RECCURENCE_RULE ➕ CREATION_DATE OTHER DATES...
```

GTD tags with associated queries in daily and periodic notes are:

- `#next` for next actions -> Other tags in the tasks are considered as contexts
(example: `#next #computer` will be considered as an action to do next when using a
`computer`)

- `#waiting` for waiting for tasks
- `#delegated` for delegated tasks

These may evolve with obsidian-tasks plugin, and you should refer to the
[official documentation][2] for more informations.

## Tasks statuses
- `- [ ]` -> Tasks to do
- `- [/]` -> Tasks in progress
- `- [x]` -> Tasks done
- `- [-]` -> Tasks cancelled
- `- [?]` -> Tasks on-hold

Clicking on a task status will change it to the next status.

`- [ ]` -> `- [/]` -> `- [x]` -> `- [ ]`

You may also change a task status by [many different ways][3].

[1]: ../getting-started/installation.md#how-to-login-to-plugins
[2]: https://publish.obsidian.md/tasks/Introduction
[3]: https://publish.obsidian.md/tasks/Editing/Toggling+and+Editing+Statuses