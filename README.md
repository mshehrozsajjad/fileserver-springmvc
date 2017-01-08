# fileserver-springmvc
<h3>Introduction</h3>
A file server is a dedicated machine, typically running on a local network which acts as a shared disk storage for authorized users. The utility of such an application can be increased many-folds by allowing web based public interfaces and dynamic group management for this service.

In order to provide public interfaces, we are using RESTful Web Services which are based on the REST architecture. These are light-weight, scalable and stateless web services; where the context is maintained by the client and not by the server. These allow you to define APIs with well-define interfaces, which can be shared with anyone publicly, allowing for direct access to the resources.
<h3>Features</h3>

A Spring based Web App which works using RESTful Web Services. This application will have the following features:
<ol>
   <li> Following MVC by using Spring MVC.</li>
   <li>Using RESTful webservices(e.g. for file upload use /project/file/upload)</li>
    <li>Authenticatin (login/logout) and Authorize the user using Spring Security.</li>
    <li>CSRF protection</li>
    <li>Allow file sharing between users</li>
      <li>In file upload, when the server receives file, it should divide the file in 5 parts and store these parts and their metadata.</li>
      <li>  Provide the user with a unique URL for the resource that can be shared with other users.</li>
       <li> A user can download a file by using the unique URL provided by the uploader.</li>
       <li> In file download the server will first combine the chunks of file and then send the combined single file as a response to the user request.</li>
    <li>Communication will be done using a standard protocol like JSON, XML etc</li>
    <li>Allowing sharing of resources via public links</li>
    <li>Using Hibernate for managing the database</li>
    <li>Loging all activities</li>
</ol>
