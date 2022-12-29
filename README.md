# timedatectl

Configure the systemd-timesyncd service.

## Requirements

There are no requirements for this role.

## Role Variables

timesyncd_servers - space separated list of servers to sync time with

timesyncd_params - see the file /etc/systemd/timesyncd.conf for reference

timezone - the timezone of the local machine

## Example Playbook

    - hosts: servers
      roles:
        - dillagr.timedatectl
          timesyncd_servers: "asia.pool.ntp.org"
          timezone: "Asia/Hongkong"


## License

GPL3.0
