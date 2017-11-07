# MetadataTable
Work on and around an interactive metadata table for sequence submission and modification


SRA Metadata is rich, sometimes too rich.  There's no single standardized location for many types of useful information.
This is a generalizable framework for pullking SRA metadata and summarizing usefully, with some common use-cases ready to go.

What's the problem?
Even the type of study is heterogeneous for different submitters.  The location of for instance tissue and developmental stage specifications within SRA metadata also varies, as do the values used to describe particular tissues.

Why should we solve it?

Third-party efforts to load all metadata into a relational db suggest how widespread the problem is-- a customizable localized implementation helps many.

What is ?

Overview Diagram

How to use

Installation options:

We provide two options for installing : Docker or directly from Github.

Docker

The Docker image contains as well as a webserver and FTP server in case you want to deploy the FTP server. It does also contain a web server for testing the main website (but should only be used for debug purposes).

docker pull ncbihackathons/<this software> command to pull the image from the DockerHub
docker run ncbihackathons/<this software> Run the docker image from the master shell script
Edit the configuration files as below
Installing from Github

git clone https://github.com/NCBI-Hackathons/<this software>.git
Edit the configuration files as below
sh server/<this software>.sh to test
Add cron job as required (to execute .sh script)
Configuration

Examples here

Testing

We tested
