FROM archlinux:base-devel

# Update repos and packages
RUN pacman --noconfirm  -Syu

# Install C/C++ programming tools (most come with base-devel tag)
RUN pacman --noconfirm -S meson ninja 

# Install JDK and some java tools
RUN pacman --noconfirm -S jdk11-openjdk openjdk11-doc gradle maven

# Install python
RUN pacman --noconfirm -S python

# Install miscellaneous tools
RUN pacman --noconfirm -S git neovim bash-completion

WORKDIR /mydir
