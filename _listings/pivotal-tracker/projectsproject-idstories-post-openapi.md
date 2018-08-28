---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 0
info:
  title: Pivotal Tracker Post Projects Project Stories
  description: Post projects project stories.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---