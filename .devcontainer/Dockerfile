ARG VARIANT=16-bullseye
FROM mcr.microsoft.com/devcontainers/javascript-node:0-${VARIANT}

ARG NODE_MODULES="tslint-to-eslint-config typescript @google/clasp"
RUN su node -c "umask 0002 && npm install -g ${NODE_MODULES}" \
    && npm cache clean --force > /dev/null 2>&1