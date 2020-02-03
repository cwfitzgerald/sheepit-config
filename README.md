# Sheepit Config

This is an example of a multi-gpu/cpu sheepit config. Right click on the powershell and click `Run with Powershell` to start it.

## Configuration

To set up, look in the config file and replace all things in <brackets> with the value you want. Generally you need to adjust:
	
  - Path to java in start-sheepit.ps1
  - Username in configs
  - Password in configs
  - Hostname in configs
  - Cpu cores in configs
    - Always use `cpu-count - gpu-count`. If you have 8 cores and 2 gpus, use 8 - 2 = 6 cores. GPU instances generally need one core.
