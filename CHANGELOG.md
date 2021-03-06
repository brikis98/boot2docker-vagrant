# Changelog

## 0.12.0 (2015-05-07)

- Use our own vagrant box - [blinkreaction/boot2docker](https://vagrantcloud.com/blinkreaction/boxes/boot2docker)
  - Updated Docker to v1.6.0
  - Updated Docker Compose to v1.2.0
- [SMB2 (experimental)] sync folder option for Windows - complete automation of SMB sharing setup.
- Automatically start containers if docker-compose.yml is present in the Vagrantfile directory (single project mode)
- Miscellaneous code cleanup

## 0.11.1 (2015-04-09)

- Hotfix: added check for empty hosts in vagrant.yml

## 0.11.0 (2015-04-09)

- Using semantic versioning and tracking changes in the CHANGELOG.md file
- All configuration moved into vagrant.yml
- Refactored synced folders setup
  - Focused on better Windows support with SMB and rsync
  - Added an experimental `smb2` synced folder option, which does not require running vagrant as admin, but requires initial manual setup.
  - rsync can now be done per project instead of the whole <Projects> folder
- Documentation overhaul
- Fixes in setup.sh - making sure brew formulae are up to date.
