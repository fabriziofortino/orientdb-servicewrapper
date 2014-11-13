A service wrapper execution for OrientDB Server using [Java Service Wrapper](http://wrapper.tanukisoftware.org/).

## Installation
1. Download the orientdb-servicewrapper zip file or clone the github repository.
2. Copy the `service` folder under the OrientDB `bin` directory.
3. Edit the `orientdb.conf` file and change the variable *set.default.ORIENTDB_HOME* with the OrientDB installation path.

## Use
To run OrientDB as a service go to the *bin/service* folder and execute the script `orientdb` with one of the following parameters:

| Parameter     | Description   |
| ------------- |:-------------:|
| console      | Execute OrientDB in the current console |
| start      | Start OrientDB in background as a daemon process      |
| stop | Stop OrientDB if running      |
| restart | Restart OrientDB if running, otherwise just start it      |
| condrestart | Restart OrientDB only if already running      |
| status | Show the OrientDB current status      |
| install | Install OrientDB to run as a system service (init.d / service)      |
| remove | Uninstall OrientDB as a system service (init.d / service)      |
| dump | Request a Java thread dump      |

## Options
By default orientdb-servicewrapper is configured to run OrientDB server with an initial heap size of 512M and a maximum heap size of 1024M. To change the memory configuration edit the properties *set.default.ORIENTDB_INIT_HEAP_SIZE* and *set.default.ORIENTDB_MAX_HEAP_SIZE* in the `orientdb.conf` file. 

## Blog Articles
[OrientDB in service mode with Java Service Wrapper](http://fabriziofortino.github.io/articles/running-orientdb-in-service-mode-with-jsw/)

## License
This project is a 'derived work' hence it is licensed with the same Java Service Wrapper Community Edition: [GPL version 2](http://www.gnu.org/licenses/gpl-2.0.html)).

For more details on the license agreement and terms of use see http://wrapper.tanukisoftware.com/doc/english/licenseCommunity.html

Java Service Wrapper requires a commercial license to run it on 64-bit Windows.
