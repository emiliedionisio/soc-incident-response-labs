# Troubleshooting

## Docker Removal

The CodePath installation script expects Docker to be removed before installation.

Commands used:

sudo apt-get remove -y docker docker-engine docker.io containerd runc docker-ce docker-ce-cli docker-ce-rootless-extras

sudo apt-get purge -y docker docker-engine docker.io containerd runc docker-ce docker-ce-cli docker-ce-rootless-extras

sudo apt-get autoremove -y

sudo rm -rf /var/lib/docker

## Docker Compose Removal

sudo rm -f /usr/local/bin/docker-compose

sudo rm -f /usr/bin/docker-compose

## apt-key Warning

During installation the script generated:

apt-key: command not found

Modern Ubuntu releases have deprecated apt-key. Despite the warning, the installation completed successfully.

## Docker Repository Warning

The installer also displayed:

NO_PUBKEY 7EA0A9C3F273FCD8

Docker packages were still installed successfully, and Catalyst containers started normally.

## Container Verification

Verify Catalyst is running:

sudo docker ps

Expected containers:

- catalyst
- nginx
- authelia
- arangodb
- minio

## Catalyst Login

URL: https://catalyst.localhost

Username: admin

Password: admin

## Threat Intelligence Resources

VirusTotal: https://www.virustotal.com/

AbuseIPDB: https://www.abuseipdb.com/

These services were used to enrich the Indicators of Compromise and validate malicious activity.
