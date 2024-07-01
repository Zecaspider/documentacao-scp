# Ansible Role: sys-disk-cleanup

## Description

The `disk_cleanup` role is designed to automate routine disk maintenance tasks on Unix-based systems using Ansible. It ensures efficient disk usage by performing the following operations:

* **Clean Package Cache** : Removes unnecessary files from package manager cache, optimizing storage usage and potentially freeing up disk space.
* **Remove Unused Packages** : Automatically identifies and removes packages that are no longer required, further optimizing disk usage.
* **Clean Old Logs** : Searches and removes log files older than 30 days from specified directories (`/var/log/` by default), maintaining disk cleanliness and improving performance.
* **Clean Temporary Directories** : Clears out temporary directories (`/tmp/` by default), ensuring these spaces do not accumulate unnecessary files over time.

## Requirements

- Ansible 2.9 or higher

## Role Variables

This role does not have any configurable variables.

## Dependencies

This role does not have any external dependencies.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: sys-disk-cleanup
```

## License

This role is licensed under the MIT License.

## Author Information

This role was created is maintained by the DiS Team.

## Additional Notes
