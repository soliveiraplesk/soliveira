Running the app in a local environment.

During the process to build the docker image some issues could happen due to the dockerfile instructions. The first one refers the python installation, its required to edit the file and change the instruction from:

RUN apt-get install -y python

to 

RUN apt-get install -y python3

The python service will be installed but another error will be generated from the instruction:

RUN pip3 install -r requirements.txt

The reason for this error is due to the lasted python updates. As suggested, the docker deployment in a local machine can be skipped and the additional tasks performed locally.

Install SQL server locally

Deploy a SQL locally, create a database, create the table store and insert the data specified.

HTTP Request

An HTTPS request can be done via Curl command to store the allys credentials, using HTTPS the credentials are going to be encrypted by default.



