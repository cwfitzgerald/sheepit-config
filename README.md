# Sheepit Config

This is an example of a multi-gpu/cpu sheepit config. Right click on the powershell and click `Run with Powershell` to start it.

Relative paths are not relative to where you think they are, so you should ***ALWAYS USE ABSOLUTE PATHS*** in your config.

## Configuration

To set up, look in the config file and replace all things in <brackets> with the value you want. Generally you need to adjust:
	
  - Path to java in start-sheepit.ps1
  - Path to sheepit jar in start-sheepit.ps1
  - Username in configs
  - Password in configs
  - Hostname in configs
    - This is not a network hostname, this is just a name to give the client a label. Labels need not be unique.
  - Cpu cores in configs
    - Always use `cpu-count - gpu-count`. If you have 8 logical cores and 2 gpus, use 8 - 2 = 6 cores. GPU instances generally need one logical core.
  - Memory for cpu config
    - This is a number in bytes which can be modified with letters. `2G` for 2 gigabytes, `2M` and `2K` for megabytes and kilobytes.
