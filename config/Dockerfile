FROM docker.io/networktocode/nautobot as final

USER root

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get autoremove -y && \
    apt-get clean all && \
    rm -rf /var/lib/apt/lists/*

USER nautobot

RUN pip --no-cache-dir install --upgrade pip wheel && \
    pip --no-cache-dir install nautobot-ssot && \
    pip --no-cache-dir install nornir-nautobot && \
    pip --no-cache-dir install nautobot-golden-config && \
    pip --no-cache-dir install nautobot-device-onboarding
