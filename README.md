# Limework fork of RedisBungee
[![RedisBungee Build](https://github.com/Limework/RedisBungee/actions/workflows/maven.yml/badge.svg)](https://github.com/Limework/RedisBungee/actions/workflows/maven.yml) [![](https://jitpack.io/v/limework/redisbungee.svg)](https://jitpack.io/#limework/redisbungee)

Spigot link: [click](https://www.spigotmc.org/resources/redisbungee.87700/)

The maintainer of RedisBungee has became inactive, so we have taken the development of the plugin.

RedisBungee uses [Redis](https://redis.io) to Synchronize data between [BungeeCord](https://github.com/SpigotMC/BungeeCord) proxies

# 0.7 API BREAKING CHANGE:
we do not advice using version (0.7) till we finish making it stable , 
but if you plan to use redis-bungee 0.7 the api has breaking change. 
JedisPool was changed to Pool<Jedis> to support Redis Sentinel
If ANYONE found a good way to fix this api breaking change
pull requests are welcomed :)
## Notice: about older versions of redis than redis 6.0

As of now Version 0.6.4-SNAPSHOT is only supporting redis 6.0 and above!

## Compiling

Now you can use Maven without installing it using [Maven wrappe](https://github.com/takari/maven-wrapper) :)

RedisBungee is distributed as a [maven](https://maven.apache.org) project. 

To compile and installing to in your local Maven repository:

    git clone https://github.com/Limework/RedisBungee.git .
    mvnw clean install
    mvnw package

If you have deb maven installed, you can use the `mvn` command instead.

And use it in your pom file.

    <dependency>
      <groupId>com.imaginarycode.minecraft</groupId>
      <artifactId>RedisBungee</artifactId>
      <version>0.6.4-SNAPSHOT</version>
      <scope>provided</scope>
    </dependency>

Or if you want to use the jitpack maven server

    <repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
    
And use it in your pom file.
    
    <dependency>
	    <groupId>com.github.limework</groupId>
	    <artifactId>redisbungee</artifactId>
	    <version>0.6.3</version>
	</dependency>


## Javadocs
Hosted on limework website. Version 0.6.0 (note: any version 0.6.* will not have API changes.)
https://limework.net/JavaDocs/RedisBungee/

## Configuration

**REDISBUNGEE REQUIRES A REDIS SERVER**, preferably with reasonably low latency. The default [config](https://github.com/limework/RedisBungee/blob/master/src/main/resources/example_config.yml) is saved when the plugin first starts.

## License!

This project is distributed under Eclipse Public License 1.0

You can find it [here](https://github.com/Limework/RedisBungee/blob/master/LICENSE)

You can find the original RedisBungee by minecrafter [here](https://github.com/minecrafter/RedisBungee) or spigot page [here](https://www.spigotmc.org/resources/redisbungee.13494/)

## YourKit

YourKit supports open source projects with innovative and intelligent tools for monitoring and profiling Java and .NET applications. YourKit is the creator of [YourKit Java Profiler](https://www.yourkit.com/java/profiler/), [YourKit .NET Profiler](https://www.yourkit.com/.net/profiler/) and [YourKit YouMonitor](https://www.yourkit.com/youmonitor/).

![YourKit](https://www.yourkit.com/images/yklogo.png)
