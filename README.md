# Serverless ETLing
Making ETLing simpler using containers as a plug and play model.

The application with separate common pieces of the ETLing process into separate docker containers. For example, the unzip container in the project will takes a link as input then downloads and unzips the file at that link. A separate container can take a csv location as input and put it into a postgres database. This allows for plug and play ETLing pipelines for the data.

Using ACI, a user can define container groups with the exact elements they want. For example put the unzip and postgres modules together and can download a zip file from a datasource, unzip it then feed it into a databases all without writing a line of code. Also only pay per second usign the ACI instance. 

