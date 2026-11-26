Scenario: Add a new task successfully
  Given the user is logged in
  When the user adds a task "Study Python"
  Then the task should be added successfully
  And the task should appear in the task list

Scenario: Mark a task as completed
  Given the user has an existing task "Study Python"
  When the user marks the task as completed
  Then the task status should be "Completed"

Scenario: Reject an empty task
  Given the user is logged in
  When the user adds a task with an empty title
  Then the task should not be added
  And an error message "Task title is required" should be displayed