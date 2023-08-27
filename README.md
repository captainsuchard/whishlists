<div align="center">
<img src="./brand/banner.svg" alt="">
<hr style="margin-top: 0.5rem; margin-bottom: 0.5rem;"/>
<img alt="License" src="https://img.shields.io/github/license/captainsuchard/wishlists?style=for-the-badge">
<img alt="GoLang Version" src="https://img.shields.io/github/go-mod/go-version/captainsuchard/wishlists?filename=backend%2Fgo.mod&style=for-the-badge&logo=go&label=Golang%20Version">
<img alt="Issues" src="https://img.shields.io/github/issues/captainsuchard/wishlists?style=for-the-badge&logo=github&label=Issues">
</div>

This repository contains a web application and backend to securely host your
own wishlists for birthdays, baby showers, christmas or any other occasion.

## Structure
Since the backend and frontend are closely related they are both in this
repository.
The folder `frontend` contains the application frontend which is based on 
React.js.
The folder `backend` contains the application backend written in Go.

The backend uses a MongoDB to store the wishlists since they are "just" a
JSON document and a MongoDB allows easy storage for such documents.
Futhermore, this makes moving wishlists between servers much easier than needing
to export a Postgres or MariaDB.

## Deployment
Since this project is still in its early stages there is no full deployment
method available.
The currently targeted method is a Docker container for each part 
(frontend, backend) since this allows an easy deployment for everybody.
However, for advanced users there will be a possiblity to just take the compiled
frontend files and host them on a http server (e.g. 
[caddy](https://caddyserver.com/)) and use a reverse proxy to host the backend
on a different server/port/etc.

> [!NOTE]  
> Further information will be provided here as soon as the development 
> progresses