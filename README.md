# Logstash Plugin

This is a plugin for [Logstash](https://github.com/elasticsearch/logstash).

It is fully free and fully open source. The license is GNU GPL v2.0, meaning you are pretty much free to use it however you want in whatever way.

## Documentation

This plugin based logstash 1.4.2.

## Need Help?

Need help? Just send emails shaogx@gmail.com.

## Install

### 1. download code via git or zip.

### 2. copy the code to logstash_path/lib and spec directories.

### 3. configure

output {
				beanstalk {
					delay => 0 # number, default: 0
					host => '172.16.20.xxx' # string (required)
					port => 11300 # number, default: 11300
					priority => 65536 # number, default: 65536
					ttr => 300 # number, default: 300
					tube => 'logstash' # string (required)
				}
}



