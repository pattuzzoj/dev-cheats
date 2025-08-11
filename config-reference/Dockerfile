# Sets the base image for building the new image
FROM <base-image>

# Specifies the image author (deprecated, use LABEL)
MAINTAINER <name> <email>

# Adds metadata to the image
LABEL <key>=<value> \
      <key>=<value>

# Defines build-time variables (only available during build)
ARG <name>=<default-value>

# Sets environment variables
ENV <key>=<value> \
    <key>=<value>

# Sets the default shell for RUN commands
SHELL ["<path-to-shell>", "<option>"]

# Sets the working directory for subsequent instructions
WORKDIR <path>

# Copies files/directories from local to image
COPY <src> <dest>

# Adds local or remote files/directories (also extracts tar archives)
ADD <src> <dest>

# Executes commands at build time
RUN <command>

# Documents the port the container listens on
EXPOSE <port>

# Creates a mount point for external volumes
VOLUME ["<path>"]

# Sets the user (and optionally group) to run processes
USER <user>[:<group>]

# Defines a command to check container health
HEALTHCHECK --interval=<time> --timeout=<time> CMD <command> || exit 1

# Specifies the system call signal to stop the container
STOPSIGNAL <signal>

# Adds instructions triggered when the image is used as a base
ONBUILD <instruction> <args>

# Sets the default executable for the container
ENTRYPOINT ["<executable>", "<param>"]

# Provides default parameters for ENTRYPOINT or default command
CMD ["<param>", "<param>"]