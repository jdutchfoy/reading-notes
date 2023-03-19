# README.md

## Read Assignment 13

To update something, the HTTP PUT method is used. This method will replace the current data of the target with the new content

The DELETE and PUT method grabs/requires the id of the target resource that needs to be deleted o updated. A unique identifier is necessary to remove or change a specific resource.

CRUD stands for Create, Read, Update, and Delete; it describes the four essential functions "that models should be able to do and are considered necessary to implement a persistent storage application 1". The four basic functions it represents are create, read, update, and delete, which corresponds to post, get, put, and delete in HTTP/REST methods. CRUD is a function that can live within REST; REST is a standard API architecture.

Bring in all the required libraries and routers required
require the model, connect to the database, create middleware
create endpoints and parameters needed, as well as create async functions needed
handle errors
Export the router/model
