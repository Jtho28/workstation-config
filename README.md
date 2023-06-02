## Workstation Configuration
This is meant to be a continuation of my sway repo. The end goal is to delete the sway repo and use this instead because Ansible is much easier to manage. Just a few more commits to this and I'll probably be single! More time to work on it!

## Instructions
All you need to do is install ansible and run this command... </br>
`ansible-playbook setup.yml -i inventory.yml --connection=local --extra-vars "type=lemon" --ask-become-pass` </br>
Replace type with the sway configuration you'd like.

That being said, if you want to modify the playbook, i've attempted to include some stuff to help test, without modifying your host system. For pip, all you should need is `ansible`. 
However, you will need podman installed as well.

INSERT WORKING INSTRUCTIONS HERE (I don't know how to do this quite yet)

## WM Themes
Lemon - The lemon config files are what I use for my desktop.
Focused - The focused theme is kinda meant for laptops, I removed a lot of the transparency and rounded corners to try to save space for smaller displays. I would also like to significantly shrink the waybar if I can find a way to shrink the modules. It's not done yet.

## First-time Setup
So eventually I want a playbook that will just automate the entire setup of a workstation, based on the type of machine it is and specific variables that the user can override. I think this would be a cool way to set up computers whenever I get a new one. This could maybe even evolve into trying to create an entire distro remix, but we'll see.

# TO-DO
- automate sway output config based on ansible magic variables
- optionally install generic software that I like on my workstation
- windows and macOS support
- fix location of wofi on focused
- change the look of wofi, it looks silly rn
- create a few other themes
