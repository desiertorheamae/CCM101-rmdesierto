# Mission Reflection

Object storage is more suitable for storing millions of photos because it is designed to manage large amounts of unstructured data. Unlike traditional block storage, object storage keeps each file as a separate object with its own information and identifier. It can also expand as more files are added, which makes it useful for applications that store a large number of photos.

Docker made the deployment of the MinIO storage server easier because it allowed me to set up the server using a single command. I did not have to install and configure each required component separately. The Docker command also allowed me to set the username and password through environment variables when the MinIO container was started.

A bucket is a container used to organize and store objects in an object storage system. In this activity, I created a bucket named `client-photos` through the MinIO Web Console. I also uploaded a sample file to the bucket to confirm that the storage server was working properly.

Large companies use several methods to protect their stored data from being lost when a physical server fails. They may keep multiple copies of their data, use backups, and store data across different servers or locations. These methods help ensure that the data can still be accessed even if one server experiences a hardware problem.

My confidence in using the Linux command line has improved through this laboratory activity. I became more comfortable navigating directories, checking files, using Git commands, and deploying a service with Docker. I also learned how command-line tools can be used to manage cloud services. At first, some commands were unfamiliar to me, but practicing them throughout the activity helped me become more confident in working with Linux.
