## Table of Contents

* [About the Project](#about-the-project)
* [Technology](#technology)
* [Getting Started](#getting-started)
* [Installation](#installation)
* [Consuming](#consuming)
* [Behaviour Driven Development](#behaviour driven development)

## About The Project
This is a REST API that is used to post news, view information of departments and its employees(users). It has features that allows one access specific info about users and departments, view a list of all the users in a department and also the list of departments a user is associated with.

## Technology
* Java
* Spark Java(Make the News Api)
* JUnit(testing)
* Postgres(Database)
* Gradle(building app)
* Postman (test Api)


## Usage

This api is hosted on Heroku, so you can choose to consume using this link [https://org-news-portal.herokuapp.com/](https://org-news-portal.herokuapp.com/)

These are the REST api routes:

<table>
  <tr>
    <th>Behavior</th>
    <th>Path</th>
    <th>Http Verb</th>
  </tr>
  <tr>
    <td>Create a new departmetnt</td>
    <td>/department/new</td>
    <td>POST</td>
  </tr>
  <tr>
    <td>Delete a specific department</td>
    <td>/department/:department_id</td>
    <td>DELETE</td>
  </tr>
  <tr>
    <td>View info a specific department</td>
    <td>/department/:departmetn_id</td>
    <td>GET</td>
  </tr>
  <tr>
    <td>Get a list of all departments</td>
    <td>/departments</td>
    <td>GET</td>
  </tr>
  <tr>
    <td>Create a new user/employee</td>
    <td>/users/new</td>
    <td>POST</td>
  </tr>
  <tr>
    <td>Get a list of users</td>
    <td>/users</td>
    <td>GET</td>
  </tr>
  <tr>
    <td>Post news about a specific department</td>
    <td>/departments/:department_id/news/new</td>
    <td>POST</td>
  </tr>
  <tr>
    <td>Get a list of the news relating to specific department</td>
    <td>/departments/:department_id/news</td>
    <td>GET</td>
  </tr>
  <tr>
    <td>Add a user to a department</td>
    <td>departments/:department_id/user/:user_id/new</td>
    <td>POST</td>
  </tr>
  <tr>
    <td>View a list of the employees/users in a department</td>
    <td>/departments/:department_id/users</td>
    <td>GET</td>
  </tr>
  <tr>
    <td>View list of departments an employee is associated with</td>
    <td>/user/:user_id/departments</td>
    <td>GET</td>
  </tr>
</table>

## Behaviour Driven Development

* Post for department/user
* Get departments/users that were created in an a array