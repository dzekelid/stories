---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{PROJECT_ID}/stories/{STORY_ID}:
    get:
      summary: Get Projects Project Stories Story
      description: Retrieves information about a single story.
      operationId: getProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
    put:
      summary: Put Projects Project Stories Story
      description: Put projects project stories story.
      operationId: putProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
    delete:
      summary: Delete Projects Project Stories Story
      description: Delete projects project stories story.
      operationId: deleteProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-delete
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
  /projects/{PROJECT_ID}/stories:
    get:
      summary: Get Projects Project Stories
      description: Retrieves all stories for a project, or those matching filter(s)
      operationId: getProjectsProjectStories
      x-api-path-slug: projectsproject-idstories-get
      parameters:
      - in: query
        name: filter
        description: A filter for the returned stories to match
      - in: query
        name: limit
        description: Controls the maximum number of stories returned
      - in: query
        name: offset
        description: Controls the number of stories to skip from the beginning of
          the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
    post:
      summary: Post Projects Project Stories
      description: Post projects project stories.
      operationId: postProjectsProjectStories
      x-api-path-slug: projectsproject-idstories-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
  /projects/{PROJECT_ID}/stories/{STORY_ID}/notes:
    put:
      summary: Put Projects Project Stories Story Notes
      description: Put projects project stories story notes.
      operationId: putProjectsProjectStoriesStoryNotes
      x-api-path-slug: projectsproject-idstoriesstory-idnotes-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Notes
  /projects/{PROJECT_ID}/stories/deliver_all_finished:
    post:
      summary: Post Projects Project Stories Deliver All Finished
      description: Takes all finished stories and marks them as delivered. This could
        be used to automate a demo deploy process. The updated stories are returned
        as the result.
      operationId: postProjectsProjectStoriesDeliverAllFinished
      x-api-path-slug: projectsproject-idstoriesdeliver-all-finished-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - Deliver
      - ""
      - Finished
  /projects/{PROJECT_ID}/stories/{STORY_ID}/moves:
    post:
      summary: Post Projects Project Stories Story Moves
      description: Moves a story before or after another story. The moved story is
        returned in the response.
      operationId: postProjectsProjectStoriesStoryMoves
      x-api-path-slug: projectsproject-idstoriesstory-idmoves-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Moves
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks/{TASK_ID}:
    get:
      summary: Get Projects Project Stories Story Tasks Task
      description: Get projects project stories story tasks task.
      operationId: getProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    put:
      summary: Put Projects Project Stories Story Tasks Task
      description: Put projects project stories story tasks task.
      operationId: putProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    delete:
      summary: Delete Projects Project Stories Story Tasks Task
      description: Delete projects project stories story tasks task.
      operationId: deleteProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-delete
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks:
    get:
      summary: Get Projects Project Stories Story Tasks
      description: Get projects project stories story tasks.
      operationId: getProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
    post:
      summary: Post Projects Project Stories Story Tasks
      description: Post projects project stories story tasks.
      operationId: postProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
  /projects/{PROJECT_ID}/stories/{STORY_ID}/attachments:
    post:
      summary: Post Projects Project Stories Story Attachments
      description: Post projects project stories story attachments.
      operationId: postProjectsProjectStoriesStoryAttachments
      x-api-path-slug: projectsproject-idstoriesstory-idattachments-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Attachments
---