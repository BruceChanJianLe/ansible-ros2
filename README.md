# ANSIBLE ROS2

A quick way to install ROS2 on Ubuntu with ansible playbook!
If you are using ROS1 please refer to this [repo](https://github.com/brucechanjianle/ansible-ros).

## Dependencies

```bash
sudo apt install ansible git -y
```

## Usage
Installing ROS2
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "ros2_distribution=foxy" -K
```

For Docker
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "ros2_distribution=foxy"
```

## About Sourcing
Sourcing of ROS2 is not done automatically as of now, please refer to `.dotfiles/.bash_aliases` on how to add the source command.

Reference: https://github.com/rarrais/ansible-role-ros2

## Reference

- https://linuxhint.com/manage_ubuntu_package_repositories_ppas_ansible/
- https://stackoverflow.com/questions/58169348/how-is-the-architecture-fact-called-in-ansible
- https://askubuntu.com/questions/1398344/apt-key-deprecation-warning-when-updating-system
