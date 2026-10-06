# VM deployment

The systemd units in this directory define the runtime contract. They are not framework installers.

Before installation:

1. Create the `app` service account.
2. Install the runtime required by the selected framework.
3. Install the application under `/opt/${{ values.name }}/`.
4. Create environment files under `/etc/${{ values.name }}/`.
5. Restrict environment-file permissions.
6. Enable only the tiers selected for the service.
7. Put a TLS-capable reverse proxy in front of externally exposed services where appropriate.
