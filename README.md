KANBAN 看板
===========

Demo
----
Live demo hosted here on Heroku (database is reset daily):
[**LIVE DEMO**](http://kanban.seanomlor.com)

[![Screenshot](/app/assets/images/screenshot.jpg)](http://kanban.seanomlor.com)

Summary
-------
Kanban is a work-in-progress Trello clone I developed for a final project at [App Academy](http://appacademy.io), a 9-week Ruby on Rails and JavaScript web development intensive in San Francisco.

Built with Ruby on Rails on the backend as a JSON API for Backbone.js on the frontend.

System Requirements
-------------------
* set up [docker](https://docker.com/)
** set up [boot2docker](http://boot2docker.io/) if mac or linux
* set up [fig](http://www.fig.sh/)

Deployment
----------
* fig build
* fig run web bash -l -c 'rake db:setup'
* fig up

Test
----
Point Browser to http://localhost:3000 for linux host or http://192.168.59.103:3000/ for mac or windows

Notes
-----
* Hand-rolled Rails user authentication with BCrypt
* Custom, nested Rails JSON templating with [Rabl](https://github.com/nesquena/rabl)
* Backbone models/collections with [Backbone-relational.js](http://backbonerelational.org/)
* Auto-updating comment timestamps with jQuery [timeago](http://timeago.yarp.com)
* Editable board, list and card titles with jQuery [JEditable](http://www.appelsiini.net/projects/jeditable)

License
-------
Kanban is released under the [MIT License](/LICENSE).

---
Developed by [Sean Omlor](http://seanomlor.com)
Dockerized by [Zeke Dean](http://zeke-dean.com)
