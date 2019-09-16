FROM python:3.7

ENV DEVCONTAINER True

RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        git \
        nodejs \
        yarn \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Install python dependencies
RUN python -m pip install --upgrade colorlog black pylint python-language-server

# Install latest Home Assistant dev version
RUN python -m pip install --upgrade git+git://github.com/home-assistant/home-assistant.git@dev

# Create the custom_components directory
RUN cd && mkdir -p /config/custom_components


# Set workspace
WORKDIR /workspace

# Set the default shell to bash instead of sh
ENV SHELL /bin/bash
