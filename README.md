# ANSIBLE ROS2

A quick way to install ROS2 on Ubuntu with ansible playbook!

> If you are using ROS1 please refer to this [repo](https://github.com/brucechanjianle/ansible-ros).

## Dependencies

```bash
sudo apt install ansible git -y
```

## Usage
Installing ROS2 only  
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "ros2_distribution=jazzy" -K
```

Installing ROS2 and zsh tab completion patch  
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "ros2_distribution=jazzy zsh_tab_completion=true" -K
```

For Docker
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "ros2_distribution=jazzy zsh_tab_completion=true"
```

## Zsh Tab Completion Patch

This would only run the patch for zsh tab completion!  
```bash
ansible-pull -U https://github.com/brucechanjianle/ansible-ros2 -e "only_zsh_patch=true zsh_tab_completion=true" -K
```

## About Sourcing
Sourcing of ROS2 is not done automatically as of now, please refer to [`.dotfiles/.bash_aliases`](https://github.com/BruceChanJianLe/dotfiles/blob/master/.bash_aliases)
on how to add the source command.


## Reference
- https://github.com/rarrais/ansible-role-ros2
- https://linuxhint.com/manage_ubuntu_package_repositories_ppas_ansible/
- https://stackoverflow.com/questions/58169348/how-is-the-architecture-fact-called-in-ansible
- https://askubuntu.com/questions/1398344/apt-key-deprecation-warning-when-updating-system
