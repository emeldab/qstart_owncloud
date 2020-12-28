# Quickstart for Installing and Using ownCloud

An ownCloud server lets you synchronize and share files with a desktop or mobile client. This guide demonstrates how to install and use ownCloud on your own Linux server. It addresses the following steps:
* Install and configure an ownCloud server.
* Enable users to connect to an ownCloud server using the server's IP address and port 8080.
* Connect to an ownCloud server using a desktop or mobile client.
* Add a user account.

## Installing and Configuring an ownCloud Server
You install and configure ownCloud according to your setup and needs. You may be a single-user or mid-sized enterprise and therefore, it is important to understand  the requirements and considerations to take into account.

**Note**: To be able to connect to ownCloud using the server's IP address and port 8080, make sure you install [ownCloud with Docker](https://doc.owncloud.com/server/10.5/admin_manual/installation/docker/).

1. Download [ownCloud](https://owncloud.com/download-server/).
2. Configure your web server.
3. Run the installation wizard.

We recommend that you refer to the documentation for details on installing and configuring ownCloud:
* [Installation](https://doc.owncloud.com/server/10.3/admin_manual/installation/).
* [Configuration](https://doc.owncloud.com/server/10.3/admin_manual/configuration/).

## Connecting to an ownCloud Server Using the Server's IP Address and Port 8080
You install ownCloud with Docker and set your configuration file to be able connect to the server's IP address and HTTP-connect to port-8080.

1. Make sure you installed ownCloud using Docker locally.
2. Create a new project directory.
3. Copy [docker-compose.yml from the GitHub repository](https://raw.githubusercontent.com/owncloud/docs/master/modules/admin_manual/examples/installation/docker/docker-compose.yml).
4. Create the environment configuration file.
5. Build and start the container.
6. Open http://localhost:8080 in a browser to log in to the ownCloud UI.

For details, see [Docker Compose](https://doc.owncloud.com/server/10.5/admin_manual/installation/docker/#docker-compose).

## Connecting to an ownCloud Server Using a Desktop or Mobile Client
### Desktop Client
The installation wizard guides you step-by-step to connect to your ownCloud server using a desktop client.

1. Enter your server URL.
2. Enter your ownCloud login on the next screen.
3. Click the **Connect** button after you complete selecting your sync folders.

For details, see [Installing the Desktop Synchronization Client](https://doc.owncloud.org/desktop/2.5/installing.html#installation-wizard).

### Mobile Devices
You can connect to ownCloud using mobile devices on Android and iOS.

1. Enter your server URL, login name, and password.
2. Click the **Connect** button. 

For details, see:
* **Android** - [Connecting to Your ownCloud Server](https://doc.owncloud.org/android/#connecting-to-your-owncloud-server).
* **IOS** - [Getting the ownCloud iOS App](https://doc.owncloud.com/ios/#getting-the-owncloud-ios-app).

## Adding a User Account
An administrator manages user-related configuration tasks such as adding new user accounts.

1. Enter the new user’s **Login Name** and **initial Password** (cannot be "0").
2. Assign **Groups** memberships (optional).
3. Click the **Create** button.

For details, see [Create a New User](https://doc.owncloud.org/server/10.0/admin_manual/configuration/user/user_configuration.html#creating-a-new-user).
