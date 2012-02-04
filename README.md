NapkinDrawings.com
==================

Overview
--------

NapkinDrawings.com is an online spreadsheet application to store data for collaboration and scheduling.

Dependencies
------------

The system is dependent on a number of outside services and projects to operate. These dependencies are listed
below in application stack order.

**Twitter Bootstrap**
Twitter bootstrap is used to provide a fast and robust HTML/CSS infrastructure to build UI elements with. In
addition, the bootstrap-alert and bootstrap-modal JavaScript extensions are used for notifications and other
overlay interactions.

**Raphael**
Charting for the monitoring and statistics section is built using the gRaphael charting library. There are 
several dependencies here.

*Raphael* - The core Rapahel library
*gRaphael* - The base graphing library
*gRaphael-pie* - The pie chart extension to gRaphael
*gRaphael-bar* - The bar chart extension to gRaphael
*gRaphael-line* - The line chart extension to gRaphael

**Backbone**
Backbone.js is used to provide client side rendering of all UI elements. Backbone provides the workhorse for
the application, which interacts with the ReST API endpoint to collect data for display. Templating is handled
by Mustache.js.

**Underscore**
Backbone.js depends on jQuery and Underscore.js. Additional utility is available in the library, providing use
beyond simple dependency satisfaction.

**jQuery**
jQuery is required for DOM manipulation and animations in Backbone.js. It is extremely useful outside of this
capacity as well.

**Mustache**
All templating is handled by Mustache.js, which is an extremely convenient and ubiquitous template format.

**Socket.io**
Realtime push and notification features for live updating of data values in the sheet, as well as search and
monitoring features.

**Express**
Express is a robust server side MVC framework for Node. This framework is responsible for generating the views 
that will be rendered by backbone to create the interface. There are additional modules that are used for 
additional functionality, listed below.

*Express-Configure* - Configuration loading from datas store, such as Redis

**Node**

*mongoose*
*cluster* - A multicore server management for node.js
*connect* - A convenient I/O layer for Node
*connect-redis* - Express session manager in redis
*redis* - Required by connect-redis
*hiredis* - Required by redis for hi performance redis connections (native C driver instead of pure JS)
*url* - A URL manipulation module for Node to aid with the processing of URLs

**Nginx**
**Redis**
**MongoDB**
