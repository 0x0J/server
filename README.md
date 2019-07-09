# server 

Server is a package used to make a general design for all sort of server types.
This can be wrappers for a database, api or any kind of connection.

The use case is for Programs that need to access a number of different apis, dbs or ssh connections, in an effort to make the design for each of those server wrappers as common as possible for an easier overview and maintainable state.

Server is actually just an interface with a set of methods to have.
The rest of this package is for making it easier to follow the server standard, such as the cmd tool to generate a template for 
the kind of wrapper wanted, etc db.

There is a ServerContainer which is a helper struct that can store these generated servers
and make sure connections are maintained or reconnected etc.

