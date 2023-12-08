# ANSIBLE ROS2

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
